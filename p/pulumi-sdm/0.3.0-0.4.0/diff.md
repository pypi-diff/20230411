# Comparing `tmp/pulumi_sdm-0.3.0.tar.gz` & `tmp/pulumi_sdm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_sdm-0.3.0.tar", last modified: Tue Sep 20 15:20:36 2022, max compression
+gzip compressed data, was "dist/pulumi_sdm-0.4.0.tar", last modified: Tue Apr 11 08:38:55 2023, max compression
```

## Comparing `pulumi_sdm-0.3.0.tar` & `pulumi_sdm-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm/
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   677511 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8154 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     9091 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/account.py
--rw-r--r--   0 runner    (1001) docker     (121)     8065 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/account_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)     9188 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     5451 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_account_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)     8804 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     6531 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     4612 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_remote_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     7600 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     4584 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_role.py
--rw-r--r--   0 runner    (1001) docker     (121)     5900 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/get_ssh_ca_pubkey.py
--rw-r--r--   0 runner    (1001) docker     (121)     8260 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/node.py
--rw-r--r--   0 runner    (1001) docker     (121)   974894 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8364 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (121)   138548 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)     9738 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/role.py
--rw-r--r--   0 runner    (1001) docker     (121)    23471 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/pulumi_sdm/secret_store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2154 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/pulumi_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-20 15:20:36.000000 pulumi_sdm-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-09-20 15:20:35.000000 pulumi_sdm-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   769508 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/account_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_remote_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/get_ssh_ca_pubkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1110292 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145518 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm/secret_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/pulumi_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-11 08:38:55.000000 pulumi_sdm-0.4.0/setup.py
```

### Comparing `pulumi_sdm-0.3.0/PKG-INFO` & `pulumi_sdm-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_sdm
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pulumi_sdm-0.3.0/README.md` & `pulumi_sdm-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/__init__.py` & `pulumi_sdm-0.4.0/pulumi_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/_inputs.py` & `pulumi_sdm-0.4.0/pulumi_sdm/_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,25 +16,28 @@
     'NodeRelayArgs',
     'ResourceAksArgs',
     'ResourceAksBasicAuthArgs',
     'ResourceAksServiceAccountArgs',
     'ResourceAksServiceAccountUserImpersonationArgs',
     'ResourceAksUserImpersonationArgs',
     'ResourceAmazonEksArgs',
+    'ResourceAmazonEksInstanceProfileArgs',
+    'ResourceAmazonEksInstanceProfileUserImpersonationArgs',
     'ResourceAmazonEksUserImpersonationArgs',
     'ResourceAmazonEsArgs',
     'ResourceAmazonmqAmqp091Args',
     'ResourceAthenaArgs',
     'ResourceAuroraMysqlArgs',
     'ResourceAuroraPostgresArgs',
     'ResourceAwsArgs',
     'ResourceAwsConsoleArgs',
     'ResourceAwsConsoleStaticKeyPairArgs',
     'ResourceAzureArgs',
     'ResourceAzureCertificateArgs',
+    'ResourceAzureMysqlArgs',
     'ResourceAzurePostgresArgs',
     'ResourceBigQueryArgs',
     'ResourceCassandraArgs',
     'ResourceCitusArgs',
     'ResourceClustrixArgs',
     'ResourceCockroachArgs',
     'ResourceDb2IArgs',
@@ -87,14 +90,15 @@
     'ResourceSshCustomerKeyArgs',
     'ResourceSybaseArgs',
     'ResourceSybaseIqArgs',
     'ResourceTeradataArgs',
     'SecretStoreAwsArgs',
     'SecretStoreAzureStoreArgs',
     'SecretStoreCyberarkConjurArgs',
+    'SecretStoreCyberarkPamArgs',
     'SecretStoreCyberarkPamExperimentalArgs',
     'SecretStoreDelineaStoreArgs',
     'SecretStoreGcpStoreArgs',
     'SecretStoreVaultApproleArgs',
     'SecretStoreVaultTlsArgs',
     'SecretStoreVaultTokenArgs',
 ]
@@ -167,26 +171,38 @@
 
 @pulumi.input_type
 class AccountUserArgs:
     def __init__(__self__, *,
                  email: pulumi.Input[str],
                  first_name: pulumi.Input[str],
                  last_name: pulumi.Input[str],
+                 external_id: Optional[pulumi.Input[str]] = None,
+                 managed_by: Optional[pulumi.Input[str]] = None,
+                 permission_level: Optional[pulumi.Input[str]] = None,
                  suspended: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] email: The User's email address. Must be unique.
         :param pulumi.Input[str] first_name: The User's first name.
         :param pulumi.Input[str] last_name: The User's last name.
+        :param pulumi.Input[str] external_id: External ID is an alternative unique ID this user is represented by within an external service.
+        :param pulumi.Input[str] managed_by: Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
+        :param pulumi.Input[str] permission_level: PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
         :param pulumi.Input[bool] suspended: The User's suspended state.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "first_name", first_name)
         pulumi.set(__self__, "last_name", last_name)
+        if external_id is not None:
+            pulumi.set(__self__, "external_id", external_id)
+        if managed_by is not None:
+            pulumi.set(__self__, "managed_by", managed_by)
+        if permission_level is not None:
+            pulumi.set(__self__, "permission_level", permission_level)
         if suspended is not None:
             pulumi.set(__self__, "suspended", suspended)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
@@ -221,14 +237,50 @@
         return pulumi.get(self, "last_name")
 
     @last_name.setter
     def last_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "last_name", value)
 
     @property
+    @pulumi.getter(name="externalId")
+    def external_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        External ID is an alternative unique ID this user is represented by within an external service.
+        """
+        return pulumi.get(self, "external_id")
+
+    @external_id.setter
+    def external_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "external_id", value)
+
+    @property
+    @pulumi.getter(name="managedBy")
+    def managed_by(self) -> Optional[pulumi.Input[str]]:
+        """
+        Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
+        """
+        return pulumi.get(self, "managed_by")
+
+    @managed_by.setter
+    def managed_by(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "managed_by", value)
+
+    @property
+    @pulumi.getter(name="permissionLevel")
+    def permission_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
+        """
+        return pulumi.get(self, "permission_level")
+
+    @permission_level.setter
+    def permission_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "permission_level", value)
+
+    @property
     @pulumi.getter
     def suspended(self) -> Optional[pulumi.Input[bool]]:
         """
         The User's suspended state.
         """
         return pulumi.get(self, "suspended")
 
@@ -250,36 +302,48 @@
 
 
 @pulumi.input_type
 class NodeGatewayArgs:
     def __init__(__self__, *,
                  listen_address: pulumi.Input[str],
                  bind_address: Optional[pulumi.Input[str]] = None,
+                 device: Optional[pulumi.Input[str]] = None,
                  gateway_filter: Optional[pulumi.Input[str]] = None,
+                 location: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 token: Optional[pulumi.Input[str]] = None):
+                 token: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
         :param pulumi.Input[str] bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
+        :param pulumi.Input[str] device: Device is a read only device name uploaded by the gateway process when  it comes online.
         :param pulumi.Input[str] gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
+        :param pulumi.Input[str] location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param pulumi.Input[str] name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        :param pulumi.Input[str] version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         pulumi.set(__self__, "listen_address", listen_address)
         if bind_address is not None:
             pulumi.set(__self__, "bind_address", bind_address)
+        if device is not None:
+            pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
+        if location is not None:
+            pulumi.set(__self__, "location", location)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="listenAddress")
     def listen_address(self) -> pulumi.Input[str]:
         """
         The public hostname/port tuple at which the gateway will be accessible to clients.
         """
@@ -298,27 +362,51 @@
         return pulumi.get(self, "bind_address")
 
     @bind_address.setter
     def bind_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bind_address", value)
 
     @property
+    @pulumi.getter
+    def device(self) -> Optional[pulumi.Input[str]]:
+        """
+        Device is a read only device name uploaded by the gateway process when  it comes online.
+        """
+        return pulumi.get(self, "device")
+
+    @device.setter
+    def device(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "device", value)
+
+    @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[pulumi.Input[str]]:
         """
         GatewayFilter can be used to restrict the peering between relays and gateways.
         """
         return pulumi.get(self, "gateway_filter")
 
     @gateway_filter.setter
     def gateway_filter(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway_filter", value)
 
     @property
     @pulumi.getter
+    def location(self) -> Optional[pulumi.Input[str]]:
+        """
+        Location is a read only network location uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "location")
+
+    @location.setter
+    def location(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "location", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         """
         return pulumi.get(self, "name")
 
     @name.setter
@@ -342,35 +430,71 @@
     def token(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
+    @property
+    @pulumi.getter
+    def version(self) -> Optional[pulumi.Input[str]]:
+        """
+        Version is a read only sdm binary version uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "version", value)
+
 
 @pulumi.input_type
 class NodeRelayArgs:
     def __init__(__self__, *,
+                 device: Optional[pulumi.Input[str]] = None,
                  gateway_filter: Optional[pulumi.Input[str]] = None,
+                 location: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 token: Optional[pulumi.Input[str]] = None):
+                 token: Optional[pulumi.Input[str]] = None,
+                 version: Optional[pulumi.Input[str]] = None):
         """
+        :param pulumi.Input[str] device: Device is a read only device name uploaded by the gateway process when  it comes online.
         :param pulumi.Input[str] gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
+        :param pulumi.Input[str] location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param pulumi.Input[str] name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        :param pulumi.Input[str] version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
+        if device is not None:
+            pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
+        if location is not None:
+            pulumi.set(__self__, "location", location)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def device(self) -> Optional[pulumi.Input[str]]:
+        """
+        Device is a read only device name uploaded by the gateway process when  it comes online.
+        """
+        return pulumi.get(self, "device")
+
+    @device.setter
+    def device(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "device", value)
 
     @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[pulumi.Input[str]]:
         """
         GatewayFilter can be used to restrict the peering between relays and gateways.
         """
@@ -378,14 +502,26 @@
 
     @gateway_filter.setter
     def gateway_filter(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "gateway_filter", value)
 
     @property
     @pulumi.getter
+    def location(self) -> Optional[pulumi.Input[str]]:
+        """
+        Location is a read only network location uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "location")
+
+    @location.setter
+    def location(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "location", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         """
         return pulumi.get(self, "name")
 
     @name.setter
@@ -409,14 +545,26 @@
     def token(self) -> Optional[pulumi.Input[str]]:
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "token", value)
 
+    @property
+    @pulumi.getter
+    def version(self) -> Optional[pulumi.Input[str]]:
+        """
+        Version is a read only sdm binary version uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "version", value)
+
 
 @pulumi.input_type
 class ResourceAksArgs:
     def __init__(__self__, *,
                  hostname: pulumi.Input[str],
                  name: pulumi.Input[str],
                  port: pulumi.Input[int],
@@ -432,21 +580,23 @@
                  secret_store_certificate_authority_key: Optional[pulumi.Input[str]] = None,
                  secret_store_certificate_authority_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_key_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -476,14 +626,16 @@
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_client_key_key is not None:
             pulumi.set(__self__, "secret_store_client_key_key", secret_store_client_key_key)
         if secret_store_client_key_path is not None:
             pulumi.set(__self__, "secret_store_client_key_path", secret_store_client_key_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Input[str]:
         return pulumi.get(self, "hostname")
@@ -667,14 +819,26 @@
 
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -694,22 +858,24 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -727,14 +893,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -866,14 +1034,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -901,23 +1081,25 @@
                  healthcheck_namespace: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  remote_identity_group_id: Optional[pulumi.Input[str]] = None,
                  remote_identity_healthcheck_username: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_token_key: Optional[pulumi.Input[str]] = None,
                  secret_store_token_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] secret_store_token_key: * kubernetes_user_impersonation:
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -933,14 +1115,16 @@
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_token_key is not None:
             pulumi.set(__self__, "secret_store_token_key", secret_store_token_key)
         if secret_store_token_path is not None:
             pulumi.set(__self__, "secret_store_token_path", secret_store_token_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -1066,14 +1250,26 @@
 
     @secret_store_token_path.setter
     def secret_store_token_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_token_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -1099,23 +1295,25 @@
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  healthcheck_namespace: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_token_key: Optional[pulumi.Input[str]] = None,
                  secret_store_token_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] secret_store_token_key: * kubernetes_user_impersonation:
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -1127,14 +1325,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_token_key is not None:
             pulumi.set(__self__, "secret_store_token_key", secret_store_token_key)
         if secret_store_token_path is not None:
             pulumi.set(__self__, "secret_store_token_path", secret_store_token_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -1242,14 +1442,26 @@
 
     @secret_store_token_path.setter
     def secret_store_token_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_token_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -1282,21 +1494,23 @@
                  secret_store_certificate_authority_key: Optional[pulumi.Input[str]] = None,
                  secret_store_certificate_authority_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_key_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -1322,14 +1536,16 @@
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_client_key_key is not None:
             pulumi.set(__self__, "secret_store_client_key_key", secret_store_client_key_key)
         if secret_store_client_key_path is not None:
             pulumi.set(__self__, "secret_store_client_key_path", secret_store_client_key_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Input[str]:
         return pulumi.get(self, "hostname")
@@ -1495,14 +1711,26 @@
 
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -1534,21 +1762,23 @@
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
@@ -1589,14 +1819,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "cluster_name")
@@ -1834,14 +2066,592 @@
 
     @secret_store_secret_access_key_path.setter
     def secret_store_secret_access_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_secret_access_key_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
+class ResourceAmazonEksInstanceProfileArgs:
+    def __init__(__self__, *,
+                 cluster_name: pulumi.Input[str],
+                 endpoint: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 region: pulumi.Input[str],
+                 bind_interface: Optional[pulumi.Input[str]] = None,
+                 certificate_authority: Optional[pulumi.Input[str]] = None,
+                 egress_filter: Optional[pulumi.Input[str]] = None,
+                 healthcheck_namespace: Optional[pulumi.Input[str]] = None,
+                 remote_identity_group_id: Optional[pulumi.Input[str]] = None,
+                 remote_identity_healthcheck_username: Optional[pulumi.Input[str]] = None,
+                 role_arn: Optional[pulumi.Input[str]] = None,
+                 role_external_id: Optional[pulumi.Input[str]] = None,
+                 secret_store_certificate_authority_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_certificate_authority_path: Optional[pulumi.Input[str]] = None,
+                 secret_store_id: Optional[pulumi.Input[str]] = None,
+                 secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
+                 secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] bind_interface: Bind interface
+        :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "cluster_name", cluster_name)
+        pulumi.set(__self__, "endpoint", endpoint)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "region", region)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if certificate_authority is not None:
+            pulumi.set(__self__, "certificate_authority", certificate_authority)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if healthcheck_namespace is not None:
+            pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if role_arn is not None:
+            pulumi.set(__self__, "role_arn", role_arn)
+        if role_external_id is not None:
+            pulumi.set(__self__, "role_external_id", role_external_id)
+        if secret_store_certificate_authority_key is not None:
+            pulumi.set(__self__, "secret_store_certificate_authority_key", secret_store_certificate_authority_key)
+        if secret_store_certificate_authority_path is not None:
+            pulumi.set(__self__, "secret_store_certificate_authority_path", secret_store_certificate_authority_path)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if secret_store_role_arn_key is not None:
+            pulumi.set(__self__, "secret_store_role_arn_key", secret_store_role_arn_key)
+        if secret_store_role_arn_path is not None:
+            pulumi.set(__self__, "secret_store_role_arn_path", secret_store_role_arn_path)
+        if secret_store_role_external_id_key is not None:
+            pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
+        if secret_store_role_external_id_path is not None:
+            pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="clusterName")
+    def cluster_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "cluster_name")
+
+    @cluster_name.setter
+    def cluster_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_name", value)
+
+    @property
+    @pulumi.getter
+    def endpoint(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "endpoint")
+
+    @endpoint.setter
+    def endpoint(self, value: pulumi.Input[str]):
+        pulumi.set(self, "endpoint", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def region(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "region")
+
+    @region.setter
+    def region(self, value: pulumi.Input[str]):
+        pulumi.set(self, "region", value)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[pulumi.Input[str]]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @bind_interface.setter
+    def bind_interface(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "bind_interface", value)
+
+    @property
+    @pulumi.getter(name="certificateAuthority")
+    def certificate_authority(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "certificate_authority")
+
+    @certificate_authority.setter
+    def certificate_authority(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "certificate_authority", value)
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @egress_filter.setter
+    def egress_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "egress_filter", value)
+
+    @property
+    @pulumi.getter(name="healthcheckNamespace")
+    def healthcheck_namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        """
+        return pulumi.get(self, "healthcheck_namespace")
+
+    @healthcheck_namespace.setter
+    def healthcheck_namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "healthcheck_namespace", value)
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @remote_identity_group_id.setter
+    def remote_identity_group_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "remote_identity_group_id", value)
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @remote_identity_healthcheck_username.setter
+    def remote_identity_healthcheck_username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "remote_identity_healthcheck_username", value)
+
+    @property
+    @pulumi.getter(name="roleArn")
+    def role_arn(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "role_arn")
+
+    @role_arn.setter
+    def role_arn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "role_arn", value)
+
+    @property
+    @pulumi.getter(name="roleExternalId")
+    def role_external_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "role_external_id")
+
+    @role_external_id.setter
+    def role_external_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "role_external_id", value)
+
+    @property
+    @pulumi.getter(name="secretStoreCertificateAuthorityKey")
+    def secret_store_certificate_authority_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_certificate_authority_key")
+
+    @secret_store_certificate_authority_key.setter
+    def secret_store_certificate_authority_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_certificate_authority_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreCertificateAuthorityPath")
+    def secret_store_certificate_authority_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_certificate_authority_path")
+
+    @secret_store_certificate_authority_path.setter
+    def secret_store_certificate_authority_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_certificate_authority_path", value)
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @secret_store_id.setter
+    def secret_store_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_id", value)
+
+    @property
+    @pulumi.getter(name="secretStoreRoleArnKey")
+    def secret_store_role_arn_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_role_arn_key")
+
+    @secret_store_role_arn_key.setter
+    def secret_store_role_arn_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_role_arn_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreRoleArnPath")
+    def secret_store_role_arn_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_role_arn_path")
+
+    @secret_store_role_arn_path.setter
+    def secret_store_role_arn_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_role_arn_path", value)
+
+    @property
+    @pulumi.getter(name="secretStoreRoleExternalIdKey")
+    def secret_store_role_external_id_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_role_external_id_key")
+
+    @secret_store_role_external_id_key.setter
+    def secret_store_role_external_id_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_role_external_id_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreRoleExternalIdPath")
+    def secret_store_role_external_id_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_role_external_id_path")
+
+    @secret_store_role_external_id_path.setter
+    def secret_store_role_external_id_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_role_external_id_path", value)
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
+class ResourceAmazonEksInstanceProfileUserImpersonationArgs:
+    def __init__(__self__, *,
+                 cluster_name: pulumi.Input[str],
+                 endpoint: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 region: pulumi.Input[str],
+                 bind_interface: Optional[pulumi.Input[str]] = None,
+                 certificate_authority: Optional[pulumi.Input[str]] = None,
+                 egress_filter: Optional[pulumi.Input[str]] = None,
+                 healthcheck_namespace: Optional[pulumi.Input[str]] = None,
+                 remote_identity_group_id: Optional[pulumi.Input[str]] = None,
+                 remote_identity_healthcheck_username: Optional[pulumi.Input[str]] = None,
+                 role_arn: Optional[pulumi.Input[str]] = None,
+                 role_external_id: Optional[pulumi.Input[str]] = None,
+                 secret_store_certificate_authority_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_certificate_authority_path: Optional[pulumi.Input[str]] = None,
+                 secret_store_id: Optional[pulumi.Input[str]] = None,
+                 secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
+                 secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] bind_interface: Bind interface
+        :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "cluster_name", cluster_name)
+        pulumi.set(__self__, "endpoint", endpoint)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "region", region)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if certificate_authority is not None:
+            pulumi.set(__self__, "certificate_authority", certificate_authority)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if healthcheck_namespace is not None:
+            pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if role_arn is not None:
+            pulumi.set(__self__, "role_arn", role_arn)
+        if role_external_id is not None:
+            pulumi.set(__self__, "role_external_id", role_external_id)
+        if secret_store_certificate_authority_key is not None:
+            pulumi.set(__self__, "secret_store_certificate_authority_key", secret_store_certificate_authority_key)
+        if secret_store_certificate_authority_path is not None:
+            pulumi.set(__self__, "secret_store_certificate_authority_path", secret_store_certificate_authority_path)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if secret_store_role_arn_key is not None:
+            pulumi.set(__self__, "secret_store_role_arn_key", secret_store_role_arn_key)
+        if secret_store_role_arn_path is not None:
+            pulumi.set(__self__, "secret_store_role_arn_path", secret_store_role_arn_path)
+        if secret_store_role_external_id_key is not None:
+            pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
+        if secret_store_role_external_id_path is not None:
+            pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="clusterName")
+    def cluster_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "cluster_name")
+
+    @cluster_name.setter
+    def cluster_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cluster_name", value)
+
+    @property
+    @pulumi.getter
+    def endpoint(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "endpoint")
+
+    @endpoint.setter
+    def endpoint(self, value: pulumi.Input[str]):
+        pulumi.set(self, "endpoint", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def region(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "region")
+
+    @region.setter
+    def region(self, value: pulumi.Input[str]):
+        pulumi.set(self, "region", value)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[pulumi.Input[str]]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @bind_interface.setter
+    def bind_interface(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "bind_interface", value)
+
+    @property
+    @pulumi.getter(name="certificateAuthority")
+    def certificate_authority(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "certificate_authority")
+
+    @certificate_authority.setter
+    def certificate_authority(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "certificate_authority", value)
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @egress_filter.setter
+    def egress_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "egress_filter", value)
+
+    @property
+    @pulumi.getter(name="healthcheckNamespace")
+    def healthcheck_namespace(self) -> Optional[pulumi.Input[str]]:
+        """
+        The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        """
+        return pulumi.get(self, "healthcheck_namespace")
+
+    @healthcheck_namespace.setter
+    def healthcheck_namespace(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "healthcheck_namespace", value)
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @remote_identity_group_id.setter
+    def remote_identity_group_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "remote_identity_group_id", value)
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @remote_identity_healthcheck_username.setter
+    def remote_identity_healthcheck_username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "remote_identity_healthcheck_username", value)
+
+    @property
+    @pulumi.getter(name="roleArn")
+    def role_arn(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "role_arn")
+
+    @role_arn.setter
+    def role_arn(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "role_arn", value)
+
+    @property
+    @pulumi.getter(name="roleExternalId")
+    def role_external_id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "role_external_id")
+
+    @role_external_id.setter
+    def role_external_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "role_external_id", value)
+
+    @property
+    @pulumi.getter(name="secretStoreCertificateAuthorityKey")
+    def secret_store_certificate_authority_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_certificate_authority_key")
+
+    @secret_store_certificate_authority_key.setter
+    def secret_store_certificate_authority_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_certificate_authority_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreCertificateAuthorityPath")
+    def secret_store_certificate_authority_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_certificate_authority_path")
+
+    @secret_store_certificate_authority_path.setter
+    def secret_store_certificate_authority_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_certificate_authority_path", value)
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @secret_store_id.setter
+    def secret_store_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_id", value)
+
+    @property
+    @pulumi.getter(name="secretStoreRoleArnKey")
+    def secret_store_role_arn_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_role_arn_key")
+
+    @secret_store_role_arn_key.setter
+    def secret_store_role_arn_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_role_arn_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreRoleArnPath")
+    def secret_store_role_arn_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_role_arn_path")
+
+    @secret_store_role_arn_path.setter
+    def secret_store_role_arn_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_role_arn_path", value)
+
+    @property
+    @pulumi.getter(name="secretStoreRoleExternalIdKey")
+    def secret_store_role_external_id_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_role_external_id_key")
+
+    @secret_store_role_external_id_key.setter
+    def secret_store_role_external_id_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_role_external_id_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreRoleExternalIdPath")
+    def secret_store_role_external_id_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_role_external_id_path")
+
+    @secret_store_role_external_id_path.setter
+    def secret_store_role_external_id_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_role_external_id_path", value)
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -1871,21 +2681,23 @@
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
@@ -1922,14 +2734,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> pulumi.Input[str]:
         return pulumi.get(self, "cluster_name")
@@ -2149,14 +2963,26 @@
 
     @secret_store_secret_access_key_path.setter
     def secret_store_secret_access_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_secret_access_key_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -2182,20 +3008,22 @@
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -2226,14 +3054,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
@@ -2414,14 +3244,26 @@
 
     @secret_store_secret_access_key_path.setter
     def secret_store_secret_access_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_secret_access_key_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -2440,22 +3282,24 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -2472,14 +3316,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -2601,14 +3447,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -2652,20 +3510,22 @@
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "output", output)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -2696,14 +3556,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
         """
@@ -2884,14 +3746,26 @@
 
     @secret_store_secret_access_key_path.setter
     def secret_store_secret_access_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_secret_access_key_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -2911,21 +3785,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -2943,14 +3819,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -3079,14 +3957,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -3116,21 +4006,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -3150,14 +4042,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -3295,14 +4189,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -3579,14 +4485,15 @@
                  secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  session_expiry: Optional[pulumi.Input[int]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
@@ -3642,14 +4549,17 @@
     @region.setter
     def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter
     def subdomain(self) -> pulumi.Input[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @subdomain.setter
     def subdomain(self, value: pulumi.Input[str]):
         pulumi.set(self, "subdomain", value)
 
     @property
@@ -3824,14 +4734,15 @@
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_path: Optional[pulumi.Input[str]] = None,
                  session_expiry: Optional[pulumi.Input[int]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
@@ -3897,14 +4808,17 @@
     @region.setter
     def region(self, value: pulumi.Input[str]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter
     def subdomain(self) -> pulumi.Input[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @subdomain.setter
     def subdomain(self, value: pulumi.Input[str]):
         pulumi.set(self, "subdomain", value)
 
     @property
@@ -4118,15 +5032,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
-        :param pulumi.Input[str] secret_store_tenant_id_key: * azure_postgres:
+        :param pulumi.Input[str] secret_store_tenant_id_key: * azure_mysql:
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4255,15 +5169,15 @@
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter(name="secretStoreTenantIdKey")
     def secret_store_tenant_id_key(self) -> Optional[pulumi.Input[str]]:
         """
-        * azure_postgres:
+        * azure_mysql:
         """
         return pulumi.get(self, "secret_store_tenant_id_key")
 
     @secret_store_tenant_id_key.setter
     def secret_store_tenant_id_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_tenant_id_key", value)
 
@@ -4316,15 +5230,15 @@
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
-        :param pulumi.Input[str] secret_store_tenant_id_key: * azure_postgres:
+        :param pulumi.Input[str] secret_store_tenant_id_key: * azure_mysql:
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4453,15 +5367,15 @@
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter(name="secretStoreTenantIdKey")
     def secret_store_tenant_id_key(self) -> Optional[pulumi.Input[str]]:
         """
-        * azure_postgres:
+        * azure_mysql:
         """
         return pulumi.get(self, "secret_store_tenant_id_key")
 
     @secret_store_tenant_id_key.setter
     def secret_store_tenant_id_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_tenant_id_key", value)
 
@@ -4493,14 +5407,234 @@
 
     @tenant_id.setter
     def tenant_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tenant_id", value)
 
 
 @pulumi.input_type
+class ResourceAzureMysqlArgs:
+    def __init__(__self__, *,
+                 database: pulumi.Input[str],
+                 hostname: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 bind_interface: Optional[pulumi.Input[str]] = None,
+                 egress_filter: Optional[pulumi.Input[str]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 port: Optional[pulumi.Input[int]] = None,
+                 port_override: Optional[pulumi.Input[int]] = None,
+                 secret_store_id: Optional[pulumi.Input[str]] = None,
+                 secret_store_password_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_password_path: Optional[pulumi.Input[str]] = None,
+                 secret_store_username_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] bind_interface: Bind interface
+        :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "database", database)
+        pulumi.set(__self__, "hostname", hostname)
+        pulumi.set(__self__, "name", name)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if secret_store_password_key is not None:
+            pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
+        if secret_store_password_path is not None:
+            pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if secret_store_username_key is not None:
+            pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
+        if secret_store_username_path is not None:
+            pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def database(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "database")
+
+    @database.setter
+    def database(self, value: pulumi.Input[str]):
+        pulumi.set(self, "database", value)
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "hostname")
+
+    @hostname.setter
+    def hostname(self, value: pulumi.Input[str]):
+        pulumi.set(self, "hostname", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[pulumi.Input[str]]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @bind_interface.setter
+    def bind_interface(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "bind_interface", value)
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[pulumi.Input[str]]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @egress_filter.setter
+    def egress_filter(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "egress_filter", value)
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port", value)
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port_override")
+
+    @port_override.setter
+    def port_override(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port_override", value)
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @secret_store_id.setter
+    def secret_store_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_id", value)
+
+    @property
+    @pulumi.getter(name="secretStorePasswordKey")
+    def secret_store_password_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_password_key")
+
+    @secret_store_password_key.setter
+    def secret_store_password_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_password_key", value)
+
+    @property
+    @pulumi.getter(name="secretStorePasswordPath")
+    def secret_store_password_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_password_path")
+
+    @secret_store_password_path.setter
+    def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_password_path", value)
+
+    @property
+    @pulumi.getter(name="secretStoreUsernameKey")
+    def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_username_key")
+
+    @secret_store_username_key.setter
+    def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_username_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreUsernamePath")
+    def secret_store_username_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_username_path")
+
+    @secret_store_username_path.setter
+    def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_username_path", value)
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
+
+
+@pulumi.input_type
 class ResourceAzurePostgresArgs:
     def __init__(__self__, *,
                  database: pulumi.Input[str],
                  hostname: pulumi.Input[str],
                  name: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
@@ -4509,21 +5643,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4543,14 +5679,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -4688,14 +5826,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -4721,21 +5871,23 @@
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  private_key: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_private_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_private_key_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project", project)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4747,14 +5899,16 @@
             pulumi.set(__self__, "private_key", private_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_private_key_key is not None:
             pulumi.set(__self__, "secret_store_private_key_key", secret_store_private_key_key)
         if secret_store_private_key_path is not None:
             pulumi.set(__self__, "secret_store_private_key_path", secret_store_private_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -4856,14 +6010,26 @@
 
     @secret_store_private_key_path.setter
     def secret_store_private_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_private_key_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -4891,22 +6057,24 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -4923,14 +6091,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -5052,14 +6222,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -5098,21 +6280,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5132,14 +6316,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -5277,14 +6463,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -5313,21 +6511,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5345,14 +6545,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -5481,14 +6683,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -5518,21 +6732,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5552,14 +6768,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -5697,14 +6915,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -5732,22 +6962,24 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5763,14 +6995,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -5892,14 +7126,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -5937,21 +7183,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5969,14 +7217,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -6105,14 +7355,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -6141,21 +7403,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -6173,14 +7437,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
@@ -6309,14 +7575,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -6346,21 +7624,23 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
@@ -6379,14 +7659,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
@@ -6524,14 +7806,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -6559,21 +7853,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -6590,14 +7886,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -6717,14 +8015,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -6759,20 +8069,22 @@
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
@@ -6802,14 +8114,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> pulumi.Input[str]:
         return pulumi.get(self, "endpoint")
@@ -6990,14 +8304,26 @@
 
     @secret_store_secret_access_key_path.setter
     def secret_store_secret_access_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_secret_access_key_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -7016,22 +8342,24 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -7048,14 +8376,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -7177,14 +8507,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -7219,21 +8561,26 @@
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
+                 secret_store_username_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 tls_required: Optional[pulumi.Input[bool]] = None):
+                 tls_required: Optional[pulumi.Input[bool]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -7246,18 +8593,26 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if secret_store_username_key is not None:
+            pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
+        if secret_store_username_path is not None:
+            pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Input[str]:
         return pulumi.get(self, "hostname")
 
     @hostname.setter
@@ -7354,14 +8709,44 @@
         return pulumi.get(self, "secret_store_password_path")
 
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
+    @pulumi.getter(name="secretStoreUsernameKey")
+    def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_username_key")
+
+    @secret_store_username_key.setter
+    def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_username_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreUsernamePath")
+    def secret_store_username_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_username_path")
+
+    @secret_store_username_path.setter
+    def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_username_path", value)
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
@@ -7374,14 +8759,23 @@
     def tls_required(self) -> Optional[pulumi.Input[bool]]:
         return pulumi.get(self, "tls_required")
 
     @tls_required.setter
     def tls_required(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "tls_required", value)
 
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
+
 
 @pulumi.input_type
 class ResourceGcpArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  scopes: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
@@ -7525,21 +8919,23 @@
                  remote_identity_healthcheck_username: Optional[pulumi.Input[str]] = None,
                  secret_store_certificate_authority_key: Optional[pulumi.Input[str]] = None,
                  secret_store_certificate_authority_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_service_account_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_service_account_key_path: Optional[pulumi.Input[str]] = None,
                  service_account_key: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -7560,14 +8956,16 @@
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_service_account_key_key is not None:
             pulumi.set(__self__, "secret_store_service_account_key_key", secret_store_service_account_key_key)
         if secret_store_service_account_key_path is not None:
             pulumi.set(__self__, "secret_store_service_account_key_path", secret_store_service_account_key_path)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> pulumi.Input[str]:
         return pulumi.get(self, "endpoint")
@@ -7706,14 +9104,26 @@
 
     @service_account_key.setter
     def service_account_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_account_key", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -7732,21 +9142,23 @@
                  healthcheck_namespace: Optional[pulumi.Input[str]] = None,
                  secret_store_certificate_authority_key: Optional[pulumi.Input[str]] = None,
                  secret_store_certificate_authority_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_service_account_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_service_account_key_path: Optional[pulumi.Input[str]] = None,
                  service_account_key: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -7763,14 +9175,16 @@
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_service_account_key_key is not None:
             pulumi.set(__self__, "secret_store_service_account_key_key", secret_store_service_account_key_key)
         if secret_store_service_account_key_path is not None:
             pulumi.set(__self__, "secret_store_service_account_key_path", secret_store_service_account_key_path)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> pulumi.Input[str]:
         return pulumi.get(self, "endpoint")
@@ -7891,14 +9305,26 @@
 
     @service_account_key.setter
     def service_account_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_account_key", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -7919,21 +9345,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -7953,14 +9381,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -8098,14 +9528,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -8137,14 +9579,15 @@
                  host_override: Optional[pulumi.Input[str]] = None,
                  secret_store_auth_header_key: Optional[pulumi.Input[str]] = None,
                  secret_store_auth_header_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[str] url: * kubernetes:
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
@@ -8192,14 +9635,17 @@
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def subdomain(self) -> pulumi.Input[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @subdomain.setter
     def subdomain(self, value: pulumi.Input[str]):
         pulumi.set(self, "subdomain", value)
 
     @property
@@ -8335,14 +9781,15 @@
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[str] url: * kubernetes:
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
@@ -8396,14 +9843,17 @@
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def subdomain(self) -> pulumi.Input[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @subdomain.setter
     def subdomain(self, value: pulumi.Input[str]):
         pulumi.set(self, "subdomain", value)
 
     @property
@@ -8560,14 +10010,15 @@
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  headers_blacklist: Optional[pulumi.Input[str]] = None,
                  host_override: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[str] url: * kubernetes:
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
@@ -8609,14 +10060,17 @@
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def subdomain(self) -> pulumi.Input[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @subdomain.setter
     def subdomain(self, value: pulumi.Input[str]):
         pulumi.set(self, "subdomain", value)
 
     @property
@@ -8725,21 +10179,23 @@
                  secret_store_certificate_authority_key: Optional[pulumi.Input[str]] = None,
                  secret_store_certificate_authority_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_key_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8769,14 +10225,16 @@
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_client_key_key is not None:
             pulumi.set(__self__, "secret_store_client_key_key", secret_store_client_key_key)
         if secret_store_client_key_path is not None:
             pulumi.set(__self__, "secret_store_client_key_path", secret_store_client_key_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Input[str]:
         return pulumi.get(self, "hostname")
@@ -8960,14 +10418,26 @@
 
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -8987,22 +10457,24 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9020,14 +10492,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -9159,14 +10633,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -9194,23 +10680,25 @@
                  healthcheck_namespace: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  remote_identity_group_id: Optional[pulumi.Input[str]] = None,
                  remote_identity_healthcheck_username: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_token_key: Optional[pulumi.Input[str]] = None,
                  secret_store_token_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] secret_store_token_key: * kubernetes_user_impersonation:
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9226,14 +10714,16 @@
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_token_key is not None:
             pulumi.set(__self__, "secret_store_token_key", secret_store_token_key)
         if secret_store_token_path is not None:
             pulumi.set(__self__, "secret_store_token_path", secret_store_token_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -9359,14 +10849,26 @@
 
     @secret_store_token_path.setter
     def secret_store_token_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_token_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -9392,23 +10894,25 @@
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  healthcheck_namespace: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_token_key: Optional[pulumi.Input[str]] = None,
                  secret_store_token_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  token: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[str] secret_store_token_key: * kubernetes_user_impersonation:
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9420,14 +10924,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_token_key is not None:
             pulumi.set(__self__, "secret_store_token_key", secret_store_token_key)
         if secret_store_token_path is not None:
             pulumi.set(__self__, "secret_store_token_path", secret_store_token_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -9535,14 +11041,26 @@
 
     @secret_store_token_path.setter
     def secret_store_token_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_token_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -9575,21 +11093,23 @@
                  secret_store_certificate_authority_key: Optional[pulumi.Input[str]] = None,
                  secret_store_certificate_authority_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_certificate_path: Optional[pulumi.Input[str]] = None,
                  secret_store_client_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_client_key_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9615,14 +11135,16 @@
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_client_key_key is not None:
             pulumi.set(__self__, "secret_store_client_key_key", secret_store_client_key_key)
         if secret_store_client_key_path is not None:
             pulumi.set(__self__, "secret_store_client_key_path", secret_store_client_key_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Input[str]:
         return pulumi.get(self, "hostname")
@@ -9788,14 +11310,26 @@
 
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -9815,21 +11349,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9847,14 +11383,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -9983,14 +11521,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -10013,34 +11563,38 @@
                  hostname: pulumi.Input[str],
                  name: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Input[str]:
         return pulumi.get(self, "hostname")
@@ -10113,14 +11667,26 @@
 
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -10140,21 +11706,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -10172,14 +11740,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -10308,14 +11878,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -10344,22 +11926,24 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -10377,14 +11961,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -10515,14 +12101,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -10561,22 +12159,24 @@
                  port_override: Optional[pulumi.Input[int]] = None,
                  replica_set: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -10596,14 +12196,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -10743,14 +12345,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -10790,22 +12404,24 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
@@ -10826,14 +12442,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -10982,14 +12600,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -11029,22 +12659,24 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
@@ -11065,14 +12697,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -11221,14 +12855,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -11265,22 +12911,24 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -11296,14 +12944,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -11425,14 +13075,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -11480,21 +13142,23 @@
                  secret_store_client_key_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
                  server_name: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -11532,14 +13196,16 @@
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
         if server_name is not None:
             pulumi.set(__self__, "server_name", server_name)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -11758,14 +13424,26 @@
 
     @server_name.setter
     def server_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server_name", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -11805,21 +13483,23 @@
                  secret_store_client_key_path: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
                  server_name: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -11859,14 +13539,16 @@
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
         if server_name is not None:
             pulumi.set(__self__, "server_name", server_name)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -12094,14 +13776,26 @@
 
     @server_name.setter
     def server_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "server_name", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -12130,21 +13824,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -12162,14 +13858,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -12298,14 +13996,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -12328,34 +14038,38 @@
                  endpoint: pulumi.Input[str],
                  name: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> pulumi.Input[str]:
         return pulumi.get(self, "endpoint")
@@ -12428,14 +14142,26 @@
 
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -12462,20 +14188,22 @@
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_arn_path: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_key: Optional[pulumi.Input[str]] = None,
                  secret_store_role_external_id_path: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_secret_access_key_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
@@ -12507,14 +14235,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> pulumi.Input[str]:
         return pulumi.get(self, "endpoint")
@@ -12704,14 +14434,26 @@
 
     @secret_store_secret_access_key_path.setter
     def secret_store_secret_access_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_secret_access_key_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -12731,22 +14473,24 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
@@ -12763,14 +14507,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -12901,14 +14647,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -12947,21 +14705,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -12981,14 +14741,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -13126,14 +14888,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -13160,22 +14934,24 @@
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -13189,14 +14965,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -13309,14 +15087,26 @@
 
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -13353,22 +15143,24 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  tls_required: Optional[pulumi.Input[bool]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -13385,14 +15177,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -13514,14 +15308,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -13553,34 +15359,38 @@
                  hostname: pulumi.Input[str],
                  name: pulumi.Input[str],
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Input[str]:
         return pulumi.get(self, "hostname")
@@ -13653,14 +15463,26 @@
 
     @secret_store_id.setter
     def secret_store_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_id", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -13669,57 +15491,62 @@
 
 
 @pulumi.input_type
 class ResourceRdpArgs:
     def __init__(__self__, *,
                  hostname: pulumi.Input[str],
                  name: pulumi.Input[str],
-                 port: pulumi.Input[int],
                  bind_interface: Optional[pulumi.Input[str]] = None,
                  downgrade_nla_connections: Optional[pulumi.Input[bool]] = None,
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
+                 port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if downgrade_nla_connections is not None:
             pulumi.set(__self__, "downgrade_nla_connections", downgrade_nla_connections)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -13739,23 +15566,14 @@
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
-    @pulumi.getter
-    def port(self) -> pulumi.Input[int]:
-        return pulumi.get(self, "port")
-
-    @port.setter
-    def port(self, value: pulumi.Input[int]):
-        pulumi.set(self, "port", value)
-
-    @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[pulumi.Input[str]]:
         """
         Bind interface
         """
         return pulumi.get(self, "bind_interface")
 
@@ -13790,14 +15608,23 @@
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
+    @pulumi.getter
+    def port(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "port", value)
+
+    @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[pulumi.Input[int]]:
         return pulumi.get(self, "port_override")
 
     @port_override.setter
     def port_override(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "port_override", value)
@@ -13848,14 +15675,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -13881,20 +15720,26 @@
                  egress_filter: Optional[pulumi.Input[str]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
-                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+                 secret_store_username_key: Optional[pulumi.Input[str]] = None,
+                 secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
+                 tls_required: Optional[pulumi.Input[bool]] = None,
+                 username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -13907,16 +15752,26 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if secret_store_username_key is not None:
+            pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
+        if secret_store_username_path is not None:
+            pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if tls_required is not None:
+            pulumi.set(__self__, "tls_required", tls_required)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> pulumi.Input[str]:
         return pulumi.get(self, "hostname")
 
     @hostname.setter
@@ -14013,25 +15868,73 @@
         return pulumi.get(self, "secret_store_password_path")
 
     @secret_store_password_path.setter
     def secret_store_password_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_password_path", value)
 
     @property
+    @pulumi.getter(name="secretStoreUsernameKey")
+    def secret_store_username_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_username_key")
+
+    @secret_store_username_key.setter
+    def secret_store_username_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_username_key", value)
+
+    @property
+    @pulumi.getter(name="secretStoreUsernamePath")
+    def secret_store_username_path(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "secret_store_username_path")
+
+    @secret_store_username_path.setter
+    def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "secret_store_username_path", value)
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
+    @property
+    @pulumi.getter(name="tlsRequired")
+    def tls_required(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "tls_required")
+
+    @tls_required.setter
+    def tls_required(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "tls_required", value)
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "username")
+
+    @username.setter
+    def username(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "username", value)
+
 
 @pulumi.input_type
 class ResourceRedshiftArgs:
     def __init__(__self__, *,
                  database: pulumi.Input[str],
                  hostname: pulumi.Input[str],
                  name: pulumi.Input[str],
@@ -14042,21 +15945,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -14076,14 +15981,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -14221,14 +16128,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -14257,21 +16176,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -14289,14 +16210,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -14425,14 +16348,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -14461,21 +16396,23 @@
                  port_override: Optional[pulumi.Input[int]] = None,
                  schema: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -14493,14 +16430,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -14629,14 +16568,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -14665,14 +16616,15 @@
                  saml_metadata: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_saml_metadata_key: Optional[pulumi.Input[str]] = None,
                  secret_store_saml_metadata_path: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_username", healthcheck_username)
         pulumi.set(__self__, "name", name)
@@ -14714,14 +16666,17 @@
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def subdomain(self) -> pulumi.Input[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @subdomain.setter
     def subdomain(self, value: pulumi.Input[str]):
         pulumi.set(self, "subdomain", value)
 
     @property
@@ -14823,21 +16778,23 @@
                  port_override: Optional[pulumi.Input[int]] = None,
                  schema: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -14859,14 +16816,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -15013,14 +16972,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -15049,21 +17020,23 @@
                  key_type: Optional[pulumi.Input[str]] = None,
                  port_forwarding: Optional[pulumi.Input[bool]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
@@ -15081,14 +17054,16 @@
             pulumi.set(__self__, "public_key", public_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -15217,14 +17192,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -15254,21 +17241,23 @@
                  port_forwarding: Optional[pulumi.Input[bool]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  remote_identity_group_id: Optional[pulumi.Input[str]] = None,
                  remote_identity_healthcheck_username: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
@@ -15288,14 +17277,16 @@
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -15433,14 +17424,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -15470,21 +17473,23 @@
                  port_override: Optional[pulumi.Input[int]] = None,
                  private_key: Optional[pulumi.Input[str]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_private_key_key: Optional[pulumi.Input[str]] = None,
                  secret_store_private_key_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
@@ -15504,14 +17509,16 @@
             pulumi.set(__self__, "secret_store_private_key_key", secret_store_private_key_key)
         if secret_store_private_key_path is not None:
             pulumi.set(__self__, "secret_store_private_key_path", secret_store_private_key_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -15649,14 +17656,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -15684,21 +17703,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -15715,14 +17736,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -15842,14 +17865,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -15877,21 +17912,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -15908,14 +17945,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -16035,14 +18074,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -16070,21 +18121,23 @@
                  port: Optional[pulumi.Input[int]] = None,
                  port_override: Optional[pulumi.Input[int]] = None,
                  secret_store_id: Optional[pulumi.Input[str]] = None,
                  secret_store_password_key: Optional[pulumi.Input[str]] = None,
                  secret_store_password_path: Optional[pulumi.Input[str]] = None,
                  secret_store_username_key: Optional[pulumi.Input[str]] = None,
                  secret_store_username_path: Optional[pulumi.Input[str]] = None,
+                 subdomain: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  username: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the Resource.
         :param pulumi.Input[str] bind_interface: Bind interface
         :param pulumi.Input[str] egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param pulumi.Input[str] secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param pulumi.Input[str] subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -16101,14 +18154,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -16228,14 +18283,26 @@
 
     @secret_store_username_path.setter
     def secret_store_username_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_store_username_path", value)
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[pulumi.Input[str]]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @subdomain.setter
+    def subdomain(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "subdomain", value)
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
@@ -16359,14 +18426,63 @@
     def __init__(__self__, *,
                  app_url: pulumi.Input[str],
                  name: pulumi.Input[str],
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "app_url", app_url)
+        pulumi.set(__self__, "name", name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="appUrl")
+    def app_url(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "app_url")
+
+    @app_url.setter
+    def app_url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "app_url", value)
+
+    @property
+    @pulumi.getter
+    def name(self) -> pulumi.Input[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
+
+@pulumi.input_type
+class SecretStoreCyberarkPamArgs:
+    def __init__(__self__, *,
+                 app_url: pulumi.Input[str],
+                 name: pulumi.Input[str],
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
+        """
+        :param pulumi.Input[str] name: Unique human-readable name of the SecretStore.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "app_url", app_url)
         pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/_utilities.py` & `pulumi_sdm-0.4.0/pulumi_sdm/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/account.py` & `pulumi_sdm-0.4.0/pulumi_sdm/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/account_attachment.py` & `pulumi_sdm-0.4.0/pulumi_sdm/account_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/config/vars.py` & `pulumi_sdm-0.4.0/pulumi_sdm/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_account.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_account.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,21 +18,24 @@
 ]
 
 @pulumi.output_type
 class GetAccountResult:
     """
     A collection of values returned by getAccount.
     """
-    def __init__(__self__, accounts=None, email=None, first_name=None, id=None, ids=None, last_name=None, name=None, suspended=None, tags=None, type=None):
+    def __init__(__self__, accounts=None, email=None, external_id=None, first_name=None, id=None, ids=None, last_name=None, name=None, suspended=None, tags=None, type=None):
         if accounts and not isinstance(accounts, list):
             raise TypeError("Expected argument 'accounts' to be a list")
         pulumi.set(__self__, "accounts", accounts)
         if email and not isinstance(email, str):
             raise TypeError("Expected argument 'email' to be a str")
         pulumi.set(__self__, "email", email)
+        if external_id and not isinstance(external_id, str):
+            raise TypeError("Expected argument 'external_id' to be a str")
+        pulumi.set(__self__, "external_id", external_id)
         if first_name and not isinstance(first_name, str):
             raise TypeError("Expected argument 'first_name' to be a str")
         pulumi.set(__self__, "first_name", first_name)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if ids and not isinstance(ids, list):
@@ -68,14 +71,22 @@
     def email(self) -> Optional[str]:
         """
         The User's email address. Must be unique.
         """
         return pulumi.get(self, "email")
 
     @property
+    @pulumi.getter(name="externalId")
+    def external_id(self) -> Optional[str]:
+        """
+        External ID is an alternative unique ID this user is represented by within an external service.
+        """
+        return pulumi.get(self, "external_id")
+
+    @property
     @pulumi.getter(name="firstName")
     def first_name(self) -> Optional[str]:
         """
         The User's first name.
         """
         return pulumi.get(self, "first_name")
 
@@ -137,25 +148,27 @@
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetAccountResult(
             accounts=self.accounts,
             email=self.email,
+            external_id=self.external_id,
             first_name=self.first_name,
             id=self.id,
             ids=self.ids,
             last_name=self.last_name,
             name=self.name,
             suspended=self.suspended,
             tags=self.tags,
             type=self.type)
 
 
 def get_account(email: Optional[str] = None,
+                external_id: Optional[str] = None,
                 first_name: Optional[str] = None,
                 id: Optional[str] = None,
                 last_name: Optional[str] = None,
                 name: Optional[str] = None,
                 suspended: Optional[bool] = None,
                 tags: Optional[Mapping[str, Any]] = None,
                 type: Optional[str] = None,
@@ -176,49 +189,53 @@
             "region": "us-west",
         },
         type="user")
     ```
 
 
     :param str email: The User's email address. Must be unique.
+    :param str external_id: External ID is an alternative unique ID this user is represented by within an external service.
     :param str first_name: The User's first name.
     :param str id: Unique identifier of the User.
     :param str last_name: The User's last name.
     :param str name: Unique human-readable name of the Service.
     :param bool suspended: The User's suspended state.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
     :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
     """
     __args__ = dict()
     __args__['email'] = email
+    __args__['externalId'] = external_id
     __args__['firstName'] = first_name
     __args__['id'] = id
     __args__['lastName'] = last_name
     __args__['name'] = name
     __args__['suspended'] = suspended
     __args__['tags'] = tags
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getAccount:getAccount', __args__, opts=opts, typ=GetAccountResult).value
 
     return AwaitableGetAccountResult(
         accounts=__ret__.accounts,
         email=__ret__.email,
+        external_id=__ret__.external_id,
         first_name=__ret__.first_name,
         id=__ret__.id,
         ids=__ret__.ids,
         last_name=__ret__.last_name,
         name=__ret__.name,
         suspended=__ret__.suspended,
         tags=__ret__.tags,
         type=__ret__.type)
 
 
 @_utilities.lift_output_func(get_account)
 def get_account_output(email: Optional[pulumi.Input[Optional[str]]] = None,
+                       external_id: Optional[pulumi.Input[Optional[str]]] = None,
                        first_name: Optional[pulumi.Input[Optional[str]]] = None,
                        id: Optional[pulumi.Input[Optional[str]]] = None,
                        last_name: Optional[pulumi.Input[Optional[str]]] = None,
                        name: Optional[pulumi.Input[Optional[str]]] = None,
                        suspended: Optional[pulumi.Input[Optional[bool]]] = None,
                        tags: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                        type: Optional[pulumi.Input[Optional[str]]] = None,
@@ -239,14 +256,15 @@
             "region": "us-west",
         },
         type="user")
     ```
 
 
     :param str email: The User's email address. Must be unique.
+    :param str external_id: External ID is an alternative unique ID this user is represented by within an external service.
     :param str first_name: The User's first name.
     :param str id: Unique identifier of the User.
     :param str last_name: The User's last name.
     :param str name: Unique human-readable name of the Service.
     :param bool suspended: The User's suspended state.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
     :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_account_attachment.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_account_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_node.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_remote_identity.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_remote_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_remote_identity_group.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_remote_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_resource.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_role.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_role.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,21 +18,24 @@
 ]
 
 @pulumi.output_type
 class GetRoleResult:
     """
     A collection of values returned by getRole.
     """
-    def __init__(__self__, id=None, ids=None, name=None, roles=None, tags=None):
+    def __init__(__self__, id=None, ids=None, managed_by=None, name=None, roles=None, tags=None):
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if ids and not isinstance(ids, list):
             raise TypeError("Expected argument 'ids' to be a list")
         pulumi.set(__self__, "ids", ids)
+        if managed_by and not isinstance(managed_by, str):
+            raise TypeError("Expected argument 'managed_by' to be a str")
+        pulumi.set(__self__, "managed_by", managed_by)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if roles and not isinstance(roles, list):
             raise TypeError("Expected argument 'roles' to be a list")
         pulumi.set(__self__, "roles", roles)
         if tags and not isinstance(tags, dict):
@@ -52,14 +55,22 @@
     def ids(self) -> Sequence[str]:
         """
         a list of strings of ids of data sources that match the given arguments.
         """
         return pulumi.get(self, "ids")
 
     @property
+    @pulumi.getter(name="managedBy")
+    def managed_by(self) -> str:
+        """
+        Managed By is a read only field for what service manages this role, e.g. StrongDM, Okta, Azure.
+        """
+        return pulumi.get(self, "managed_by")
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Role.
         """
         return pulumi.get(self, "name")
 
@@ -84,14 +95,15 @@
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetRoleResult(
             id=self.id,
             ids=self.ids,
+            managed_by=self.managed_by,
             name=self.name,
             roles=self.roles,
             tags=self.tags)
 
 
 def get_role(id: Optional[str] = None,
              name: Optional[str] = None,
@@ -113,14 +125,15 @@
     __args__['tags'] = tags
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('sdm:index/getRole:getRole', __args__, opts=opts, typ=GetRoleResult).value
 
     return AwaitableGetRoleResult(
         id=__ret__.id,
         ids=__ret__.ids,
+        managed_by=__ret__.managed_by,
         name=__ret__.name,
         roles=__ret__.roles,
         tags=__ret__.tags)
 
 
 @_utilities.lift_output_func(get_role)
 def get_role_output(id: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_secret_store.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_secret_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 def get_secret_store(id: Optional[str] = None,
                      name: Optional[str] = None,
                      tags: Optional[Mapping[str, Any]] = None,
                      type: Optional[str] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetSecretStoreResult:
     """
     A SecretStore is a server where resource secrets (passwords, keys) are stored.
-     Coming soon support for HashiCorp Vault and AWS Secret Store. Contact support@strongdm.com to request access to the beta.
+     Coming soon support for HashiCorp Vault and AWS Secret Store.
 
 
     :param str id: Unique identifier of the SecretStore.
     :param str name: Unique human-readable name of the SecretStore.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
     :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
     """
@@ -139,15 +139,15 @@
 def get_secret_store_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                             name: Optional[pulumi.Input[Optional[str]]] = None,
                             tags: Optional[pulumi.Input[Optional[Mapping[str, Any]]]] = None,
                             type: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSecretStoreResult]:
     """
     A SecretStore is a server where resource secrets (passwords, keys) are stored.
-     Coming soon support for HashiCorp Vault and AWS Secret Store. Contact support@strongdm.com to request access to the beta.
+     Coming soon support for HashiCorp Vault and AWS Secret Store.
 
 
     :param str id: Unique identifier of the SecretStore.
     :param str name: Unique human-readable name of the SecretStore.
     :param Mapping[str, Any] tags: Tags is a map of key, value pairs.
     :param str type: a filter to select all items of a certain subtype. See the [filter documentation](https://www.strongdm.com/docs/automation/getting-started/filters for more information.
     """
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/get_ssh_ca_pubkey.py` & `pulumi_sdm-0.4.0/pulumi_sdm/get_ssh_ca_pubkey.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/node.py` & `pulumi_sdm-0.4.0/pulumi_sdm/node.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/outputs.py` & `pulumi_sdm-0.4.0/pulumi_sdm/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,28 @@
     'NodeRelay',
     'ResourceAks',
     'ResourceAksBasicAuth',
     'ResourceAksServiceAccount',
     'ResourceAksServiceAccountUserImpersonation',
     'ResourceAksUserImpersonation',
     'ResourceAmazonEks',
+    'ResourceAmazonEksInstanceProfile',
+    'ResourceAmazonEksInstanceProfileUserImpersonation',
     'ResourceAmazonEksUserImpersonation',
     'ResourceAmazonEs',
     'ResourceAmazonmqAmqp091',
     'ResourceAthena',
     'ResourceAuroraMysql',
     'ResourceAuroraPostgres',
     'ResourceAws',
     'ResourceAwsConsole',
     'ResourceAwsConsoleStaticKeyPair',
     'ResourceAzure',
     'ResourceAzureCertificate',
+    'ResourceAzureMysql',
     'ResourceAzurePostgres',
     'ResourceBigQuery',
     'ResourceCassandra',
     'ResourceCitus',
     'ResourceClustrix',
     'ResourceCockroach',
     'ResourceDb2I',
@@ -88,14 +91,15 @@
     'ResourceSshCustomerKey',
     'ResourceSybase',
     'ResourceSybaseIq',
     'ResourceTeradata',
     'SecretStoreAws',
     'SecretStoreAzureStore',
     'SecretStoreCyberarkConjur',
+    'SecretStoreCyberarkPam',
     'SecretStoreCyberarkPamExperimental',
     'SecretStoreDelineaStore',
     'SecretStoreGcpStore',
     'SecretStoreVaultApprole',
     'SecretStoreVaultTls',
     'SecretStoreVaultToken',
     'GetAccountAccountResult',
@@ -111,24 +115,27 @@
     'GetResourceResourceAkResult',
     'GetResourceResourceAksBasicAuthResult',
     'GetResourceResourceAksServiceAccountResult',
     'GetResourceResourceAksServiceAccountUserImpersonationResult',
     'GetResourceResourceAksUserImpersonationResult',
     'GetResourceResourceAmazonEResult',
     'GetResourceResourceAmazonEkResult',
+    'GetResourceResourceAmazonEksInstanceProfileResult',
+    'GetResourceResourceAmazonEksInstanceProfileUserImpersonationResult',
     'GetResourceResourceAmazonEksUserImpersonationResult',
     'GetResourceResourceAmazonmqAmqp091Result',
     'GetResourceResourceAthenaResult',
     'GetResourceResourceAuroraMysqlResult',
     'GetResourceResourceAuroraPostgreResult',
     'GetResourceResourceAwResult',
     'GetResourceResourceAwsConsoleResult',
     'GetResourceResourceAwsConsoleStaticKeyPairResult',
     'GetResourceResourceAzureResult',
     'GetResourceResourceAzureCertificateResult',
+    'GetResourceResourceAzureMysqlResult',
     'GetResourceResourceAzurePostgreResult',
     'GetResourceResourceBigQueryResult',
     'GetResourceResourceCassandraResult',
     'GetResourceResourceCitusResult',
     'GetResourceResourceClustrixResult',
     'GetResourceResourceCockroachResult',
     'GetResourceResourceDb2IResult',
@@ -183,14 +190,15 @@
     'GetResourceResourceSybaseIqResult',
     'GetResourceResourceTeradataResult',
     'GetRoleRoleResult',
     'GetSecretStoreSecretStoreResult',
     'GetSecretStoreSecretStoreAwResult',
     'GetSecretStoreSecretStoreAzureStoreResult',
     'GetSecretStoreSecretStoreCyberarkConjurResult',
+    'GetSecretStoreSecretStoreCyberarkPamResult',
     'GetSecretStoreSecretStoreCyberarkPamExperimentalResult',
     'GetSecretStoreSecretStoreDelineaStoreResult',
     'GetSecretStoreSecretStoreGcpStoreResult',
     'GetSecretStoreSecretStoreVaultApproleResult',
     'GetSecretStoreSecretStoreVaultTlResult',
     'GetSecretStoreSecretStoreVaultTokenResult',
 ]
@@ -250,14 +258,20 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "firstName":
             suggest = "first_name"
         elif key == "lastName":
             suggest = "last_name"
+        elif key == "externalId":
+            suggest = "external_id"
+        elif key == "managedBy":
+            suggest = "managed_by"
+        elif key == "permissionLevel":
+            suggest = "permission_level"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in AccountUser. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         AccountUser.__key_warning(key)
         return super().__getitem__(key)
@@ -266,26 +280,38 @@
         AccountUser.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  email: str,
                  first_name: str,
                  last_name: str,
+                 external_id: Optional[str] = None,
+                 managed_by: Optional[str] = None,
+                 permission_level: Optional[str] = None,
                  suspended: Optional[bool] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str email: The User's email address. Must be unique.
         :param str first_name: The User's first name.
         :param str last_name: The User's last name.
+        :param str external_id: External ID is an alternative unique ID this user is represented by within an external service.
+        :param str managed_by: Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
+        :param str permission_level: PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
         :param bool suspended: The User's suspended state.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "email", email)
         pulumi.set(__self__, "first_name", first_name)
         pulumi.set(__self__, "last_name", last_name)
+        if external_id is not None:
+            pulumi.set(__self__, "external_id", external_id)
+        if managed_by is not None:
+            pulumi.set(__self__, "managed_by", managed_by)
+        if permission_level is not None:
+            pulumi.set(__self__, "permission_level", permission_level)
         if suspended is not None:
             pulumi.set(__self__, "suspended", suspended)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
@@ -308,14 +334,38 @@
     def last_name(self) -> str:
         """
         The User's last name.
         """
         return pulumi.get(self, "last_name")
 
     @property
+    @pulumi.getter(name="externalId")
+    def external_id(self) -> Optional[str]:
+        """
+        External ID is an alternative unique ID this user is represented by within an external service.
+        """
+        return pulumi.get(self, "external_id")
+
+    @property
+    @pulumi.getter(name="managedBy")
+    def managed_by(self) -> Optional[str]:
+        """
+        Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
+        """
+        return pulumi.get(self, "managed_by")
+
+    @property
+    @pulumi.getter(name="permissionLevel")
+    def permission_level(self) -> Optional[str]:
+        """
+        PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
+        """
+        return pulumi.get(self, "permission_level")
+
+    @property
     @pulumi.getter
     def suspended(self) -> Optional[bool]:
         """
         The User's suspended state.
         """
         return pulumi.get(self, "suspended")
 
@@ -350,36 +400,48 @@
     def get(self, key: str, default = None) -> Any:
         NodeGateway.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  listen_address: str,
                  bind_address: Optional[str] = None,
+                 device: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
+                 location: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
-                 token: Optional[str] = None):
+                 token: Optional[str] = None,
+                 version: Optional[str] = None):
         """
         :param str listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
         :param str bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
+        :param str device: Device is a read only device name uploaded by the gateway process when  it comes online.
         :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
+        :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
         pulumi.set(__self__, "listen_address", listen_address)
         if bind_address is not None:
             pulumi.set(__self__, "bind_address", bind_address)
+        if device is not None:
+            pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
+        if location is not None:
+            pulumi.set(__self__, "location", location)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter(name="listenAddress")
     def listen_address(self) -> str:
         """
         The public hostname/port tuple at which the gateway will be accessible to clients.
         """
@@ -390,23 +452,39 @@
     def bind_address(self) -> Optional[str]:
         """
         The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
         """
         return pulumi.get(self, "bind_address")
 
     @property
+    @pulumi.getter
+    def device(self) -> Optional[str]:
+        """
+        Device is a read only device name uploaded by the gateway process when  it comes online.
+        """
+        return pulumi.get(self, "device")
+
+    @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
         GatewayFilter can be used to restrict the peering between relays and gateways.
         """
         return pulumi.get(self, "gateway_filter")
 
     @property
     @pulumi.getter
+    def location(self) -> Optional[str]:
+        """
+        Location is a read only network location uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "location")
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         """
         return pulumi.get(self, "name")
 
     @property
@@ -418,14 +496,22 @@
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         return pulumi.get(self, "token")
 
+    @property
+    @pulumi.getter
+    def version(self) -> Optional[str]:
+        """
+        Version is a read only sdm binary version uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "version")
+
 
 @pulumi.output_type
 class NodeRelay(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "gatewayFilter":
@@ -439,42 +525,70 @@
         return super().__getitem__(key)
 
     def get(self, key: str, default = None) -> Any:
         NodeRelay.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
+                 device: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
+                 location: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
-                 token: Optional[str] = None):
+                 token: Optional[str] = None,
+                 version: Optional[str] = None):
         """
+        :param str device: Device is a read only device name uploaded by the gateway process when  it comes online.
         :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
+        :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         """
+        if device is not None:
+            pulumi.set(__self__, "device", device)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
+        if location is not None:
+            pulumi.set(__self__, "location", location)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def device(self) -> Optional[str]:
+        """
+        Device is a read only device name uploaded by the gateway process when  it comes online.
+        """
+        return pulumi.get(self, "device")
 
     @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
         GatewayFilter can be used to restrict the peering between relays and gateways.
         """
         return pulumi.get(self, "gateway_filter")
 
     @property
     @pulumi.getter
+    def location(self) -> Optional[str]:
+        """
+        Location is a read only network location uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "location")
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[str]:
         """
         Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         """
         return pulumi.get(self, "name")
 
     @property
@@ -486,14 +600,22 @@
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def token(self) -> Optional[str]:
         return pulumi.get(self, "token")
 
+    @property
+    @pulumi.getter
+    def version(self) -> Optional[str]:
+        """
+        Version is a read only sdm binary version uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "version")
+
 
 @pulumi.output_type
 class ResourceAks(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bindInterface":
@@ -556,21 +678,23 @@
                  secret_store_certificate_authority_key: Optional[str] = None,
                  secret_store_certificate_authority_path: Optional[str] = None,
                  secret_store_client_certificate_key: Optional[str] = None,
                  secret_store_client_certificate_path: Optional[str] = None,
                  secret_store_client_key_key: Optional[str] = None,
                  secret_store_client_key_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -600,14 +724,16 @@
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_client_key_key is not None:
             pulumi.set(__self__, "secret_store_client_key_key", secret_store_client_key_key)
         if secret_store_client_key_path is not None:
             pulumi.set(__self__, "secret_store_client_key_path", secret_store_client_key_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
         return pulumi.get(self, "hostname")
@@ -715,14 +841,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -771,22 +905,24 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -804,14 +940,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -891,14 +1029,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -951,23 +1097,25 @@
                  healthcheck_namespace: Optional[str] = None,
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_token_key: Optional[str] = None,
                  secret_store_token_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str secret_store_token_key: * kubernetes_user_impersonation:
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -983,14 +1131,16 @@
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_token_key is not None:
             pulumi.set(__self__, "secret_store_token_key", secret_store_token_key)
         if secret_store_token_path is not None:
             pulumi.set(__self__, "secret_store_token_path", secret_store_token_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -1068,14 +1218,22 @@
     @property
     @pulumi.getter(name="secretStoreTokenPath")
     def secret_store_token_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_token_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -1122,23 +1280,25 @@
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_token_key: Optional[str] = None,
                  secret_store_token_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str secret_store_token_key: * kubernetes_user_impersonation:
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -1150,14 +1310,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_token_key is not None:
             pulumi.set(__self__, "secret_store_token_key", secret_store_token_key)
         if secret_store_token_path is not None:
             pulumi.set(__self__, "secret_store_token_path", secret_store_token_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -1225,14 +1387,22 @@
     @property
     @pulumi.getter(name="secretStoreTokenPath")
     def secret_store_token_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_token_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -1300,21 +1470,23 @@
                  secret_store_certificate_authority_key: Optional[str] = None,
                  secret_store_certificate_authority_path: Optional[str] = None,
                  secret_store_client_certificate_key: Optional[str] = None,
                  secret_store_client_certificate_path: Optional[str] = None,
                  secret_store_client_key_key: Optional[str] = None,
                  secret_store_client_key_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -1340,14 +1512,16 @@
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_client_key_key is not None:
             pulumi.set(__self__, "secret_store_client_key_key", secret_store_client_key_key)
         if secret_store_client_key_path is not None:
             pulumi.set(__self__, "secret_store_client_key_path", secret_store_client_key_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
         return pulumi.get(self, "hostname")
@@ -1445,14 +1619,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -1539,21 +1721,23 @@
                  secret_store_id: Optional[str] = None,
                  secret_store_role_arn_key: Optional[str] = None,
                  secret_store_role_arn_path: Optional[str] = None,
                  secret_store_role_external_id_key: Optional[str] = None,
                  secret_store_role_external_id_path: Optional[str] = None,
                  secret_store_secret_access_key_key: Optional[str] = None,
                  secret_store_secret_access_key_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
@@ -1594,14 +1778,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> str:
         return pulumi.get(self, "cluster_name")
@@ -1739,14 +1925,514 @@
     @property
     @pulumi.getter(name="secretStoreSecretAccessKeyPath")
     def secret_store_secret_access_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_secret_access_key_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class ResourceAmazonEksInstanceProfile(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clusterName":
+            suggest = "cluster_name"
+        elif key == "bindInterface":
+            suggest = "bind_interface"
+        elif key == "certificateAuthority":
+            suggest = "certificate_authority"
+        elif key == "egressFilter":
+            suggest = "egress_filter"
+        elif key == "healthcheckNamespace":
+            suggest = "healthcheck_namespace"
+        elif key == "remoteIdentityGroupId":
+            suggest = "remote_identity_group_id"
+        elif key == "remoteIdentityHealthcheckUsername":
+            suggest = "remote_identity_healthcheck_username"
+        elif key == "roleArn":
+            suggest = "role_arn"
+        elif key == "roleExternalId":
+            suggest = "role_external_id"
+        elif key == "secretStoreCertificateAuthorityKey":
+            suggest = "secret_store_certificate_authority_key"
+        elif key == "secretStoreCertificateAuthorityPath":
+            suggest = "secret_store_certificate_authority_path"
+        elif key == "secretStoreId":
+            suggest = "secret_store_id"
+        elif key == "secretStoreRoleArnKey":
+            suggest = "secret_store_role_arn_key"
+        elif key == "secretStoreRoleArnPath":
+            suggest = "secret_store_role_arn_path"
+        elif key == "secretStoreRoleExternalIdKey":
+            suggest = "secret_store_role_external_id_key"
+        elif key == "secretStoreRoleExternalIdPath":
+            suggest = "secret_store_role_external_id_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ResourceAmazonEksInstanceProfile. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ResourceAmazonEksInstanceProfile.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ResourceAmazonEksInstanceProfile.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cluster_name: str,
+                 endpoint: str,
+                 name: str,
+                 region: str,
+                 bind_interface: Optional[str] = None,
+                 certificate_authority: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 healthcheck_namespace: Optional[str] = None,
+                 remote_identity_group_id: Optional[str] = None,
+                 remote_identity_healthcheck_username: Optional[str] = None,
+                 role_arn: Optional[str] = None,
+                 role_external_id: Optional[str] = None,
+                 secret_store_certificate_authority_key: Optional[str] = None,
+                 secret_store_certificate_authority_path: Optional[str] = None,
+                 secret_store_id: Optional[str] = None,
+                 secret_store_role_arn_key: Optional[str] = None,
+                 secret_store_role_arn_path: Optional[str] = None,
+                 secret_store_role_external_id_key: Optional[str] = None,
+                 secret_store_role_external_id_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str name: Unique human-readable name of the Resource.
+        :param str bind_interface: Bind interface
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "cluster_name", cluster_name)
+        pulumi.set(__self__, "endpoint", endpoint)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "region", region)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if certificate_authority is not None:
+            pulumi.set(__self__, "certificate_authority", certificate_authority)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if healthcheck_namespace is not None:
+            pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if role_arn is not None:
+            pulumi.set(__self__, "role_arn", role_arn)
+        if role_external_id is not None:
+            pulumi.set(__self__, "role_external_id", role_external_id)
+        if secret_store_certificate_authority_key is not None:
+            pulumi.set(__self__, "secret_store_certificate_authority_key", secret_store_certificate_authority_key)
+        if secret_store_certificate_authority_path is not None:
+            pulumi.set(__self__, "secret_store_certificate_authority_path", secret_store_certificate_authority_path)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if secret_store_role_arn_key is not None:
+            pulumi.set(__self__, "secret_store_role_arn_key", secret_store_role_arn_key)
+        if secret_store_role_arn_path is not None:
+            pulumi.set(__self__, "secret_store_role_arn_path", secret_store_role_arn_path)
+        if secret_store_role_external_id_key is not None:
+            pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
+        if secret_store_role_external_id_path is not None:
+            pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="clusterName")
+    def cluster_name(self) -> str:
+        return pulumi.get(self, "cluster_name")
+
+    @property
+    @pulumi.getter
+    def endpoint(self) -> str:
+        return pulumi.get(self, "endpoint")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def region(self) -> str:
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="certificateAuthority")
+    def certificate_authority(self) -> Optional[str]:
+        return pulumi.get(self, "certificate_authority")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter(name="healthcheckNamespace")
+    def healthcheck_namespace(self) -> Optional[str]:
+        """
+        The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        """
+        return pulumi.get(self, "healthcheck_namespace")
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[str]:
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[str]:
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @property
+    @pulumi.getter(name="roleArn")
+    def role_arn(self) -> Optional[str]:
+        return pulumi.get(self, "role_arn")
+
+    @property
+    @pulumi.getter(name="roleExternalId")
+    def role_external_id(self) -> Optional[str]:
+        return pulumi.get(self, "role_external_id")
+
+    @property
+    @pulumi.getter(name="secretStoreCertificateAuthorityKey")
+    def secret_store_certificate_authority_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_certificate_authority_key")
+
+    @property
+    @pulumi.getter(name="secretStoreCertificateAuthorityPath")
+    def secret_store_certificate_authority_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_certificate_authority_path")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter(name="secretStoreRoleArnKey")
+    def secret_store_role_arn_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_role_arn_key")
+
+    @property
+    @pulumi.getter(name="secretStoreRoleArnPath")
+    def secret_store_role_arn_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_role_arn_path")
+
+    @property
+    @pulumi.getter(name="secretStoreRoleExternalIdKey")
+    def secret_store_role_external_id_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_role_external_id_key")
+
+    @property
+    @pulumi.getter(name="secretStoreRoleExternalIdPath")
+    def secret_store_role_external_id_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_role_external_id_path")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class ResourceAmazonEksInstanceProfileUserImpersonation(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clusterName":
+            suggest = "cluster_name"
+        elif key == "bindInterface":
+            suggest = "bind_interface"
+        elif key == "certificateAuthority":
+            suggest = "certificate_authority"
+        elif key == "egressFilter":
+            suggest = "egress_filter"
+        elif key == "healthcheckNamespace":
+            suggest = "healthcheck_namespace"
+        elif key == "remoteIdentityGroupId":
+            suggest = "remote_identity_group_id"
+        elif key == "remoteIdentityHealthcheckUsername":
+            suggest = "remote_identity_healthcheck_username"
+        elif key == "roleArn":
+            suggest = "role_arn"
+        elif key == "roleExternalId":
+            suggest = "role_external_id"
+        elif key == "secretStoreCertificateAuthorityKey":
+            suggest = "secret_store_certificate_authority_key"
+        elif key == "secretStoreCertificateAuthorityPath":
+            suggest = "secret_store_certificate_authority_path"
+        elif key == "secretStoreId":
+            suggest = "secret_store_id"
+        elif key == "secretStoreRoleArnKey":
+            suggest = "secret_store_role_arn_key"
+        elif key == "secretStoreRoleArnPath":
+            suggest = "secret_store_role_arn_path"
+        elif key == "secretStoreRoleExternalIdKey":
+            suggest = "secret_store_role_external_id_key"
+        elif key == "secretStoreRoleExternalIdPath":
+            suggest = "secret_store_role_external_id_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ResourceAmazonEksInstanceProfileUserImpersonation. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ResourceAmazonEksInstanceProfileUserImpersonation.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ResourceAmazonEksInstanceProfileUserImpersonation.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 cluster_name: str,
+                 endpoint: str,
+                 name: str,
+                 region: str,
+                 bind_interface: Optional[str] = None,
+                 certificate_authority: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 healthcheck_namespace: Optional[str] = None,
+                 remote_identity_group_id: Optional[str] = None,
+                 remote_identity_healthcheck_username: Optional[str] = None,
+                 role_arn: Optional[str] = None,
+                 role_external_id: Optional[str] = None,
+                 secret_store_certificate_authority_key: Optional[str] = None,
+                 secret_store_certificate_authority_path: Optional[str] = None,
+                 secret_store_id: Optional[str] = None,
+                 secret_store_role_arn_key: Optional[str] = None,
+                 secret_store_role_arn_path: Optional[str] = None,
+                 secret_store_role_external_id_key: Optional[str] = None,
+                 secret_store_role_external_id_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str name: Unique human-readable name of the Resource.
+        :param str bind_interface: Bind interface
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "cluster_name", cluster_name)
+        pulumi.set(__self__, "endpoint", endpoint)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "region", region)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if certificate_authority is not None:
+            pulumi.set(__self__, "certificate_authority", certificate_authority)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if healthcheck_namespace is not None:
+            pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if role_arn is not None:
+            pulumi.set(__self__, "role_arn", role_arn)
+        if role_external_id is not None:
+            pulumi.set(__self__, "role_external_id", role_external_id)
+        if secret_store_certificate_authority_key is not None:
+            pulumi.set(__self__, "secret_store_certificate_authority_key", secret_store_certificate_authority_key)
+        if secret_store_certificate_authority_path is not None:
+            pulumi.set(__self__, "secret_store_certificate_authority_path", secret_store_certificate_authority_path)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if secret_store_role_arn_key is not None:
+            pulumi.set(__self__, "secret_store_role_arn_key", secret_store_role_arn_key)
+        if secret_store_role_arn_path is not None:
+            pulumi.set(__self__, "secret_store_role_arn_path", secret_store_role_arn_path)
+        if secret_store_role_external_id_key is not None:
+            pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
+        if secret_store_role_external_id_path is not None:
+            pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="clusterName")
+    def cluster_name(self) -> str:
+        return pulumi.get(self, "cluster_name")
+
+    @property
+    @pulumi.getter
+    def endpoint(self) -> str:
+        return pulumi.get(self, "endpoint")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def region(self) -> str:
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="certificateAuthority")
+    def certificate_authority(self) -> Optional[str]:
+        return pulumi.get(self, "certificate_authority")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter(name="healthcheckNamespace")
+    def healthcheck_namespace(self) -> Optional[str]:
+        """
+        The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        """
+        return pulumi.get(self, "healthcheck_namespace")
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[str]:
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[str]:
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @property
+    @pulumi.getter(name="roleArn")
+    def role_arn(self) -> Optional[str]:
+        return pulumi.get(self, "role_arn")
+
+    @property
+    @pulumi.getter(name="roleExternalId")
+    def role_external_id(self) -> Optional[str]:
+        return pulumi.get(self, "role_external_id")
+
+    @property
+    @pulumi.getter(name="secretStoreCertificateAuthorityKey")
+    def secret_store_certificate_authority_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_certificate_authority_key")
+
+    @property
+    @pulumi.getter(name="secretStoreCertificateAuthorityPath")
+    def secret_store_certificate_authority_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_certificate_authority_path")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter(name="secretStoreRoleArnKey")
+    def secret_store_role_arn_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_role_arn_key")
+
+    @property
+    @pulumi.getter(name="secretStoreRoleArnPath")
+    def secret_store_role_arn_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_role_arn_path")
+
+    @property
+    @pulumi.getter(name="secretStoreRoleExternalIdKey")
+    def secret_store_role_external_id_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_role_external_id_key")
+
+    @property
+    @pulumi.getter(name="secretStoreRoleExternalIdPath")
+    def secret_store_role_external_id_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_role_external_id_path")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -1827,21 +2513,23 @@
                  secret_store_id: Optional[str] = None,
                  secret_store_role_arn_key: Optional[str] = None,
                  secret_store_role_arn_path: Optional[str] = None,
                  secret_store_role_external_id_key: Optional[str] = None,
                  secret_store_role_external_id_path: Optional[str] = None,
                  secret_store_secret_access_key_key: Optional[str] = None,
                  secret_store_secret_access_key_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "cluster_name", cluster_name)
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
@@ -1878,14 +2566,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> str:
         return pulumi.get(self, "cluster_name")
@@ -2013,14 +2703,22 @@
     @property
     @pulumi.getter(name="secretStoreSecretAccessKeyPath")
     def secret_store_secret_access_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_secret_access_key_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -2089,20 +2787,22 @@
                  secret_store_id: Optional[str] = None,
                  secret_store_role_arn_key: Optional[str] = None,
                  secret_store_role_arn_path: Optional[str] = None,
                  secret_store_role_external_id_key: Optional[str] = None,
                  secret_store_role_external_id_path: Optional[str] = None,
                  secret_store_secret_access_key_key: Optional[str] = None,
                  secret_store_secret_access_key_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -2133,14 +2833,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
@@ -2245,14 +2947,22 @@
     @property
     @pulumi.getter(name="secretStoreSecretAccessKeyPath")
     def secret_store_secret_access_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_secret_access_key_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -2300,22 +3010,24 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -2332,14 +3044,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -2413,14 +3127,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -2499,20 +3221,22 @@
                  secret_store_id: Optional[str] = None,
                  secret_store_role_arn_key: Optional[str] = None,
                  secret_store_role_arn_path: Optional[str] = None,
                  secret_store_role_external_id_key: Optional[str] = None,
                  secret_store_role_external_id_path: Optional[str] = None,
                  secret_store_secret_access_key_key: Optional[str] = None,
                  secret_store_secret_access_key_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "output", output)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
@@ -2543,14 +3267,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def name(self) -> str:
         """
@@ -2655,14 +3381,22 @@
     @property
     @pulumi.getter(name="secretStoreSecretAccessKeyPath")
     def secret_store_secret_access_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_secret_access_key_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -2709,21 +3443,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -2741,14 +3477,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -2825,14 +3563,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -2887,21 +3633,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -2921,14 +3669,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -3010,14 +3760,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -3304,14 +4062,15 @@
                  secret_store_role_arn_path: Optional[str] = None,
                  secret_store_role_external_id_key: Optional[str] = None,
                  secret_store_role_external_id_path: Optional[str] = None,
                  session_expiry: Optional[int] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
@@ -3359,14 +4118,17 @@
     @pulumi.getter
     def region(self) -> str:
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def subdomain(self) -> str:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
         Bind interface
@@ -3530,14 +4292,15 @@
                  secret_store_role_external_id_path: Optional[str] = None,
                  secret_store_secret_access_key_key: Optional[str] = None,
                  secret_store_secret_access_key_path: Optional[str] = None,
                  session_expiry: Optional[int] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
@@ -3595,14 +4358,17 @@
     @pulumi.getter
     def region(self) -> str:
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter
     def subdomain(self) -> str:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
 
@@ -3769,15 +4535,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
-        :param str secret_store_tenant_id_key: * azure_postgres:
+        :param str secret_store_tenant_id_key: * azure_mysql:
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -3866,15 +4632,15 @@
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter(name="secretStoreTenantIdKey")
     def secret_store_tenant_id_key(self) -> Optional[str]:
         """
-        * azure_postgres:
+        * azure_mysql:
         """
         return pulumi.get(self, "secret_store_tenant_id_key")
 
     @property
     @pulumi.getter(name="secretStoreTenantIdPath")
     def secret_store_tenant_id_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_tenant_id_path")
@@ -3950,15 +4716,15 @@
                  tags: Optional[Mapping[str, str]] = None,
                  tenant_id: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
-        :param str secret_store_tenant_id_key: * azure_postgres:
+        :param str secret_store_tenant_id_key: * azure_mysql:
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "name", name)
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4047,15 +4813,15 @@
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter(name="secretStoreTenantIdKey")
     def secret_store_tenant_id_key(self) -> Optional[str]:
         """
-        * azure_postgres:
+        * azure_mysql:
         """
         return pulumi.get(self, "secret_store_tenant_id_key")
 
     @property
     @pulumi.getter(name="secretStoreTenantIdPath")
     def secret_store_tenant_id_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_tenant_id_path")
@@ -4071,14 +4837,201 @@
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
+class ResourceAzureMysql(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "bindInterface":
+            suggest = "bind_interface"
+        elif key == "egressFilter":
+            suggest = "egress_filter"
+        elif key == "portOverride":
+            suggest = "port_override"
+        elif key == "secretStoreId":
+            suggest = "secret_store_id"
+        elif key == "secretStorePasswordKey":
+            suggest = "secret_store_password_key"
+        elif key == "secretStorePasswordPath":
+            suggest = "secret_store_password_path"
+        elif key == "secretStoreUsernameKey":
+            suggest = "secret_store_username_key"
+        elif key == "secretStoreUsernamePath":
+            suggest = "secret_store_username_path"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ResourceAzureMysql. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ResourceAzureMysql.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ResourceAzureMysql.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 database: str,
+                 hostname: str,
+                 name: str,
+                 bind_interface: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 password: Optional[str] = None,
+                 port: Optional[int] = None,
+                 port_override: Optional[int] = None,
+                 secret_store_id: Optional[str] = None,
+                 secret_store_password_key: Optional[str] = None,
+                 secret_store_password_path: Optional[str] = None,
+                 secret_store_username_key: Optional[str] = None,
+                 secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 username: Optional[str] = None):
+        """
+        :param str name: Unique human-readable name of the Resource.
+        :param str bind_interface: Bind interface
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "database", database)
+        pulumi.set(__self__, "hostname", hostname)
+        pulumi.set(__self__, "name", name)
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if secret_store_password_key is not None:
+            pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
+        if secret_store_password_path is not None:
+            pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if secret_store_username_key is not None:
+            pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
+        if secret_store_username_path is not None:
+            pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter
+    def database(self) -> str:
+        return pulumi.get(self, "database")
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> str:
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[str]:
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter(name="secretStorePasswordKey")
+    def secret_store_password_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_password_key")
+
+    @property
+    @pulumi.getter(name="secretStorePasswordPath")
+    def secret_store_password_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_password_path")
+
+    @property
+    @pulumi.getter(name="secretStoreUsernameKey")
+    def secret_store_username_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_username_key")
+
+    @property
+    @pulumi.getter(name="secretStoreUsernamePath")
+    def secret_store_username_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_username_path")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
 class ResourceAzurePostgres(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bindInterface":
             suggest = "bind_interface"
         elif key == "egressFilter":
@@ -4120,21 +5073,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4154,14 +5109,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -4243,14 +5200,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -4297,21 +5262,23 @@
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  port_override: Optional[int] = None,
                  private_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_private_key_key: Optional[str] = None,
                  secret_store_private_key_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project", project)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4323,14 +5290,16 @@
             pulumi.set(__self__, "private_key", private_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_private_key_key is not None:
             pulumi.set(__self__, "secret_store_private_key_key", secret_store_private_key_key)
         if secret_store_private_key_path is not None:
             pulumi.set(__self__, "secret_store_private_key_path", secret_store_private_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -4392,14 +5361,22 @@
     @property
     @pulumi.getter(name="secretStorePrivateKeyPath")
     def secret_store_private_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_private_key_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -4452,22 +5429,24 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -4484,14 +5463,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -4565,14 +5546,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -4632,21 +5621,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4666,14 +5657,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -4755,14 +5748,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -4814,21 +5815,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -4846,14 +5849,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -4930,14 +5935,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -4992,21 +6005,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5026,14 +6041,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -5115,14 +6132,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -5175,22 +6200,24 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5206,14 +6233,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -5287,14 +6316,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -5351,21 +6388,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5383,14 +6422,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -5467,14 +6508,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -5528,21 +6577,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -5560,14 +6611,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
@@ -5644,14 +6697,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -5710,21 +6771,23 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
@@ -5743,14 +6806,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
@@ -5832,14 +6897,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -5890,21 +6963,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -5921,14 +6996,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -6000,14 +7077,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -6081,20 +7166,22 @@
                  secret_store_id: Optional[str] = None,
                  secret_store_role_arn_key: Optional[str] = None,
                  secret_store_role_arn_path: Optional[str] = None,
                  secret_store_role_external_id_key: Optional[str] = None,
                  secret_store_role_external_id_path: Optional[str] = None,
                  secret_store_secret_access_key_key: Optional[str] = None,
                  secret_store_secret_access_key_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
@@ -6124,14 +7211,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
         return pulumi.get(self, "endpoint")
@@ -6236,14 +7325,22 @@
     @property
     @pulumi.getter(name="secretStoreSecretAccessKeyPath")
     def secret_store_secret_access_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_secret_access_key_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -6291,22 +7388,24 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -6323,14 +7422,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -6404,14 +7505,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -6438,14 +7547,18 @@
             suggest = "port_override"
         elif key == "secretStoreId":
             suggest = "secret_store_id"
         elif key == "secretStorePasswordKey":
             suggest = "secret_store_password_key"
         elif key == "secretStorePasswordPath":
             suggest = "secret_store_password_path"
+        elif key == "secretStoreUsernameKey":
+            suggest = "secret_store_username_key"
+        elif key == "secretStoreUsernamePath":
+            suggest = "secret_store_username_path"
         elif key == "tlsRequired":
             suggest = "tls_required"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ResourceElasticacheRedis. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
@@ -6463,21 +7576,26 @@
                  egress_filter: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
+                 secret_store_username_key: Optional[str] = None,
+                 secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
-                 tls_required: Optional[bool] = None):
+                 tls_required: Optional[bool] = None,
+                 username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -6490,18 +7608,26 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if secret_store_username_key is not None:
+            pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
+        if secret_store_username_path is not None:
+            pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
         return pulumi.get(self, "hostname")
 
     @property
@@ -6558,26 +7684,49 @@
 
     @property
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
+    @pulumi.getter(name="secretStoreUsernameKey")
+    def secret_store_username_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_username_key")
+
+    @property
+    @pulumi.getter(name="secretStoreUsernamePath")
+    def secret_store_username_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_username_path")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
         return pulumi.get(self, "tls_required")
 
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
+
 
 @pulumi.output_type
 class ResourceGcp(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bindInterface":
@@ -6749,21 +7898,23 @@
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_certificate_authority_key: Optional[str] = None,
                  secret_store_certificate_authority_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_service_account_key_key: Optional[str] = None,
                  secret_store_service_account_key_path: Optional[str] = None,
                  service_account_key: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -6784,14 +7935,16 @@
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_service_account_key_key is not None:
             pulumi.set(__self__, "secret_store_service_account_key_key", secret_store_service_account_key_key)
         if secret_store_service_account_key_path is not None:
             pulumi.set(__self__, "secret_store_service_account_key_path", secret_store_service_account_key_path)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
         return pulumi.get(self, "endpoint")
@@ -6874,14 +8027,22 @@
     @property
     @pulumi.getter(name="serviceAccountKey")
     def service_account_key(self) -> Optional[str]:
         return pulumi.get(self, "service_account_key")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -6931,21 +8092,23 @@
                  healthcheck_namespace: Optional[str] = None,
                  secret_store_certificate_authority_key: Optional[str] = None,
                  secret_store_certificate_authority_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_service_account_key_key: Optional[str] = None,
                  secret_store_service_account_key_path: Optional[str] = None,
                  service_account_key: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -6962,14 +8125,16 @@
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_service_account_key_key is not None:
             pulumi.set(__self__, "secret_store_service_account_key_key", secret_store_service_account_key_key)
         if secret_store_service_account_key_path is not None:
             pulumi.set(__self__, "secret_store_service_account_key_path", secret_store_service_account_key_path)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
         return pulumi.get(self, "endpoint")
@@ -7042,14 +8207,22 @@
     @property
     @pulumi.getter(name="serviceAccountKey")
     def service_account_key(self) -> Optional[str]:
         return pulumi.get(self, "service_account_key")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -7099,21 +8272,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -7133,14 +8308,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -7222,14 +8399,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -7288,14 +8473,15 @@
                  host_override: Optional[str] = None,
                  secret_store_auth_header_key: Optional[str] = None,
                  secret_store_auth_header_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param str url: * kubernetes:
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
@@ -7335,14 +8521,17 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def subdomain(self) -> str:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def url(self) -> str:
         """
         * kubernetes:
@@ -7467,14 +8656,15 @@
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param str url: * kubernetes:
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
@@ -7520,14 +8710,17 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def subdomain(self) -> str:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def url(self) -> str:
         """
         * kubernetes:
@@ -7653,14 +8846,15 @@
                  egress_filter: Optional[str] = None,
                  headers_blacklist: Optional[str] = None,
                  host_override: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param str url: * kubernetes:
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_path", healthcheck_path)
@@ -7694,14 +8888,17 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def subdomain(self) -> str:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def url(self) -> str:
         """
         * kubernetes:
@@ -7821,21 +9018,23 @@
                  secret_store_certificate_authority_key: Optional[str] = None,
                  secret_store_certificate_authority_path: Optional[str] = None,
                  secret_store_client_certificate_key: Optional[str] = None,
                  secret_store_client_certificate_path: Optional[str] = None,
                  secret_store_client_key_key: Optional[str] = None,
                  secret_store_client_key_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -7865,14 +9064,16 @@
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_client_key_key is not None:
             pulumi.set(__self__, "secret_store_client_key_key", secret_store_client_key_key)
         if secret_store_client_key_path is not None:
             pulumi.set(__self__, "secret_store_client_key_path", secret_store_client_key_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
         return pulumi.get(self, "hostname")
@@ -7980,14 +9181,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -8036,22 +9245,24 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8069,14 +9280,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -8156,14 +9369,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -8216,23 +9437,25 @@
                  healthcheck_namespace: Optional[str] = None,
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_token_key: Optional[str] = None,
                  secret_store_token_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str secret_store_token_key: * kubernetes_user_impersonation:
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8248,14 +9471,16 @@
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_token_key is not None:
             pulumi.set(__self__, "secret_store_token_key", secret_store_token_key)
         if secret_store_token_path is not None:
             pulumi.set(__self__, "secret_store_token_path", secret_store_token_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -8333,14 +9558,22 @@
     @property
     @pulumi.getter(name="secretStoreTokenPath")
     def secret_store_token_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_token_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -8387,23 +9620,25 @@
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_token_key: Optional[str] = None,
                  secret_store_token_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param str secret_store_token_key: * kubernetes_user_impersonation:
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8415,14 +9650,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_token_key is not None:
             pulumi.set(__self__, "secret_store_token_key", secret_store_token_key)
         if secret_store_token_path is not None:
             pulumi.set(__self__, "secret_store_token_path", secret_store_token_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
@@ -8490,14 +9727,22 @@
     @property
     @pulumi.getter(name="secretStoreTokenPath")
     def secret_store_token_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_token_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -8565,21 +9810,23 @@
                  secret_store_certificate_authority_key: Optional[str] = None,
                  secret_store_certificate_authority_path: Optional[str] = None,
                  secret_store_client_certificate_key: Optional[str] = None,
                  secret_store_client_certificate_path: Optional[str] = None,
                  secret_store_client_key_key: Optional[str] = None,
                  secret_store_client_key_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8605,14 +9852,16 @@
             pulumi.set(__self__, "secret_store_client_certificate_path", secret_store_client_certificate_path)
         if secret_store_client_key_key is not None:
             pulumi.set(__self__, "secret_store_client_key_key", secret_store_client_key_key)
         if secret_store_client_key_path is not None:
             pulumi.set(__self__, "secret_store_client_key_path", secret_store_client_key_path)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
         return pulumi.get(self, "hostname")
@@ -8710,14 +9959,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -8764,21 +10021,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -8796,14 +10055,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -8880,14 +10141,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -8925,34 +10194,38 @@
                  hostname: str,
                  name: str,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
         return pulumi.get(self, "hostname")
@@ -8997,14 +10270,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -9051,21 +10332,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9083,14 +10366,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -9167,14 +10452,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -9230,22 +10523,24 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9263,14 +10558,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -9349,14 +10646,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -9420,22 +10725,24 @@
                  port_override: Optional[int] = None,
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -9455,14 +10762,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -9546,14 +10855,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -9620,22 +10937,24 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
@@ -9656,14 +10975,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -9752,14 +11073,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -9826,22 +11155,24 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "replica_set", replica_set)
         if bind_interface is not None:
@@ -9862,14 +11193,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -9958,14 +11291,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -10025,22 +11366,24 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "auth_database", auth_database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -10056,14 +11399,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -10137,14 +11482,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -10231,21 +11584,23 @@
                  secret_store_client_key_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
                  server_name: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -10283,14 +11638,16 @@
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
         if server_name is not None:
             pulumi.set(__self__, "server_name", server_name)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -10417,14 +11774,22 @@
     @property
     @pulumi.getter(name="serverName")
     def server_name(self) -> Optional[str]:
         return pulumi.get(self, "server_name")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -10509,21 +11874,23 @@
                  secret_store_client_key_path: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
                  server_name: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -10563,14 +11930,16 @@
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
         if server_name is not None:
             pulumi.set(__self__, "server_name", server_name)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -10702,14 +12071,22 @@
     @property
     @pulumi.getter(name="serverName")
     def server_name(self) -> Optional[str]:
         return pulumi.get(self, "server_name")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -10761,21 +12138,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -10793,14 +12172,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -10877,14 +12258,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -10922,34 +12311,38 @@
                  endpoint: str,
                  name: str,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
         return pulumi.get(self, "endpoint")
@@ -10994,14 +12387,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -11071,20 +12472,22 @@
                  secret_store_id: Optional[str] = None,
                  secret_store_role_arn_key: Optional[str] = None,
                  secret_store_role_arn_path: Optional[str] = None,
                  secret_store_role_external_id_key: Optional[str] = None,
                  secret_store_role_external_id_path: Optional[str] = None,
                  secret_store_secret_access_key_key: Optional[str] = None,
                  secret_store_secret_access_key_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "endpoint", endpoint)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "region", region)
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
@@ -11116,14 +12519,16 @@
             pulumi.set(__self__, "secret_store_role_external_id_key", secret_store_role_external_id_key)
         if secret_store_role_external_id_path is not None:
             pulumi.set(__self__, "secret_store_role_external_id_path", secret_store_role_external_id_path)
         if secret_store_secret_access_key_key is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_key", secret_store_secret_access_key_key)
         if secret_store_secret_access_key_path is not None:
             pulumi.set(__self__, "secret_store_secret_access_key_path", secret_store_secret_access_key_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def endpoint(self) -> str:
         return pulumi.get(self, "endpoint")
@@ -11233,14 +12638,22 @@
     @property
     @pulumi.getter(name="secretStoreSecretAccessKeyPath")
     def secret_store_secret_access_key_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_secret_access_key_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -11289,22 +12702,24 @@
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if bind_interface is not None:
@@ -11321,14 +12736,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -11407,14 +12824,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -11474,21 +12899,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -11508,14 +12935,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -11597,14 +13026,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -11652,22 +13089,24 @@
                  egress_filter: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -11681,14 +13120,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -11757,14 +13198,22 @@
     @property
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -11822,22 +13271,24 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -11854,14 +13305,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -11935,14 +13388,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -11985,34 +13446,38 @@
                  hostname: str,
                  name: str,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
         return pulumi.get(self, "hostname")
@@ -12057,14 +13522,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -12102,57 +13575,62 @@
     def get(self, key: str, default = None) -> Any:
         ResourceRdp.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  hostname: str,
                  name: str,
-                 port: int,
                  bind_interface: Optional[str] = None,
                  downgrade_nla_connections: Optional[bool] = None,
                  egress_filter: Optional[str] = None,
                  password: Optional[str] = None,
+                 port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
-        pulumi.set(__self__, "port", port)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if downgrade_nla_connections is not None:
             pulumi.set(__self__, "downgrade_nla_connections", downgrade_nla_connections)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if password is not None:
             pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -12164,19 +13642,14 @@
     def name(self) -> str:
         """
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
-    @pulumi.getter
-    def port(self) -> int:
-        return pulumi.get(self, "port")
-
-    @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
         Bind interface
         """
         return pulumi.get(self, "bind_interface")
 
@@ -12195,14 +13668,19 @@
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         return pulumi.get(self, "password")
 
     @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        return pulumi.get(self, "port")
+
+    @property
     @pulumi.getter(name="portOverride")
     def port_override(self) -> Optional[int]:
         return pulumi.get(self, "port_override")
 
     @property
     @pulumi.getter(name="secretStoreId")
     def secret_store_id(self) -> Optional[str]:
@@ -12229,14 +13707,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -12258,14 +13744,20 @@
             suggest = "port_override"
         elif key == "secretStoreId":
             suggest = "secret_store_id"
         elif key == "secretStorePasswordKey":
             suggest = "secret_store_password_key"
         elif key == "secretStorePasswordPath":
             suggest = "secret_store_password_path"
+        elif key == "secretStoreUsernameKey":
+            suggest = "secret_store_username_key"
+        elif key == "secretStoreUsernamePath":
+            suggest = "secret_store_username_path"
+        elif key == "tlsRequired":
+            suggest = "tls_required"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in ResourceRedis. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         ResourceRedis.__key_warning(key)
         return super().__getitem__(key)
@@ -12281,20 +13773,26 @@
                  egress_filter: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
-                 tags: Optional[Mapping[str, str]] = None):
+                 secret_store_username_key: Optional[str] = None,
+                 secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 tls_required: Optional[bool] = None,
+                 username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -12307,16 +13805,26 @@
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_password_key is not None:
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
+        if secret_store_username_key is not None:
+            pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
+        if secret_store_username_path is not None:
+            pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if tls_required is not None:
+            pulumi.set(__self__, "tls_required", tls_required)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def hostname(self) -> str:
         return pulumi.get(self, "hostname")
 
     @property
@@ -12373,21 +13881,49 @@
 
     @property
     @pulumi.getter(name="secretStorePasswordPath")
     def secret_store_password_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_password_path")
 
     @property
+    @pulumi.getter(name="secretStoreUsernameKey")
+    def secret_store_username_key(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_username_key")
+
+    @property
+    @pulumi.getter(name="secretStoreUsernamePath")
+    def secret_store_username_path(self) -> Optional[str]:
+        return pulumi.get(self, "secret_store_username_path")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
+    @property
+    @pulumi.getter(name="tlsRequired")
+    def tls_required(self) -> Optional[bool]:
+        return pulumi.get(self, "tls_required")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
+
 
 @pulumi.output_type
 class ResourceRedshift(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bindInterface":
@@ -12431,21 +13967,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -12465,14 +14003,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -12554,14 +14094,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -12613,21 +14161,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -12645,14 +14195,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -12729,14 +14281,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -12788,21 +14348,23 @@
                  port_override: Optional[int] = None,
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -12820,14 +14382,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -12904,14 +14468,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -12963,14 +14535,15 @@
                  saml_metadata: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_saml_metadata_key: Optional[str] = None,
                  secret_store_saml_metadata_path: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str name: Unique human-readable name of the Resource.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "healthcheck_username", healthcheck_username)
         pulumi.set(__self__, "name", name)
@@ -13004,14 +14577,17 @@
         Unique human-readable name of the Resource.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def subdomain(self) -> str:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
         Bind interface
@@ -13110,21 +14686,23 @@
                  port_override: Optional[int] = None,
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "database", database)
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -13146,14 +14724,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -13240,14 +14820,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -13303,21 +14891,23 @@
                  key_type: Optional[str] = None,
                  port_forwarding: Optional[bool] = None,
                  port_override: Optional[int] = None,
                  public_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
@@ -13335,14 +14925,16 @@
             pulumi.set(__self__, "public_key", public_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -13419,14 +15011,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -13485,21 +15085,23 @@
                  port_forwarding: Optional[bool] = None,
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
@@ -13519,14 +15121,16 @@
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -13608,14 +15212,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -13674,21 +15286,23 @@
                  port_override: Optional[int] = None,
                  private_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_private_key_key: Optional[str] = None,
                  secret_store_private_key_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "port", port)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
@@ -13708,14 +15322,16 @@
             pulumi.set(__self__, "secret_store_private_key_key", secret_store_private_key_key)
         if secret_store_private_key_path is not None:
             pulumi.set(__self__, "secret_store_private_key_path", secret_store_private_key_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -13797,14 +15413,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -13855,21 +15479,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -13886,14 +15512,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -13965,14 +15593,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -14023,21 +15659,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -14054,14 +15692,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -14133,14 +15773,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -14191,21 +15839,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  secret_store_password_key: Optional[str] = None,
                  secret_store_password_path: Optional[str] = None,
                  secret_store_username_key: Optional[str] = None,
                  secret_store_username_path: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str name: Unique human-readable name of the Resource.
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "hostname", hostname)
         pulumi.set(__self__, "name", name)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -14222,14 +15872,16 @@
             pulumi.set(__self__, "secret_store_password_key", secret_store_password_key)
         if secret_store_password_path is not None:
             pulumi.set(__self__, "secret_store_password_path", secret_store_password_path)
         if secret_store_username_key is not None:
             pulumi.set(__self__, "secret_store_username_key", secret_store_username_key)
         if secret_store_username_path is not None:
             pulumi.set(__self__, "secret_store_username_path", secret_store_username_path)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
@@ -14301,14 +15953,22 @@
     @property
     @pulumi.getter(name="secretStoreUsernamePath")
     def secret_store_username_path(self) -> Optional[str]:
         return pulumi.get(self, "secret_store_username_path")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -14463,14 +16123,68 @@
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
+class SecretStoreCyberarkPam(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "appUrl":
+            suggest = "app_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in SecretStoreCyberarkPam. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        SecretStoreCyberarkPam.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        SecretStoreCyberarkPam.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 app_url: str,
+                 name: str,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str name: Unique human-readable name of the SecretStore.
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        pulumi.set(__self__, "app_url", app_url)
+        pulumi.set(__self__, "name", name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="appUrl")
+    def app_url(self) -> str:
+        return pulumi.get(self, "app_url")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
 class SecretStoreCyberarkPamExperimental(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "appUrl":
             suggest = "app_url"
 
@@ -14930,50 +16644,84 @@
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
 class GetAccountAccountUserResult(dict):
     def __init__(__self__, *,
+                 managed_by: str,
+                 permission_level: str,
                  email: Optional[str] = None,
+                 external_id: Optional[str] = None,
                  first_name: Optional[str] = None,
                  id: Optional[str] = None,
                  last_name: Optional[str] = None,
                  suspended: Optional[bool] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str managed_by: Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
+        :param str permission_level: PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
         :param str email: The User's email address. Must be unique.
+        :param str external_id: External ID is an alternative unique ID this user is represented by within an external service.
         :param str first_name: The User's first name.
         :param str id: Unique identifier of the User.
         :param str last_name: The User's last name.
         :param bool suspended: The User's suspended state.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
+        pulumi.set(__self__, "managed_by", managed_by)
+        pulumi.set(__self__, "permission_level", permission_level)
         if email is not None:
             pulumi.set(__self__, "email", email)
+        if external_id is not None:
+            pulumi.set(__self__, "external_id", external_id)
         if first_name is not None:
             pulumi.set(__self__, "first_name", first_name)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if last_name is not None:
             pulumi.set(__self__, "last_name", last_name)
         if suspended is not None:
             pulumi.set(__self__, "suspended", suspended)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
+    @pulumi.getter(name="managedBy")
+    def managed_by(self) -> str:
+        """
+        Managed By is a read only field for what service manages this user, e.g. StrongDM, Okta, Azure.
+        """
+        return pulumi.get(self, "managed_by")
+
+    @property
+    @pulumi.getter(name="permissionLevel")
+    def permission_level(self) -> str:
+        """
+        PermissionLevel is a read only field for the user's permission level e.g. admin, DBA, user.
+        """
+        return pulumi.get(self, "permission_level")
+
+    @property
     @pulumi.getter
     def email(self) -> Optional[str]:
         """
         The User's email address. Must be unique.
         """
         return pulumi.get(self, "email")
 
     @property
+    @pulumi.getter(name="externalId")
+    def external_id(self) -> Optional[str]:
+        """
+        External ID is an alternative unique ID this user is represented by within an external service.
+        """
+        return pulumi.get(self, "external_id")
+
+    @property
     @pulumi.getter(name="firstName")
     def first_name(self) -> Optional[str]:
         """
         The User's first name.
         """
         return pulumi.get(self, "first_name")
 
@@ -15071,42 +16819,75 @@
     def relays(self) -> Sequence['outputs.GetNodeNodeRelayResult']:
         return pulumi.get(self, "relays")
 
 
 @pulumi.output_type
 class GetNodeNodeGatewayResult(dict):
     def __init__(__self__, *,
+                 device: str,
+                 location: str,
+                 version: str,
                  bind_address: Optional[str] = None,
                  gateway_filter: Optional[str] = None,
                  id: Optional[str] = None,
                  listen_address: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str device: Device is a read only device name uploaded by the gateway process when  it comes online.
+        :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
+        :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         :param str bind_address: The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
         :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
         :param str id: Unique identifier of the Relay.
         :param str listen_address: The public hostname/port tuple at which the gateway will be accessible to clients.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
+        pulumi.set(__self__, "device", device)
+        pulumi.set(__self__, "location", location)
+        pulumi.set(__self__, "version", version)
         if bind_address is not None:
             pulumi.set(__self__, "bind_address", bind_address)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if listen_address is not None:
             pulumi.set(__self__, "listen_address", listen_address)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
+    @pulumi.getter
+    def device(self) -> str:
+        """
+        Device is a read only device name uploaded by the gateway process when  it comes online.
+        """
+        return pulumi.get(self, "device")
+
+    @property
+    @pulumi.getter
+    def location(self) -> str:
+        """
+        Location is a read only network location uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "location")
+
+    @property
+    @pulumi.getter
+    def version(self) -> str:
+        """
+        Version is a read only sdm binary version uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "version")
+
+    @property
     @pulumi.getter(name="bindAddress")
     def bind_address(self) -> Optional[str]:
         """
         The hostname/port tuple which the gateway daemon will bind to. If not provided on create, set to "0.0.0.0:listen_address_port".
         """
         return pulumi.get(self, "bind_address")
 
@@ -15150,34 +16931,67 @@
         """
         return pulumi.get(self, "tags")
 
 
 @pulumi.output_type
 class GetNodeNodeRelayResult(dict):
     def __init__(__self__, *,
+                 device: str,
+                 location: str,
+                 version: str,
                  gateway_filter: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str device: Device is a read only device name uploaded by the gateway process when  it comes online.
+        :param str location: Location is a read only network location uploaded by the gateway process when it comes online.
+        :param str version: Version is a read only sdm binary version uploaded by the gateway process when it comes online.
         :param str gateway_filter: GatewayFilter can be used to restrict the peering between relays and gateways.
         :param str id: Unique identifier of the Relay.
         :param str name: Unique human-readable name of the Relay. Node names must include only letters, numbers, and hyphens (no spaces, underscores, or other special characters). Generated if not provided on create.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
+        pulumi.set(__self__, "device", device)
+        pulumi.set(__self__, "location", location)
+        pulumi.set(__self__, "version", version)
         if gateway_filter is not None:
             pulumi.set(__self__, "gateway_filter", gateway_filter)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
+    @pulumi.getter
+    def device(self) -> str:
+        """
+        Device is a read only device name uploaded by the gateway process when  it comes online.
+        """
+        return pulumi.get(self, "device")
+
+    @property
+    @pulumi.getter
+    def location(self) -> str:
+        """
+        Location is a read only network location uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "location")
+
+    @property
+    @pulumi.getter
+    def version(self) -> str:
+        """
+        Version is a read only sdm binary version uploaded by the gateway process when it comes online.
+        """
+        return pulumi.get(self, "version")
+
+    @property
     @pulumi.getter(name="gatewayFilter")
     def gateway_filter(self) -> Optional[str]:
         """
         GatewayFilter can be used to restrict the peering between relays and gateways.
         """
         return pulumi.get(self, "gateway_filter")
 
@@ -15297,24 +17111,27 @@
     def __init__(__self__, *,
                  aks: Sequence['outputs.GetResourceResourceAkResult'],
                  aks_basic_auths: Sequence['outputs.GetResourceResourceAksBasicAuthResult'],
                  aks_service_account_user_impersonations: Sequence['outputs.GetResourceResourceAksServiceAccountUserImpersonationResult'],
                  aks_service_accounts: Sequence['outputs.GetResourceResourceAksServiceAccountResult'],
                  aks_user_impersonations: Sequence['outputs.GetResourceResourceAksUserImpersonationResult'],
                  amazon_eks: Sequence['outputs.GetResourceResourceAmazonEkResult'],
+                 amazon_eks_instance_profile_user_impersonations: Sequence['outputs.GetResourceResourceAmazonEksInstanceProfileUserImpersonationResult'],
+                 amazon_eks_instance_profiles: Sequence['outputs.GetResourceResourceAmazonEksInstanceProfileResult'],
                  amazon_eks_user_impersonations: Sequence['outputs.GetResourceResourceAmazonEksUserImpersonationResult'],
                  amazon_es: Sequence['outputs.GetResourceResourceAmazonEResult'],
                  amazonmq_amqp091s: Sequence['outputs.GetResourceResourceAmazonmqAmqp091Result'],
                  athenas: Sequence['outputs.GetResourceResourceAthenaResult'],
                  aurora_mysqls: Sequence['outputs.GetResourceResourceAuroraMysqlResult'],
                  aurora_postgres: Sequence['outputs.GetResourceResourceAuroraPostgreResult'],
                  aws: Sequence['outputs.GetResourceResourceAwResult'],
                  aws_console_static_key_pairs: Sequence['outputs.GetResourceResourceAwsConsoleStaticKeyPairResult'],
                  aws_consoles: Sequence['outputs.GetResourceResourceAwsConsoleResult'],
                  azure_certificates: Sequence['outputs.GetResourceResourceAzureCertificateResult'],
+                 azure_mysqls: Sequence['outputs.GetResourceResourceAzureMysqlResult'],
                  azure_postgres: Sequence['outputs.GetResourceResourceAzurePostgreResult'],
                  azures: Sequence['outputs.GetResourceResourceAzureResult'],
                  big_queries: Sequence['outputs.GetResourceResourceBigQueryResult'],
                  cassandras: Sequence['outputs.GetResourceResourceCassandraResult'],
                  cituses: Sequence['outputs.GetResourceResourceCitusResult'],
                  clustrixes: Sequence['outputs.GetResourceResourceClustrixResult'],
                  cockroaches: Sequence['outputs.GetResourceResourceCockroachResult'],
@@ -15371,24 +17188,27 @@
                  teradatas: Sequence['outputs.GetResourceResourceTeradataResult']):
         pulumi.set(__self__, "aks", aks)
         pulumi.set(__self__, "aks_basic_auths", aks_basic_auths)
         pulumi.set(__self__, "aks_service_account_user_impersonations", aks_service_account_user_impersonations)
         pulumi.set(__self__, "aks_service_accounts", aks_service_accounts)
         pulumi.set(__self__, "aks_user_impersonations", aks_user_impersonations)
         pulumi.set(__self__, "amazon_eks", amazon_eks)
+        pulumi.set(__self__, "amazon_eks_instance_profile_user_impersonations", amazon_eks_instance_profile_user_impersonations)
+        pulumi.set(__self__, "amazon_eks_instance_profiles", amazon_eks_instance_profiles)
         pulumi.set(__self__, "amazon_eks_user_impersonations", amazon_eks_user_impersonations)
         pulumi.set(__self__, "amazon_es", amazon_es)
         pulumi.set(__self__, "amazonmq_amqp091s", amazonmq_amqp091s)
         pulumi.set(__self__, "athenas", athenas)
         pulumi.set(__self__, "aurora_mysqls", aurora_mysqls)
         pulumi.set(__self__, "aurora_postgres", aurora_postgres)
         pulumi.set(__self__, "aws", aws)
         pulumi.set(__self__, "aws_console_static_key_pairs", aws_console_static_key_pairs)
         pulumi.set(__self__, "aws_consoles", aws_consoles)
         pulumi.set(__self__, "azure_certificates", azure_certificates)
+        pulumi.set(__self__, "azure_mysqls", azure_mysqls)
         pulumi.set(__self__, "azure_postgres", azure_postgres)
         pulumi.set(__self__, "azures", azures)
         pulumi.set(__self__, "big_queries", big_queries)
         pulumi.set(__self__, "cassandras", cassandras)
         pulumi.set(__self__, "cituses", cituses)
         pulumi.set(__self__, "clustrixes", clustrixes)
         pulumi.set(__self__, "cockroaches", cockroaches)
@@ -15471,14 +17291,24 @@
 
     @property
     @pulumi.getter(name="amazonEks")
     def amazon_eks(self) -> Sequence['outputs.GetResourceResourceAmazonEkResult']:
         return pulumi.get(self, "amazon_eks")
 
     @property
+    @pulumi.getter(name="amazonEksInstanceProfileUserImpersonations")
+    def amazon_eks_instance_profile_user_impersonations(self) -> Sequence['outputs.GetResourceResourceAmazonEksInstanceProfileUserImpersonationResult']:
+        return pulumi.get(self, "amazon_eks_instance_profile_user_impersonations")
+
+    @property
+    @pulumi.getter(name="amazonEksInstanceProfiles")
+    def amazon_eks_instance_profiles(self) -> Sequence['outputs.GetResourceResourceAmazonEksInstanceProfileResult']:
+        return pulumi.get(self, "amazon_eks_instance_profiles")
+
+    @property
     @pulumi.getter(name="amazonEksUserImpersonations")
     def amazon_eks_user_impersonations(self) -> Sequence['outputs.GetResourceResourceAmazonEksUserImpersonationResult']:
         return pulumi.get(self, "amazon_eks_user_impersonations")
 
     @property
     @pulumi.getter(name="amazonEs")
     def amazon_es(self) -> Sequence['outputs.GetResourceResourceAmazonEResult']:
@@ -15521,14 +17351,19 @@
 
     @property
     @pulumi.getter(name="azureCertificates")
     def azure_certificates(self) -> Sequence['outputs.GetResourceResourceAzureCertificateResult']:
         return pulumi.get(self, "azure_certificates")
 
     @property
+    @pulumi.getter(name="azureMysqls")
+    def azure_mysqls(self) -> Sequence['outputs.GetResourceResourceAzureMysqlResult']:
+        return pulumi.get(self, "azure_mysqls")
+
+    @property
     @pulumi.getter(name="azurePostgres")
     def azure_postgres(self) -> Sequence['outputs.GetResourceResourceAzurePostgreResult']:
         return pulumi.get(self, "azure_postgres")
 
     @property
     @pulumi.getter
     def azures(self) -> Sequence['outputs.GetResourceResourceAzureResult']:
@@ -15828,22 +17663,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if client_certificate is not None:
@@ -15866,14 +17703,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if remote_identity_group_id is not None:
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -15959,14 +17798,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -15979,23 +17826,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
@@ -16010,14 +17859,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -16085,14 +17936,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -16111,23 +17970,25 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str token: * kubernetes_user_impersonation:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -16145,14 +18006,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if remote_identity_group_id is not None:
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -16225,14 +18088,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -16252,23 +18123,25 @@
                  healthcheck_namespace: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str token: * kubernetes_user_impersonation:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -16282,14 +18155,16 @@
             pulumi.set(__self__, "name", name)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -16352,14 +18227,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -16382,22 +18265,24 @@
                  healthcheck_namespace: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if client_certificate is not None:
@@ -16416,14 +18301,16 @@
             pulumi.set(__self__, "name", name)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -16499,14 +18386,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -16521,21 +18416,23 @@
                  name: Optional[str] = None,
                  port_override: Optional[int] = None,
                  region: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -16554,14 +18451,16 @@
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
@@ -16634,14 +18533,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -16660,22 +18567,24 @@
                  region: Optional[str] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -16702,14 +18611,16 @@
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
@@ -16805,14 +18716,356 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class GetResourceResourceAmazonEksInstanceProfileResult(dict):
+    def __init__(__self__, *,
+                 bind_interface: Optional[str] = None,
+                 certificate_authority: Optional[str] = None,
+                 cluster_name: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 endpoint: Optional[str] = None,
+                 healthcheck_namespace: Optional[str] = None,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None,
+                 region: Optional[str] = None,
+                 remote_identity_group_id: Optional[str] = None,
+                 remote_identity_healthcheck_username: Optional[str] = None,
+                 role_arn: Optional[str] = None,
+                 role_external_id: Optional[str] = None,
+                 secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str bind_interface: Bind interface
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str id: Unique identifier of the Resource.
+        :param str name: Unique human-readable name of the Resource.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if certificate_authority is not None:
+            pulumi.set(__self__, "certificate_authority", certificate_authority)
+        if cluster_name is not None:
+            pulumi.set(__self__, "cluster_name", cluster_name)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if endpoint is not None:
+            pulumi.set(__self__, "endpoint", endpoint)
+        if healthcheck_namespace is not None:
+            pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if region is not None:
+            pulumi.set(__self__, "region", region)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if role_arn is not None:
+            pulumi.set(__self__, "role_arn", role_arn)
+        if role_external_id is not None:
+            pulumi.set(__self__, "role_external_id", role_external_id)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="certificateAuthority")
+    def certificate_authority(self) -> Optional[str]:
+        return pulumi.get(self, "certificate_authority")
+
+    @property
+    @pulumi.getter(name="clusterName")
+    def cluster_name(self) -> Optional[str]:
+        return pulumi.get(self, "cluster_name")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def endpoint(self) -> Optional[str]:
+        return pulumi.get(self, "endpoint")
+
+    @property
+    @pulumi.getter(name="healthcheckNamespace")
+    def healthcheck_namespace(self) -> Optional[str]:
+        """
+        The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        """
+        return pulumi.get(self, "healthcheck_namespace")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def region(self) -> Optional[str]:
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[str]:
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[str]:
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @property
+    @pulumi.getter(name="roleArn")
+    def role_arn(self) -> Optional[str]:
+        return pulumi.get(self, "role_arn")
+
+    @property
+    @pulumi.getter(name="roleExternalId")
+    def role_external_id(self) -> Optional[str]:
+        return pulumi.get(self, "role_external_id")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class GetResourceResourceAmazonEksInstanceProfileUserImpersonationResult(dict):
+    def __init__(__self__, *,
+                 bind_interface: Optional[str] = None,
+                 certificate_authority: Optional[str] = None,
+                 cluster_name: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 endpoint: Optional[str] = None,
+                 healthcheck_namespace: Optional[str] = None,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None,
+                 region: Optional[str] = None,
+                 remote_identity_group_id: Optional[str] = None,
+                 remote_identity_healthcheck_username: Optional[str] = None,
+                 role_arn: Optional[str] = None,
+                 role_external_id: Optional[str] = None,
+                 secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str bind_interface: Bind interface
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        :param str id: Unique identifier of the Resource.
+        :param str name: Unique human-readable name of the Resource.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if certificate_authority is not None:
+            pulumi.set(__self__, "certificate_authority", certificate_authority)
+        if cluster_name is not None:
+            pulumi.set(__self__, "cluster_name", cluster_name)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if endpoint is not None:
+            pulumi.set(__self__, "endpoint", endpoint)
+        if healthcheck_namespace is not None:
+            pulumi.set(__self__, "healthcheck_namespace", healthcheck_namespace)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if region is not None:
+            pulumi.set(__self__, "region", region)
+        if remote_identity_group_id is not None:
+            pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
+        if remote_identity_healthcheck_username is not None:
+            pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
+        if role_arn is not None:
+            pulumi.set(__self__, "role_arn", role_arn)
+        if role_external_id is not None:
+            pulumi.set(__self__, "role_external_id", role_external_id)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter(name="certificateAuthority")
+    def certificate_authority(self) -> Optional[str]:
+        return pulumi.get(self, "certificate_authority")
+
+    @property
+    @pulumi.getter(name="clusterName")
+    def cluster_name(self) -> Optional[str]:
+        return pulumi.get(self, "cluster_name")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def endpoint(self) -> Optional[str]:
+        return pulumi.get(self, "endpoint")
+
+    @property
+    @pulumi.getter(name="healthcheckNamespace")
+    def healthcheck_namespace(self) -> Optional[str]:
+        """
+        The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
+        """
+        return pulumi.get(self, "healthcheck_namespace")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def region(self) -> Optional[str]:
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter(name="remoteIdentityGroupId")
+    def remote_identity_group_id(self) -> Optional[str]:
+        return pulumi.get(self, "remote_identity_group_id")
+
+    @property
+    @pulumi.getter(name="remoteIdentityHealthcheckUsername")
+    def remote_identity_healthcheck_username(self) -> Optional[str]:
+        return pulumi.get(self, "remote_identity_healthcheck_username")
+
+    @property
+    @pulumi.getter(name="roleArn")
+    def role_arn(self) -> Optional[str]:
+        return pulumi.get(self, "role_arn")
+
+    @property
+    @pulumi.getter(name="roleExternalId")
+    def role_external_id(self) -> Optional[str]:
+        return pulumi.get(self, "role_external_id")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -16829,22 +19082,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  region: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
@@ -16867,14 +19122,16 @@
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
@@ -16960,14 +19217,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -16979,23 +19244,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -17008,14 +19275,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -17077,14 +19346,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -17109,21 +19386,23 @@
                  output: Optional[str] = None,
                  port_override: Optional[int] = None,
                  region: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -17142,14 +19421,16 @@
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
@@ -17222,14 +19503,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -17242,22 +19531,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -17272,14 +19563,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -17344,14 +19637,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -17370,22 +19671,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -17402,14 +19705,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -17479,14 +19784,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -17634,14 +19947,15 @@
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if enable_env_variables is not None:
@@ -17750,14 +20064,17 @@
     @pulumi.getter(name="sessionExpiry")
     def session_expiry(self) -> Optional[int]:
         return pulumi.get(self, "session_expiry")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -17786,14 +20103,15 @@
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -17909,14 +20227,17 @@
     @pulumi.getter(name="sessionExpiry")
     def session_expiry(self) -> Optional[int]:
         return pulumi.get(self, "session_expiry")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -17939,15 +20260,15 @@
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_id: * azure_postgres:
+        :param str tenant_id: * azure_mysql:
         """
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -18022,15 +20343,15 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         """
-        * azure_postgres:
+        * azure_mysql:
         """
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
 class GetResourceResourceAzureCertificateResult(dict):
     def __init__(__self__, *,
@@ -18046,15 +20367,15 @@
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
-        :param str tenant_id: * azure_postgres:
+        :param str tenant_id: * azure_mysql:
         """
         if app_id is not None:
             pulumi.set(__self__, "app_id", app_id)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if client_certificate is not None:
             pulumi.set(__self__, "client_certificate", client_certificate)
@@ -18129,41 +20450,182 @@
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
         """
-        * azure_postgres:
+        * azure_mysql:
         """
         return pulumi.get(self, "tenant_id")
 
 
 @pulumi.output_type
+class GetResourceResourceAzureMysqlResult(dict):
+    def __init__(__self__, *,
+                 bind_interface: Optional[str] = None,
+                 database: Optional[str] = None,
+                 egress_filter: Optional[str] = None,
+                 hostname: Optional[str] = None,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None,
+                 password: Optional[str] = None,
+                 port: Optional[int] = None,
+                 port_override: Optional[int] = None,
+                 secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 username: Optional[str] = None):
+        """
+        :param str bind_interface: Bind interface
+        :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
+        :param str id: Unique identifier of the Resource.
+        :param str name: Unique human-readable name of the Resource.
+        :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if bind_interface is not None:
+            pulumi.set(__self__, "bind_interface", bind_interface)
+        if database is not None:
+            pulumi.set(__self__, "database", database)
+        if egress_filter is not None:
+            pulumi.set(__self__, "egress_filter", egress_filter)
+        if hostname is not None:
+            pulumi.set(__self__, "hostname", hostname)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if port_override is not None:
+            pulumi.set(__self__, "port_override", port_override)
+        if secret_store_id is not None:
+            pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
+
+    @property
+    @pulumi.getter(name="bindInterface")
+    def bind_interface(self) -> Optional[str]:
+        """
+        Bind interface
+        """
+        return pulumi.get(self, "bind_interface")
+
+    @property
+    @pulumi.getter
+    def database(self) -> Optional[str]:
+        return pulumi.get(self, "database")
+
+    @property
+    @pulumi.getter(name="egressFilter")
+    def egress_filter(self) -> Optional[str]:
+        """
+        A filter applied to the routing logic to pin datasource to nodes.
+        """
+        return pulumi.get(self, "egress_filter")
+
+    @property
+    @pulumi.getter
+    def hostname(self) -> Optional[str]:
+        return pulumi.get(self, "hostname")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the Resource.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the Resource.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[str]:
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[int]:
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="portOverride")
+    def port_override(self) -> Optional[int]:
+        return pulumi.get(self, "port_override")
+
+    @property
+    @pulumi.getter(name="secretStoreId")
+    def secret_store_id(self) -> Optional[str]:
+        """
+        ID of the secret store containing credentials for this resource, if any.
+        """
+        return pulumi.get(self, "secret_store_id")
+
+    @property
+    @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
+
+
+@pulumi.output_type
 class GetResourceResourceAzurePostgreResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
                  database: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -18180,14 +20642,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -18257,14 +20721,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -18281,22 +20753,24 @@
                  endpoint: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port_override: Optional[int] = None,
                  private_key: Optional[str] = None,
                  project: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if endpoint is not None:
@@ -18309,14 +20783,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if private_key is not None:
             pulumi.set(__self__, "private_key", private_key)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -18376,14 +20852,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -18400,23 +20884,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -18429,14 +20915,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -18498,14 +20986,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -18529,22 +21025,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -18561,14 +21059,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -18638,14 +21138,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -18663,22 +21171,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -18693,14 +21203,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -18765,14 +21277,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -18791,22 +21311,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -18823,14 +21345,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -18900,14 +21424,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -18924,23 +21456,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -18953,14 +21487,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -19022,14 +21558,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -19052,22 +21596,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -19082,14 +21628,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -19154,14 +21702,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -19179,22 +21735,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -19209,14 +21767,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
@@ -19281,14 +21841,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -19307,22 +21875,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if connect_to_replica is not None:
@@ -19339,14 +21909,16 @@
             pulumi.set(__self__, "password", password)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if replica_set is not None:
             pulumi.set(__self__, "replica_set", replica_set)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authDatabase")
@@ -19416,14 +21988,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -19440,22 +22020,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -19468,14 +22050,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -19535,14 +22119,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -19562,21 +22154,23 @@
                  name: Optional[str] = None,
                  port_override: Optional[int] = None,
                  region: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -19595,14 +22189,16 @@
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
@@ -19675,14 +22271,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -19694,23 +22298,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -19723,14 +22329,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -19792,14 +22400,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -19821,22 +22437,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
-                 tls_required: Optional[bool] = None):
+                 tls_required: Optional[bool] = None,
+                 username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -19849,18 +22468,22 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
         Bind interface
         """
@@ -19916,25 +22539,38 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter(name="tlsRequired")
     def tls_required(self) -> Optional[bool]:
         return pulumi.get(self, "tls_required")
 
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
+
 
 @pulumi.output_type
 class GetResourceResourceGcpResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
                  egress_filter: Optional[str] = None,
                  id: Optional[str] = None,
@@ -20037,22 +22673,24 @@
                  healthcheck_namespace: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if egress_filter is not None:
@@ -20069,14 +22707,16 @@
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -20147,14 +22787,22 @@
     @property
     @pulumi.getter(name="serviceAccountKey")
     def service_account_key(self) -> Optional[str]:
         return pulumi.get(self, "service_account_key")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -20166,22 +22814,24 @@
                  egress_filter: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  healthcheck_namespace: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
                  service_account_key: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if egress_filter is not None:
@@ -20194,14 +22844,16 @@
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if service_account_key is not None:
             pulumi.set(__self__, "service_account_key", service_account_key)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -20262,14 +22914,22 @@
     @property
     @pulumi.getter(name="serviceAccountKey")
     def service_account_key(self) -> Optional[str]:
         return pulumi.get(self, "service_account_key")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -20283,22 +22943,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -20315,14 +22977,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -20392,14 +23056,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -20426,14 +23098,15 @@
                  url: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str url: * kubernetes:
         """
         if auth_header is not None:
             pulumi.set(__self__, "auth_header", auth_header)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -20524,14 +23197,17 @@
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -20566,14 +23242,15 @@
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str url: * kubernetes:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if default_path is not None:
             pulumi.set(__self__, "default_path", default_path)
@@ -20666,14 +23343,17 @@
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -20711,14 +23391,15 @@
                  url: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str url: * kubernetes:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if default_path is not None:
             pulumi.set(__self__, "default_path", default_path)
@@ -20802,14 +23483,17 @@
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -20838,22 +23522,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if client_certificate is not None:
@@ -20876,14 +23562,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if remote_identity_group_id is not None:
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -20969,14 +23657,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -20989,23 +23685,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_namespace is not None:
@@ -21020,14 +23718,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -21095,14 +23795,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -21121,23 +23829,25 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str token: * kubernetes_user_impersonation:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -21155,14 +23865,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if remote_identity_group_id is not None:
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -21235,14 +23947,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -21262,23 +23982,25 @@
                  healthcheck_namespace: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  token: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         :param str token: * kubernetes_user_impersonation:
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
@@ -21292,14 +24014,16 @@
             pulumi.set(__self__, "name", name)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if token is not None:
             pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -21362,14 +24086,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -21392,22 +24124,24 @@
                  healthcheck_namespace: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str healthcheck_namespace: The path used to check the health of your connection.  Defaults to `default`.  This field is required, and is only marked as optional for backwards compatibility.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if client_certificate is not None:
@@ -21426,14 +24160,16 @@
             pulumi.set(__self__, "name", name)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -21509,14 +24245,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -21529,22 +24273,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -21559,14 +24305,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -21631,14 +24379,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -21654,21 +24410,23 @@
                  egress_filter: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -21679,14 +24437,16 @@
             pulumi.set(__self__, "name", name)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -21739,14 +24499,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -21759,22 +24527,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -21789,14 +24559,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -21861,14 +24633,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -21886,23 +24666,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -21917,14 +24699,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -21991,14 +24775,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -22022,23 +24814,25 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -22055,14 +24849,16 @@
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if replica_set is not None:
             pulumi.set(__self__, "replica_set", replica_set)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -22134,14 +24930,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -22166,23 +24970,25 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if connect_to_replica is not None:
@@ -22201,14 +25007,16 @@
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if replica_set is not None:
             pulumi.set(__self__, "replica_set", replica_set)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -22285,14 +25093,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -22317,23 +25133,25 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  replica_set: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if connect_to_replica is not None:
@@ -22352,14 +25170,16 @@
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if replica_set is not None:
             pulumi.set(__self__, "replica_set", replica_set)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -22436,14 +25256,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -22465,23 +25293,25 @@
                  egress_filter: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if auth_database is not None:
             pulumi.set(__self__, "auth_database", auth_database)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -22494,14 +25324,16 @@
             pulumi.set(__self__, "name", name)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -22563,14 +25395,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -22597,22 +25437,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  server_name: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if client_certificate is not None:
@@ -22635,14 +25477,16 @@
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if server_name is not None:
             pulumi.set(__self__, "server_name", server_name)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -22727,14 +25571,22 @@
     @property
     @pulumi.getter(name="serverName")
     def server_name(self) -> Optional[str]:
         return pulumi.get(self, "server_name")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -22757,22 +25609,24 @@
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
                  server_name: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if certificate_authority is not None:
             pulumi.set(__self__, "certificate_authority", certificate_authority)
         if client_certificate is not None:
@@ -22797,14 +25651,16 @@
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
         if server_name is not None:
             pulumi.set(__self__, "server_name", server_name)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -22894,14 +25750,22 @@
     @property
     @pulumi.getter(name="serverName")
     def server_name(self) -> Optional[str]:
         return pulumi.get(self, "server_name")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -22919,22 +25783,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -22949,14 +25815,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -23021,14 +25889,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -23044,21 +25920,23 @@
                  egress_filter: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if endpoint is not None:
@@ -23069,14 +25947,16 @@
             pulumi.set(__self__, "name", name)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -23129,14 +26009,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -23152,21 +26040,23 @@
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  region: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  role_external_id: Optional[str] = None,
                  secret_access_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -23187,14 +26077,16 @@
             pulumi.set(__self__, "role_arn", role_arn)
         if role_external_id is not None:
             pulumi.set(__self__, "role_external_id", role_external_id)
         if secret_access_key is not None:
             pulumi.set(__self__, "secret_access_key", secret_access_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
         return pulumi.get(self, "access_key")
@@ -23272,14 +26164,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -23292,23 +26192,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -23323,14 +26225,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -23397,14 +26301,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -23428,22 +26340,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -23460,14 +26374,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -23537,14 +26453,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -23562,23 +26486,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -23593,14 +26519,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -23667,14 +26595,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -23696,23 +26632,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  tls_required: Optional[bool] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -23725,14 +26663,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if tls_required is not None:
             pulumi.set(__self__, "tls_required", tls_required)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
@@ -23794,14 +26734,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -23822,21 +26770,23 @@
                  egress_filter: Optional[str] = None,
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -23847,14 +26797,16 @@
             pulumi.set(__self__, "name", name)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
@@ -23907,14 +26859,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
 
@@ -23927,22 +26887,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if downgrade_nla_connections is not None:
             pulumi.set(__self__, "downgrade_nla_connections", downgrade_nla_connections)
         if egress_filter is not None:
@@ -23957,14 +26919,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -24029,14 +26993,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -24053,21 +27025,25 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
-                 tags: Optional[Mapping[str, str]] = None):
+                 subdomain: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None,
+                 tls_required: Optional[bool] = None,
+                 username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -24080,16 +27056,22 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
+        if tls_required is not None:
+            pulumi.set(__self__, "tls_required", tls_required)
+        if username is not None:
+            pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
     def bind_interface(self) -> Optional[str]:
         """
         Bind interface
         """
@@ -24145,20 +27127,38 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
+    @property
+    @pulumi.getter(name="tlsRequired")
+    def tls_required(self) -> Optional[bool]:
+        return pulumi.get(self, "tls_required")
+
+    @property
+    @pulumi.getter
+    def username(self) -> Optional[str]:
+        return pulumi.get(self, "username")
+
 
 @pulumi.output_type
 class GetResourceResourceRedshiftResult(dict):
     def __init__(__self__, *,
                  bind_interface: Optional[str] = None,
                  database: Optional[str] = None,
                  egress_filter: Optional[str] = None,
@@ -24166,22 +27166,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -24198,14 +27200,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -24275,14 +27279,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -24300,22 +27312,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -24330,14 +27344,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -24402,14 +27418,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -24427,22 +27451,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port_override: Optional[int] = None,
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -24457,14 +27483,16 @@
             pulumi.set(__self__, "password", password)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if schema is not None:
             pulumi.set(__self__, "schema", schema)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -24529,14 +27557,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -24560,14 +27596,15 @@
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if healthcheck_username is not None:
@@ -24641,14 +27678,17 @@
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
     def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
         return pulumi.get(self, "subdomain")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
@@ -24667,22 +27707,24 @@
                  name: Optional[str] = None,
                  override_database: Optional[bool] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  schema: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if database is not None:
             pulumi.set(__self__, "database", database)
         if egress_filter is not None:
@@ -24701,14 +27743,16 @@
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if schema is not None:
             pulumi.set(__self__, "schema", schema)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -24783,14 +27827,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -24810,22 +27862,24 @@
                  id: Optional[str] = None,
                  key_type: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_forwarding: Optional[bool] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         pulumi.set(__self__, "public_key", public_key)
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
@@ -24843,14 +27897,16 @@
             pulumi.set(__self__, "port", port)
         if port_forwarding is not None:
             pulumi.set(__self__, "port_forwarding", port_forwarding)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="publicKey")
@@ -24925,14 +27981,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -24953,22 +28017,24 @@
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_forwarding: Optional[bool] = None,
                  port_override: Optional[int] = None,
                  remote_identity_group_id: Optional[str] = None,
                  remote_identity_healthcheck_username: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -24989,14 +28055,16 @@
             pulumi.set(__self__, "port_override", port_override)
         if remote_identity_group_id is not None:
             pulumi.set(__self__, "remote_identity_group_id", remote_identity_group_id)
         if remote_identity_healthcheck_username is not None:
             pulumi.set(__self__, "remote_identity_healthcheck_username", remote_identity_healthcheck_username)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="allowDeprecatedKeyExchanges")
@@ -25076,14 +28144,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -25102,22 +28178,24 @@
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  port: Optional[int] = None,
                  port_forwarding: Optional[bool] = None,
                  port_override: Optional[int] = None,
                  private_key: Optional[str] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if allow_deprecated_key_exchanges is not None:
             pulumi.set(__self__, "allow_deprecated_key_exchanges", allow_deprecated_key_exchanges)
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
@@ -25134,14 +28212,16 @@
             pulumi.set(__self__, "port_forwarding", port_forwarding)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if private_key is not None:
             pulumi.set(__self__, "private_key", private_key)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="allowDeprecatedKeyExchanges")
@@ -25211,14 +28291,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -25235,22 +28323,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -25263,14 +28353,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -25330,14 +28422,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -25354,22 +28454,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -25382,14 +28484,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -25449,14 +28553,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -25473,22 +28585,24 @@
                  hostname: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  password: Optional[str] = None,
                  port: Optional[int] = None,
                  port_override: Optional[int] = None,
                  secret_store_id: Optional[str] = None,
+                 subdomain: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None,
                  username: Optional[str] = None):
         """
         :param str bind_interface: Bind interface
         :param str egress_filter: A filter applied to the routing logic to pin datasource to nodes.
         :param str id: Unique identifier of the Resource.
         :param str name: Unique human-readable name of the Resource.
         :param str secret_store_id: ID of the secret store containing credentials for this resource, if any.
+        :param str subdomain: Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if bind_interface is not None:
             pulumi.set(__self__, "bind_interface", bind_interface)
         if egress_filter is not None:
             pulumi.set(__self__, "egress_filter", egress_filter)
         if hostname is not None:
@@ -25501,14 +28615,16 @@
             pulumi.set(__self__, "password", password)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if port_override is not None:
             pulumi.set(__self__, "port_override", port_override)
         if secret_store_id is not None:
             pulumi.set(__self__, "secret_store_id", secret_store_id)
+        if subdomain is not None:
+            pulumi.set(__self__, "subdomain", subdomain)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="bindInterface")
@@ -25568,14 +28684,22 @@
         """
         ID of the secret store containing credentials for this resource, if any.
         """
         return pulumi.get(self, "secret_store_id")
 
     @property
     @pulumi.getter
+    def subdomain(self) -> Optional[str]:
+        """
+        Subdomain is the local DNS address.  (e.g. app-prod1 turns into app-prod1.your-org-name.sdm.network)
+        """
+        return pulumi.get(self, "subdomain")
+
+    @property
+    @pulumi.getter
     def tags(self) -> Optional[Mapping[str, str]]:
         """
         Tags is a map of key, value pairs.
         """
         return pulumi.get(self, "tags")
 
     @property
@@ -25583,34 +28707,45 @@
     def username(self) -> Optional[str]:
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class GetRoleRoleResult(dict):
     def __init__(__self__, *,
+                 managed_by: str,
                  access_rules: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
+        :param str managed_by: Managed By is a read only field for what service manages this role, e.g. StrongDM, Okta, Azure.
         :param str access_rules: AccessRules is a list of access rules defining the resources this Role has access to.
         :param str id: Unique identifier of the Role.
         :param str name: Unique human-readable name of the Role.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
+        pulumi.set(__self__, "managed_by", managed_by)
         if access_rules is not None:
             pulumi.set(__self__, "access_rules", access_rules)
         if id is not None:
             pulumi.set(__self__, "id", id)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
+    @pulumi.getter(name="managedBy")
+    def managed_by(self) -> str:
+        """
+        Managed By is a read only field for what service manages this role, e.g. StrongDM, Okta, Azure.
+        """
+        return pulumi.get(self, "managed_by")
+
+    @property
     @pulumi.getter(name="accessRules")
     def access_rules(self) -> Optional[str]:
         """
         AccessRules is a list of access rules defining the resources this Role has access to.
         """
         return pulumi.get(self, "access_rules")
 
@@ -25642,23 +28777,25 @@
 @pulumi.output_type
 class GetSecretStoreSecretStoreResult(dict):
     def __init__(__self__, *,
                  aws: Sequence['outputs.GetSecretStoreSecretStoreAwResult'],
                  azure_stores: Sequence['outputs.GetSecretStoreSecretStoreAzureStoreResult'],
                  cyberark_conjurs: Sequence['outputs.GetSecretStoreSecretStoreCyberarkConjurResult'],
                  cyberark_pam_experimentals: Sequence['outputs.GetSecretStoreSecretStoreCyberarkPamExperimentalResult'],
+                 cyberark_pams: Sequence['outputs.GetSecretStoreSecretStoreCyberarkPamResult'],
                  delinea_stores: Sequence['outputs.GetSecretStoreSecretStoreDelineaStoreResult'],
                  gcp_stores: Sequence['outputs.GetSecretStoreSecretStoreGcpStoreResult'],
                  vault_approles: Sequence['outputs.GetSecretStoreSecretStoreVaultApproleResult'],
                  vault_tls: Sequence['outputs.GetSecretStoreSecretStoreVaultTlResult'],
                  vault_tokens: Sequence['outputs.GetSecretStoreSecretStoreVaultTokenResult']):
         pulumi.set(__self__, "aws", aws)
         pulumi.set(__self__, "azure_stores", azure_stores)
         pulumi.set(__self__, "cyberark_conjurs", cyberark_conjurs)
         pulumi.set(__self__, "cyberark_pam_experimentals", cyberark_pam_experimentals)
+        pulumi.set(__self__, "cyberark_pams", cyberark_pams)
         pulumi.set(__self__, "delinea_stores", delinea_stores)
         pulumi.set(__self__, "gcp_stores", gcp_stores)
         pulumi.set(__self__, "vault_approles", vault_approles)
         pulumi.set(__self__, "vault_tls", vault_tls)
         pulumi.set(__self__, "vault_tokens", vault_tokens)
 
     @property
@@ -25678,14 +28815,19 @@
 
     @property
     @pulumi.getter(name="cyberarkPamExperimentals")
     def cyberark_pam_experimentals(self) -> Sequence['outputs.GetSecretStoreSecretStoreCyberarkPamExperimentalResult']:
         return pulumi.get(self, "cyberark_pam_experimentals")
 
     @property
+    @pulumi.getter(name="cyberarkPams")
+    def cyberark_pams(self) -> Sequence['outputs.GetSecretStoreSecretStoreCyberarkPamResult']:
+        return pulumi.get(self, "cyberark_pams")
+
+    @property
     @pulumi.getter(name="delineaStores")
     def delinea_stores(self) -> Sequence['outputs.GetSecretStoreSecretStoreDelineaStoreResult']:
         return pulumi.get(self, "delinea_stores")
 
     @property
     @pulumi.getter(name="gcpStores")
     def gcp_stores(self) -> Sequence['outputs.GetSecretStoreSecretStoreGcpStoreResult']:
@@ -25818,14 +28960,65 @@
     def __init__(__self__, *,
                  app_url: Optional[str] = None,
                  id: Optional[str] = None,
                  name: Optional[str] = None,
                  tags: Optional[Mapping[str, str]] = None):
         """
         :param str id: Unique identifier of the SecretStore.
+        :param str name: Unique human-readable name of the SecretStore.
+        :param Mapping[str, str] tags: Tags is a map of key, value pairs.
+        """
+        if app_url is not None:
+            pulumi.set(__self__, "app_url", app_url)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
+
+    @property
+    @pulumi.getter(name="appUrl")
+    def app_url(self) -> Optional[str]:
+        return pulumi.get(self, "app_url")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        """
+        Unique identifier of the SecretStore.
+        """
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        """
+        Unique human-readable name of the SecretStore.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[Mapping[str, str]]:
+        """
+        Tags is a map of key, value pairs.
+        """
+        return pulumi.get(self, "tags")
+
+
+@pulumi.output_type
+class GetSecretStoreSecretStoreCyberarkPamResult(dict):
+    def __init__(__self__, *,
+                 app_url: Optional[str] = None,
+                 id: Optional[str] = None,
+                 name: Optional[str] = None,
+                 tags: Optional[Mapping[str, str]] = None):
+        """
+        :param str id: Unique identifier of the SecretStore.
         :param str name: Unique human-readable name of the SecretStore.
         :param Mapping[str, str] tags: Tags is a map of key, value pairs.
         """
         if app_url is not None:
             pulumi.set(__self__, "app_url", app_url)
         if id is not None:
             pulumi.set(__self__, "id", id)
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/provider.py` & `pulumi_sdm-0.4.0/pulumi_sdm/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/remote_identity.py` & `pulumi_sdm-0.4.0/pulumi_sdm/remote_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/resource.py` & `pulumi_sdm-0.4.0/pulumi_sdm/resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,25 +18,28 @@
     def __init__(__self__, *,
                  aks: Optional[pulumi.Input['ResourceAksArgs']] = None,
                  aks_basic_auth: Optional[pulumi.Input['ResourceAksBasicAuthArgs']] = None,
                  aks_service_account: Optional[pulumi.Input['ResourceAksServiceAccountArgs']] = None,
                  aks_service_account_user_impersonation: Optional[pulumi.Input['ResourceAksServiceAccountUserImpersonationArgs']] = None,
                  aks_user_impersonation: Optional[pulumi.Input['ResourceAksUserImpersonationArgs']] = None,
                  amazon_eks: Optional[pulumi.Input['ResourceAmazonEksArgs']] = None,
+                 amazon_eks_instance_profile: Optional[pulumi.Input['ResourceAmazonEksInstanceProfileArgs']] = None,
+                 amazon_eks_instance_profile_user_impersonation: Optional[pulumi.Input['ResourceAmazonEksInstanceProfileUserImpersonationArgs']] = None,
                  amazon_eks_user_impersonation: Optional[pulumi.Input['ResourceAmazonEksUserImpersonationArgs']] = None,
                  amazon_es: Optional[pulumi.Input['ResourceAmazonEsArgs']] = None,
                  amazonmq_amqp091: Optional[pulumi.Input['ResourceAmazonmqAmqp091Args']] = None,
                  athena: Optional[pulumi.Input['ResourceAthenaArgs']] = None,
                  aurora_mysql: Optional[pulumi.Input['ResourceAuroraMysqlArgs']] = None,
                  aurora_postgres: Optional[pulumi.Input['ResourceAuroraPostgresArgs']] = None,
                  aws: Optional[pulumi.Input['ResourceAwsArgs']] = None,
                  aws_console: Optional[pulumi.Input['ResourceAwsConsoleArgs']] = None,
                  aws_console_static_key_pair: Optional[pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs']] = None,
                  azure: Optional[pulumi.Input['ResourceAzureArgs']] = None,
                  azure_certificate: Optional[pulumi.Input['ResourceAzureCertificateArgs']] = None,
+                 azure_mysql: Optional[pulumi.Input['ResourceAzureMysqlArgs']] = None,
                  azure_postgres: Optional[pulumi.Input['ResourceAzurePostgresArgs']] = None,
                  big_query: Optional[pulumi.Input['ResourceBigQueryArgs']] = None,
                  cassandra: Optional[pulumi.Input['ResourceCassandraArgs']] = None,
                  citus: Optional[pulumi.Input['ResourceCitusArgs']] = None,
                  clustrix: Optional[pulumi.Input['ResourceClustrixArgs']] = None,
                  cockroach: Optional[pulumi.Input['ResourceCockroachArgs']] = None,
                  db2_i: Optional[pulumi.Input['ResourceDb2IArgs']] = None,
@@ -91,33 +94,37 @@
                  sybase_iq: Optional[pulumi.Input['ResourceSybaseIqArgs']] = None,
                  teradata: Optional[pulumi.Input['ResourceTeradataArgs']] = None):
         """
         The set of arguments for constructing a Resource resource.
         :param pulumi.Input['ResourceAwsConsoleArgs'] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs'] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
+        :param pulumi.Input['ResourceAzureMysqlArgs'] azure_mysql: AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoHostArgs'] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoReplicaSetArgs'] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoShardedClusterArgs'] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMtlsMysqlArgs'] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        :param pulumi.Input['ResourceOracleArgs'] oracle: Oracle is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceSnowsightArgs'] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         if aks is not None:
             pulumi.set(__self__, "aks", aks)
         if aks_basic_auth is not None:
             pulumi.set(__self__, "aks_basic_auth", aks_basic_auth)
         if aks_service_account is not None:
             pulumi.set(__self__, "aks_service_account", aks_service_account)
         if aks_service_account_user_impersonation is not None:
             pulumi.set(__self__, "aks_service_account_user_impersonation", aks_service_account_user_impersonation)
         if aks_user_impersonation is not None:
             pulumi.set(__self__, "aks_user_impersonation", aks_user_impersonation)
         if amazon_eks is not None:
             pulumi.set(__self__, "amazon_eks", amazon_eks)
+        if amazon_eks_instance_profile is not None:
+            pulumi.set(__self__, "amazon_eks_instance_profile", amazon_eks_instance_profile)
+        if amazon_eks_instance_profile_user_impersonation is not None:
+            pulumi.set(__self__, "amazon_eks_instance_profile_user_impersonation", amazon_eks_instance_profile_user_impersonation)
         if amazon_eks_user_impersonation is not None:
             pulumi.set(__self__, "amazon_eks_user_impersonation", amazon_eks_user_impersonation)
         if amazon_es is not None:
             pulumi.set(__self__, "amazon_es", amazon_es)
         if amazonmq_amqp091 is not None:
             pulumi.set(__self__, "amazonmq_amqp091", amazonmq_amqp091)
         if athena is not None:
@@ -132,14 +139,16 @@
             pulumi.set(__self__, "aws_console", aws_console)
         if aws_console_static_key_pair is not None:
             pulumi.set(__self__, "aws_console_static_key_pair", aws_console_static_key_pair)
         if azure is not None:
             pulumi.set(__self__, "azure", azure)
         if azure_certificate is not None:
             pulumi.set(__self__, "azure_certificate", azure_certificate)
+        if azure_mysql is not None:
+            pulumi.set(__self__, "azure_mysql", azure_mysql)
         if azure_postgres is not None:
             pulumi.set(__self__, "azure_postgres", azure_postgres)
         if big_query is not None:
             pulumi.set(__self__, "big_query", big_query)
         if cassandra is not None:
             pulumi.set(__self__, "cassandra", cassandra)
         if citus is not None:
@@ -302,14 +311,32 @@
         return pulumi.get(self, "amazon_eks")
 
     @amazon_eks.setter
     def amazon_eks(self, value: Optional[pulumi.Input['ResourceAmazonEksArgs']]):
         pulumi.set(self, "amazon_eks", value)
 
     @property
+    @pulumi.getter(name="amazonEksInstanceProfile")
+    def amazon_eks_instance_profile(self) -> Optional[pulumi.Input['ResourceAmazonEksInstanceProfileArgs']]:
+        return pulumi.get(self, "amazon_eks_instance_profile")
+
+    @amazon_eks_instance_profile.setter
+    def amazon_eks_instance_profile(self, value: Optional[pulumi.Input['ResourceAmazonEksInstanceProfileArgs']]):
+        pulumi.set(self, "amazon_eks_instance_profile", value)
+
+    @property
+    @pulumi.getter(name="amazonEksInstanceProfileUserImpersonation")
+    def amazon_eks_instance_profile_user_impersonation(self) -> Optional[pulumi.Input['ResourceAmazonEksInstanceProfileUserImpersonationArgs']]:
+        return pulumi.get(self, "amazon_eks_instance_profile_user_impersonation")
+
+    @amazon_eks_instance_profile_user_impersonation.setter
+    def amazon_eks_instance_profile_user_impersonation(self, value: Optional[pulumi.Input['ResourceAmazonEksInstanceProfileUserImpersonationArgs']]):
+        pulumi.set(self, "amazon_eks_instance_profile_user_impersonation", value)
+
+    @property
     @pulumi.getter(name="amazonEksUserImpersonation")
     def amazon_eks_user_impersonation(self) -> Optional[pulumi.Input['ResourceAmazonEksUserImpersonationArgs']]:
         return pulumi.get(self, "amazon_eks_user_impersonation")
 
     @amazon_eks_user_impersonation.setter
     def amazon_eks_user_impersonation(self, value: Optional[pulumi.Input['ResourceAmazonEksUserImpersonationArgs']]):
         pulumi.set(self, "amazon_eks_user_impersonation", value)
@@ -408,14 +435,26 @@
         return pulumi.get(self, "azure_certificate")
 
     @azure_certificate.setter
     def azure_certificate(self, value: Optional[pulumi.Input['ResourceAzureCertificateArgs']]):
         pulumi.set(self, "azure_certificate", value)
 
     @property
+    @pulumi.getter(name="azureMysql")
+    def azure_mysql(self) -> Optional[pulumi.Input['ResourceAzureMysqlArgs']]:
+        """
+        AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        """
+        return pulumi.get(self, "azure_mysql")
+
+    @azure_mysql.setter
+    def azure_mysql(self, value: Optional[pulumi.Input['ResourceAzureMysqlArgs']]):
+        pulumi.set(self, "azure_mysql", value)
+
+    @property
     @pulumi.getter(name="azurePostgres")
     def azure_postgres(self) -> Optional[pulumi.Input['ResourceAzurePostgresArgs']]:
         return pulumi.get(self, "azure_postgres")
 
     @azure_postgres.setter
     def azure_postgres(self, value: Optional[pulumi.Input['ResourceAzurePostgresArgs']]):
         pulumi.set(self, "azure_postgres", value)
@@ -773,17 +812,14 @@
     @neptune_iam.setter
     def neptune_iam(self, value: Optional[pulumi.Input['ResourceNeptuneIamArgs']]):
         pulumi.set(self, "neptune_iam", value)
 
     @property
     @pulumi.getter
     def oracle(self) -> Optional[pulumi.Input['ResourceOracleArgs']]:
-        """
-        Oracle is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "oracle")
 
     @oracle.setter
     def oracle(self, value: Optional[pulumi.Input['ResourceOracleArgs']]):
         pulumi.set(self, "oracle", value)
 
     @property
@@ -948,25 +984,28 @@
     def __init__(__self__, *,
                  aks: Optional[pulumi.Input['ResourceAksArgs']] = None,
                  aks_basic_auth: Optional[pulumi.Input['ResourceAksBasicAuthArgs']] = None,
                  aks_service_account: Optional[pulumi.Input['ResourceAksServiceAccountArgs']] = None,
                  aks_service_account_user_impersonation: Optional[pulumi.Input['ResourceAksServiceAccountUserImpersonationArgs']] = None,
                  aks_user_impersonation: Optional[pulumi.Input['ResourceAksUserImpersonationArgs']] = None,
                  amazon_eks: Optional[pulumi.Input['ResourceAmazonEksArgs']] = None,
+                 amazon_eks_instance_profile: Optional[pulumi.Input['ResourceAmazonEksInstanceProfileArgs']] = None,
+                 amazon_eks_instance_profile_user_impersonation: Optional[pulumi.Input['ResourceAmazonEksInstanceProfileUserImpersonationArgs']] = None,
                  amazon_eks_user_impersonation: Optional[pulumi.Input['ResourceAmazonEksUserImpersonationArgs']] = None,
                  amazon_es: Optional[pulumi.Input['ResourceAmazonEsArgs']] = None,
                  amazonmq_amqp091: Optional[pulumi.Input['ResourceAmazonmqAmqp091Args']] = None,
                  athena: Optional[pulumi.Input['ResourceAthenaArgs']] = None,
                  aurora_mysql: Optional[pulumi.Input['ResourceAuroraMysqlArgs']] = None,
                  aurora_postgres: Optional[pulumi.Input['ResourceAuroraPostgresArgs']] = None,
                  aws: Optional[pulumi.Input['ResourceAwsArgs']] = None,
                  aws_console: Optional[pulumi.Input['ResourceAwsConsoleArgs']] = None,
                  aws_console_static_key_pair: Optional[pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs']] = None,
                  azure: Optional[pulumi.Input['ResourceAzureArgs']] = None,
                  azure_certificate: Optional[pulumi.Input['ResourceAzureCertificateArgs']] = None,
+                 azure_mysql: Optional[pulumi.Input['ResourceAzureMysqlArgs']] = None,
                  azure_postgres: Optional[pulumi.Input['ResourceAzurePostgresArgs']] = None,
                  big_query: Optional[pulumi.Input['ResourceBigQueryArgs']] = None,
                  cassandra: Optional[pulumi.Input['ResourceCassandraArgs']] = None,
                  citus: Optional[pulumi.Input['ResourceCitusArgs']] = None,
                  clustrix: Optional[pulumi.Input['ResourceClustrixArgs']] = None,
                  cockroach: Optional[pulumi.Input['ResourceCockroachArgs']] = None,
                  db2_i: Optional[pulumi.Input['ResourceDb2IArgs']] = None,
@@ -1021,33 +1060,37 @@
                  sybase_iq: Optional[pulumi.Input['ResourceSybaseIqArgs']] = None,
                  teradata: Optional[pulumi.Input['ResourceTeradataArgs']] = None):
         """
         Input properties used for looking up and filtering Resource resources.
         :param pulumi.Input['ResourceAwsConsoleArgs'] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceAwsConsoleStaticKeyPairArgs'] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
+        :param pulumi.Input['ResourceAzureMysqlArgs'] azure_mysql: AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoHostArgs'] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoReplicaSetArgs'] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMongoShardedClusterArgs'] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceMtlsMysqlArgs'] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        :param pulumi.Input['ResourceOracleArgs'] oracle: Oracle is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['ResourceSnowsightArgs'] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         if aks is not None:
             pulumi.set(__self__, "aks", aks)
         if aks_basic_auth is not None:
             pulumi.set(__self__, "aks_basic_auth", aks_basic_auth)
         if aks_service_account is not None:
             pulumi.set(__self__, "aks_service_account", aks_service_account)
         if aks_service_account_user_impersonation is not None:
             pulumi.set(__self__, "aks_service_account_user_impersonation", aks_service_account_user_impersonation)
         if aks_user_impersonation is not None:
             pulumi.set(__self__, "aks_user_impersonation", aks_user_impersonation)
         if amazon_eks is not None:
             pulumi.set(__self__, "amazon_eks", amazon_eks)
+        if amazon_eks_instance_profile is not None:
+            pulumi.set(__self__, "amazon_eks_instance_profile", amazon_eks_instance_profile)
+        if amazon_eks_instance_profile_user_impersonation is not None:
+            pulumi.set(__self__, "amazon_eks_instance_profile_user_impersonation", amazon_eks_instance_profile_user_impersonation)
         if amazon_eks_user_impersonation is not None:
             pulumi.set(__self__, "amazon_eks_user_impersonation", amazon_eks_user_impersonation)
         if amazon_es is not None:
             pulumi.set(__self__, "amazon_es", amazon_es)
         if amazonmq_amqp091 is not None:
             pulumi.set(__self__, "amazonmq_amqp091", amazonmq_amqp091)
         if athena is not None:
@@ -1062,14 +1105,16 @@
             pulumi.set(__self__, "aws_console", aws_console)
         if aws_console_static_key_pair is not None:
             pulumi.set(__self__, "aws_console_static_key_pair", aws_console_static_key_pair)
         if azure is not None:
             pulumi.set(__self__, "azure", azure)
         if azure_certificate is not None:
             pulumi.set(__self__, "azure_certificate", azure_certificate)
+        if azure_mysql is not None:
+            pulumi.set(__self__, "azure_mysql", azure_mysql)
         if azure_postgres is not None:
             pulumi.set(__self__, "azure_postgres", azure_postgres)
         if big_query is not None:
             pulumi.set(__self__, "big_query", big_query)
         if cassandra is not None:
             pulumi.set(__self__, "cassandra", cassandra)
         if citus is not None:
@@ -1232,14 +1277,32 @@
         return pulumi.get(self, "amazon_eks")
 
     @amazon_eks.setter
     def amazon_eks(self, value: Optional[pulumi.Input['ResourceAmazonEksArgs']]):
         pulumi.set(self, "amazon_eks", value)
 
     @property
+    @pulumi.getter(name="amazonEksInstanceProfile")
+    def amazon_eks_instance_profile(self) -> Optional[pulumi.Input['ResourceAmazonEksInstanceProfileArgs']]:
+        return pulumi.get(self, "amazon_eks_instance_profile")
+
+    @amazon_eks_instance_profile.setter
+    def amazon_eks_instance_profile(self, value: Optional[pulumi.Input['ResourceAmazonEksInstanceProfileArgs']]):
+        pulumi.set(self, "amazon_eks_instance_profile", value)
+
+    @property
+    @pulumi.getter(name="amazonEksInstanceProfileUserImpersonation")
+    def amazon_eks_instance_profile_user_impersonation(self) -> Optional[pulumi.Input['ResourceAmazonEksInstanceProfileUserImpersonationArgs']]:
+        return pulumi.get(self, "amazon_eks_instance_profile_user_impersonation")
+
+    @amazon_eks_instance_profile_user_impersonation.setter
+    def amazon_eks_instance_profile_user_impersonation(self, value: Optional[pulumi.Input['ResourceAmazonEksInstanceProfileUserImpersonationArgs']]):
+        pulumi.set(self, "amazon_eks_instance_profile_user_impersonation", value)
+
+    @property
     @pulumi.getter(name="amazonEksUserImpersonation")
     def amazon_eks_user_impersonation(self) -> Optional[pulumi.Input['ResourceAmazonEksUserImpersonationArgs']]:
         return pulumi.get(self, "amazon_eks_user_impersonation")
 
     @amazon_eks_user_impersonation.setter
     def amazon_eks_user_impersonation(self, value: Optional[pulumi.Input['ResourceAmazonEksUserImpersonationArgs']]):
         pulumi.set(self, "amazon_eks_user_impersonation", value)
@@ -1338,14 +1401,26 @@
         return pulumi.get(self, "azure_certificate")
 
     @azure_certificate.setter
     def azure_certificate(self, value: Optional[pulumi.Input['ResourceAzureCertificateArgs']]):
         pulumi.set(self, "azure_certificate", value)
 
     @property
+    @pulumi.getter(name="azureMysql")
+    def azure_mysql(self) -> Optional[pulumi.Input['ResourceAzureMysqlArgs']]:
+        """
+        AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        """
+        return pulumi.get(self, "azure_mysql")
+
+    @azure_mysql.setter
+    def azure_mysql(self, value: Optional[pulumi.Input['ResourceAzureMysqlArgs']]):
+        pulumi.set(self, "azure_mysql", value)
+
+    @property
     @pulumi.getter(name="azurePostgres")
     def azure_postgres(self) -> Optional[pulumi.Input['ResourceAzurePostgresArgs']]:
         return pulumi.get(self, "azure_postgres")
 
     @azure_postgres.setter
     def azure_postgres(self, value: Optional[pulumi.Input['ResourceAzurePostgresArgs']]):
         pulumi.set(self, "azure_postgres", value)
@@ -1703,17 +1778,14 @@
     @neptune_iam.setter
     def neptune_iam(self, value: Optional[pulumi.Input['ResourceNeptuneIamArgs']]):
         pulumi.set(self, "neptune_iam", value)
 
     @property
     @pulumi.getter
     def oracle(self) -> Optional[pulumi.Input['ResourceOracleArgs']]:
-        """
-        Oracle is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "oracle")
 
     @oracle.setter
     def oracle(self, value: Optional[pulumi.Input['ResourceOracleArgs']]):
         pulumi.set(self, "oracle", value)
 
     @property
@@ -1880,25 +1952,28 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aks: Optional[pulumi.Input[pulumi.InputType['ResourceAksArgs']]] = None,
                  aks_basic_auth: Optional[pulumi.Input[pulumi.InputType['ResourceAksBasicAuthArgs']]] = None,
                  aks_service_account: Optional[pulumi.Input[pulumi.InputType['ResourceAksServiceAccountArgs']]] = None,
                  aks_service_account_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAksServiceAccountUserImpersonationArgs']]] = None,
                  aks_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAksUserImpersonationArgs']]] = None,
                  amazon_eks: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksArgs']]] = None,
+                 amazon_eks_instance_profile: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksInstanceProfileArgs']]] = None,
+                 amazon_eks_instance_profile_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksInstanceProfileUserImpersonationArgs']]] = None,
                  amazon_eks_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksUserImpersonationArgs']]] = None,
                  amazon_es: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEsArgs']]] = None,
                  amazonmq_amqp091: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonmqAmqp091Args']]] = None,
                  athena: Optional[pulumi.Input[pulumi.InputType['ResourceAthenaArgs']]] = None,
                  aurora_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAuroraMysqlArgs']]] = None,
                  aurora_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAuroraPostgresArgs']]] = None,
                  aws: Optional[pulumi.Input[pulumi.InputType['ResourceAwsArgs']]] = None,
                  aws_console: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']]] = None,
                  aws_console_static_key_pair: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']]] = None,
                  azure: Optional[pulumi.Input[pulumi.InputType['ResourceAzureArgs']]] = None,
                  azure_certificate: Optional[pulumi.Input[pulumi.InputType['ResourceAzureCertificateArgs']]] = None,
+                 azure_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']]] = None,
                  azure_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresArgs']]] = None,
                  big_query: Optional[pulumi.Input[pulumi.InputType['ResourceBigQueryArgs']]] = None,
                  cassandra: Optional[pulumi.Input[pulumi.InputType['ResourceCassandraArgs']]] = None,
                  citus: Optional[pulumi.Input[pulumi.InputType['ResourceCitusArgs']]] = None,
                  clustrix: Optional[pulumi.Input[pulumi.InputType['ResourceClustrixArgs']]] = None,
                  cockroach: Optional[pulumi.Input[pulumi.InputType['ResourceCockroachArgs']]] = None,
                  db2_i: Optional[pulumi.Input[pulumi.InputType['ResourceDb2IArgs']]] = None,
@@ -1963,19 +2038,19 @@
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
+        :param pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']] azure_mysql: AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoHostArgs']] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoReplicaSetArgs']] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoShardedClusterArgs']] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMtlsMysqlArgs']] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        :param pulumi.Input[pulumi.InputType['ResourceOracleArgs']] oracle: Oracle is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ResourceArgs] = None,
@@ -2006,25 +2081,28 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aks: Optional[pulumi.Input[pulumi.InputType['ResourceAksArgs']]] = None,
                  aks_basic_auth: Optional[pulumi.Input[pulumi.InputType['ResourceAksBasicAuthArgs']]] = None,
                  aks_service_account: Optional[pulumi.Input[pulumi.InputType['ResourceAksServiceAccountArgs']]] = None,
                  aks_service_account_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAksServiceAccountUserImpersonationArgs']]] = None,
                  aks_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAksUserImpersonationArgs']]] = None,
                  amazon_eks: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksArgs']]] = None,
+                 amazon_eks_instance_profile: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksInstanceProfileArgs']]] = None,
+                 amazon_eks_instance_profile_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksInstanceProfileUserImpersonationArgs']]] = None,
                  amazon_eks_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksUserImpersonationArgs']]] = None,
                  amazon_es: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEsArgs']]] = None,
                  amazonmq_amqp091: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonmqAmqp091Args']]] = None,
                  athena: Optional[pulumi.Input[pulumi.InputType['ResourceAthenaArgs']]] = None,
                  aurora_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAuroraMysqlArgs']]] = None,
                  aurora_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAuroraPostgresArgs']]] = None,
                  aws: Optional[pulumi.Input[pulumi.InputType['ResourceAwsArgs']]] = None,
                  aws_console: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']]] = None,
                  aws_console_static_key_pair: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']]] = None,
                  azure: Optional[pulumi.Input[pulumi.InputType['ResourceAzureArgs']]] = None,
                  azure_certificate: Optional[pulumi.Input[pulumi.InputType['ResourceAzureCertificateArgs']]] = None,
+                 azure_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']]] = None,
                  azure_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresArgs']]] = None,
                  big_query: Optional[pulumi.Input[pulumi.InputType['ResourceBigQueryArgs']]] = None,
                  cassandra: Optional[pulumi.Input[pulumi.InputType['ResourceCassandraArgs']]] = None,
                  citus: Optional[pulumi.Input[pulumi.InputType['ResourceCitusArgs']]] = None,
                  clustrix: Optional[pulumi.Input[pulumi.InputType['ResourceClustrixArgs']]] = None,
                  cockroach: Optional[pulumi.Input[pulumi.InputType['ResourceCockroachArgs']]] = None,
                  db2_i: Optional[pulumi.Input[pulumi.InputType['ResourceDb2IArgs']]] = None,
@@ -2089,25 +2167,28 @@
 
             __props__.__dict__["aks"] = aks
             __props__.__dict__["aks_basic_auth"] = aks_basic_auth
             __props__.__dict__["aks_service_account"] = aks_service_account
             __props__.__dict__["aks_service_account_user_impersonation"] = aks_service_account_user_impersonation
             __props__.__dict__["aks_user_impersonation"] = aks_user_impersonation
             __props__.__dict__["amazon_eks"] = amazon_eks
+            __props__.__dict__["amazon_eks_instance_profile"] = amazon_eks_instance_profile
+            __props__.__dict__["amazon_eks_instance_profile_user_impersonation"] = amazon_eks_instance_profile_user_impersonation
             __props__.__dict__["amazon_eks_user_impersonation"] = amazon_eks_user_impersonation
             __props__.__dict__["amazon_es"] = amazon_es
             __props__.__dict__["amazonmq_amqp091"] = amazonmq_amqp091
             __props__.__dict__["athena"] = athena
             __props__.__dict__["aurora_mysql"] = aurora_mysql
             __props__.__dict__["aurora_postgres"] = aurora_postgres
             __props__.__dict__["aws"] = aws
             __props__.__dict__["aws_console"] = aws_console
             __props__.__dict__["aws_console_static_key_pair"] = aws_console_static_key_pair
             __props__.__dict__["azure"] = azure
             __props__.__dict__["azure_certificate"] = azure_certificate
+            __props__.__dict__["azure_mysql"] = azure_mysql
             __props__.__dict__["azure_postgres"] = azure_postgres
             __props__.__dict__["big_query"] = big_query
             __props__.__dict__["cassandra"] = cassandra
             __props__.__dict__["citus"] = citus
             __props__.__dict__["clustrix"] = clustrix
             __props__.__dict__["cockroach"] = cockroach
             __props__.__dict__["db2_i"] = db2_i
@@ -2173,25 +2254,28 @@
             opts: Optional[pulumi.ResourceOptions] = None,
             aks: Optional[pulumi.Input[pulumi.InputType['ResourceAksArgs']]] = None,
             aks_basic_auth: Optional[pulumi.Input[pulumi.InputType['ResourceAksBasicAuthArgs']]] = None,
             aks_service_account: Optional[pulumi.Input[pulumi.InputType['ResourceAksServiceAccountArgs']]] = None,
             aks_service_account_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAksServiceAccountUserImpersonationArgs']]] = None,
             aks_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAksUserImpersonationArgs']]] = None,
             amazon_eks: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksArgs']]] = None,
+            amazon_eks_instance_profile: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksInstanceProfileArgs']]] = None,
+            amazon_eks_instance_profile_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksInstanceProfileUserImpersonationArgs']]] = None,
             amazon_eks_user_impersonation: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEksUserImpersonationArgs']]] = None,
             amazon_es: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonEsArgs']]] = None,
             amazonmq_amqp091: Optional[pulumi.Input[pulumi.InputType['ResourceAmazonmqAmqp091Args']]] = None,
             athena: Optional[pulumi.Input[pulumi.InputType['ResourceAthenaArgs']]] = None,
             aurora_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAuroraMysqlArgs']]] = None,
             aurora_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAuroraPostgresArgs']]] = None,
             aws: Optional[pulumi.Input[pulumi.InputType['ResourceAwsArgs']]] = None,
             aws_console: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']]] = None,
             aws_console_static_key_pair: Optional[pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']]] = None,
             azure: Optional[pulumi.Input[pulumi.InputType['ResourceAzureArgs']]] = None,
             azure_certificate: Optional[pulumi.Input[pulumi.InputType['ResourceAzureCertificateArgs']]] = None,
+            azure_mysql: Optional[pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']]] = None,
             azure_postgres: Optional[pulumi.Input[pulumi.InputType['ResourceAzurePostgresArgs']]] = None,
             big_query: Optional[pulumi.Input[pulumi.InputType['ResourceBigQueryArgs']]] = None,
             cassandra: Optional[pulumi.Input[pulumi.InputType['ResourceCassandraArgs']]] = None,
             citus: Optional[pulumi.Input[pulumi.InputType['ResourceCitusArgs']]] = None,
             clustrix: Optional[pulumi.Input[pulumi.InputType['ResourceClustrixArgs']]] = None,
             cockroach: Optional[pulumi.Input[pulumi.InputType['ResourceCockroachArgs']]] = None,
             db2_i: Optional[pulumi.Input[pulumi.InputType['ResourceDb2IArgs']]] = None,
@@ -2251,42 +2335,45 @@
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleArgs']] aws_console: AWSConsole is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceAwsConsoleStaticKeyPairArgs']] aws_console_static_key_pair: AWSConsoleStaticKeyPair is currently unstable, and its API may change, or it may be removed, without a major version
                bump.
+        :param pulumi.Input[pulumi.InputType['ResourceAzureMysqlArgs']] azure_mysql: AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoHostArgs']] mongo_host: MongoHost is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoReplicaSetArgs']] mongo_replica_set: MongoReplicaSet is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMongoShardedClusterArgs']] mongo_sharded_cluster: MongoShardedCluster is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceMtlsMysqlArgs']] mtls_mysql: MTLSMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        :param pulumi.Input[pulumi.InputType['ResourceOracleArgs']] oracle: Oracle is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['ResourceSnowsightArgs']] snowsight: Snowsight is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _ResourceState.__new__(_ResourceState)
 
         __props__.__dict__["aks"] = aks
         __props__.__dict__["aks_basic_auth"] = aks_basic_auth
         __props__.__dict__["aks_service_account"] = aks_service_account
         __props__.__dict__["aks_service_account_user_impersonation"] = aks_service_account_user_impersonation
         __props__.__dict__["aks_user_impersonation"] = aks_user_impersonation
         __props__.__dict__["amazon_eks"] = amazon_eks
+        __props__.__dict__["amazon_eks_instance_profile"] = amazon_eks_instance_profile
+        __props__.__dict__["amazon_eks_instance_profile_user_impersonation"] = amazon_eks_instance_profile_user_impersonation
         __props__.__dict__["amazon_eks_user_impersonation"] = amazon_eks_user_impersonation
         __props__.__dict__["amazon_es"] = amazon_es
         __props__.__dict__["amazonmq_amqp091"] = amazonmq_amqp091
         __props__.__dict__["athena"] = athena
         __props__.__dict__["aurora_mysql"] = aurora_mysql
         __props__.__dict__["aurora_postgres"] = aurora_postgres
         __props__.__dict__["aws"] = aws
         __props__.__dict__["aws_console"] = aws_console
         __props__.__dict__["aws_console_static_key_pair"] = aws_console_static_key_pair
         __props__.__dict__["azure"] = azure
         __props__.__dict__["azure_certificate"] = azure_certificate
+        __props__.__dict__["azure_mysql"] = azure_mysql
         __props__.__dict__["azure_postgres"] = azure_postgres
         __props__.__dict__["big_query"] = big_query
         __props__.__dict__["cassandra"] = cassandra
         __props__.__dict__["citus"] = citus
         __props__.__dict__["clustrix"] = clustrix
         __props__.__dict__["cockroach"] = cockroach
         __props__.__dict__["db2_i"] = db2_i
@@ -2369,14 +2456,24 @@
 
     @property
     @pulumi.getter(name="amazonEks")
     def amazon_eks(self) -> pulumi.Output[Optional['outputs.ResourceAmazonEks']]:
         return pulumi.get(self, "amazon_eks")
 
     @property
+    @pulumi.getter(name="amazonEksInstanceProfile")
+    def amazon_eks_instance_profile(self) -> pulumi.Output[Optional['outputs.ResourceAmazonEksInstanceProfile']]:
+        return pulumi.get(self, "amazon_eks_instance_profile")
+
+    @property
+    @pulumi.getter(name="amazonEksInstanceProfileUserImpersonation")
+    def amazon_eks_instance_profile_user_impersonation(self) -> pulumi.Output[Optional['outputs.ResourceAmazonEksInstanceProfileUserImpersonation']]:
+        return pulumi.get(self, "amazon_eks_instance_profile_user_impersonation")
+
+    @property
     @pulumi.getter(name="amazonEksUserImpersonation")
     def amazon_eks_user_impersonation(self) -> pulumi.Output[Optional['outputs.ResourceAmazonEksUserImpersonation']]:
         return pulumi.get(self, "amazon_eks_user_impersonation")
 
     @property
     @pulumi.getter(name="amazonEs")
     def amazon_es(self) -> pulumi.Output[Optional['outputs.ResourceAmazonEs']]:
@@ -2431,14 +2528,22 @@
 
     @property
     @pulumi.getter(name="azureCertificate")
     def azure_certificate(self) -> pulumi.Output[Optional['outputs.ResourceAzureCertificate']]:
         return pulumi.get(self, "azure_certificate")
 
     @property
+    @pulumi.getter(name="azureMysql")
+    def azure_mysql(self) -> pulumi.Output[Optional['outputs.ResourceAzureMysql']]:
+        """
+        AzureMysql is currently unstable, and its API may change, or it may be removed, without a major version bump.
+        """
+        return pulumi.get(self, "azure_mysql")
+
+    @property
     @pulumi.getter(name="azurePostgres")
     def azure_postgres(self) -> pulumi.Output[Optional['outputs.ResourceAzurePostgres']]:
         return pulumi.get(self, "azure_postgres")
 
     @property
     @pulumi.getter(name="bigQuery")
     def big_query(self) -> pulumi.Output[Optional['outputs.ResourceBigQuery']]:
@@ -2640,17 +2745,14 @@
     @pulumi.getter(name="neptuneIam")
     def neptune_iam(self) -> pulumi.Output[Optional['outputs.ResourceNeptuneIam']]:
         return pulumi.get(self, "neptune_iam")
 
     @property
     @pulumi.getter
     def oracle(self) -> pulumi.Output[Optional['outputs.ResourceOracle']]:
-        """
-        Oracle is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "oracle")
 
     @property
     @pulumi.getter
     def postgres(self) -> pulumi.Output[Optional['outputs.ResourcePostgres']]:
         return pulumi.get(self, "postgres")
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/role.py` & `pulumi_sdm-0.4.0/pulumi_sdm/role.py`

 * *Files 14% similar despite different names*

```diff
@@ -67,24 +67,28 @@
         pulumi.set(self, "tags", value)
 
 
 @pulumi.input_type
 class _RoleState:
     def __init__(__self__, *,
                  access_rules: Optional[pulumi.Input[str]] = None,
+                 managed_by: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering Role resources.
         :param pulumi.Input[str] access_rules: AccessRules is a list of access rules defining the resources this Role has access to.
+        :param pulumi.Input[str] managed_by: Managed By is a read only field for what service manages this role, e.g. StrongDM, Okta, Azure.
         :param pulumi.Input[str] name: Unique human-readable name of the Role.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         if access_rules is not None:
             pulumi.set(__self__, "access_rules", access_rules)
+        if managed_by is not None:
+            pulumi.set(__self__, "managed_by", managed_by)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="accessRules")
@@ -95,14 +99,26 @@
         return pulumi.get(self, "access_rules")
 
     @access_rules.setter
     def access_rules(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_rules", value)
 
     @property
+    @pulumi.getter(name="managedBy")
+    def managed_by(self) -> Optional[pulumi.Input[str]]:
+        """
+        Managed By is a read only field for what service manages this role, e.g. StrongDM, Okta, Azure.
+        """
+        return pulumi.get(self, "managed_by")
+
+    @managed_by.setter
+    def managed_by(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "managed_by", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Unique human-readable name of the Role.
         """
         return pulumi.get(self, "name")
 
@@ -188,56 +204,68 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = RoleArgs.__new__(RoleArgs)
 
             __props__.__dict__["access_rules"] = access_rules
             __props__.__dict__["name"] = name
             __props__.__dict__["tags"] = tags
+            __props__.__dict__["managed_by"] = None
         super(Role, __self__).__init__(
             'sdm:index/role:Role',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             access_rules: Optional[pulumi.Input[str]] = None,
+            managed_by: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None) -> 'Role':
         """
         Get an existing Role resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] access_rules: AccessRules is a list of access rules defining the resources this Role has access to.
+        :param pulumi.Input[str] managed_by: Managed By is a read only field for what service manages this role, e.g. StrongDM, Okta, Azure.
         :param pulumi.Input[str] name: Unique human-readable name of the Role.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Tags is a map of key, value pairs.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RoleState.__new__(_RoleState)
 
         __props__.__dict__["access_rules"] = access_rules
+        __props__.__dict__["managed_by"] = managed_by
         __props__.__dict__["name"] = name
         __props__.__dict__["tags"] = tags
         return Role(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="accessRules")
     def access_rules(self) -> pulumi.Output[str]:
         """
         AccessRules is a list of access rules defining the resources this Role has access to.
         """
         return pulumi.get(self, "access_rules")
 
     @property
+    @pulumi.getter(name="managedBy")
+    def managed_by(self) -> pulumi.Output[str]:
+        """
+        Managed By is a read only field for what service manages this role, e.g. StrongDM, Okta, Azure.
+        """
+        return pulumi.get(self, "managed_by")
+
+    @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         Unique human-readable name of the Role.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm/secret_store.py` & `pulumi_sdm-0.4.0/pulumi_sdm/secret_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,33 +15,34 @@
 
 @pulumi.input_type
 class SecretStoreArgs:
     def __init__(__self__, *,
                  aws: Optional[pulumi.Input['SecretStoreAwsArgs']] = None,
                  azure_store: Optional[pulumi.Input['SecretStoreAzureStoreArgs']] = None,
                  cyberark_conjur: Optional[pulumi.Input['SecretStoreCyberarkConjurArgs']] = None,
+                 cyberark_pam: Optional[pulumi.Input['SecretStoreCyberarkPamArgs']] = None,
                  cyberark_pam_experimental: Optional[pulumi.Input['SecretStoreCyberarkPamExperimentalArgs']] = None,
                  delinea_store: Optional[pulumi.Input['SecretStoreDelineaStoreArgs']] = None,
                  gcp_store: Optional[pulumi.Input['SecretStoreGcpStoreArgs']] = None,
                  vault_approle: Optional[pulumi.Input['SecretStoreVaultApproleArgs']] = None,
                  vault_tls: Optional[pulumi.Input['SecretStoreVaultTlsArgs']] = None,
                  vault_token: Optional[pulumi.Input['SecretStoreVaultTokenArgs']] = None):
         """
         The set of arguments for constructing a SecretStore resource.
-        :param pulumi.Input['SecretStoreCyberarkConjurArgs'] cyberark_conjur: CyberarkConjurStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['SecretStoreCyberarkPamExperimentalArgs'] cyberark_pam_experimental: CyberarkPAMExperimentalStore is currently unstable, and its API may change, or it may be removed, without a major
                version bump.
-        :param pulumi.Input['SecretStoreDelineaStoreArgs'] delinea_store: DelineaStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         if aws is not None:
             pulumi.set(__self__, "aws", aws)
         if azure_store is not None:
             pulumi.set(__self__, "azure_store", azure_store)
         if cyberark_conjur is not None:
             pulumi.set(__self__, "cyberark_conjur", cyberark_conjur)
+        if cyberark_pam is not None:
+            pulumi.set(__self__, "cyberark_pam", cyberark_pam)
         if cyberark_pam_experimental is not None:
             pulumi.set(__self__, "cyberark_pam_experimental", cyberark_pam_experimental)
         if delinea_store is not None:
             pulumi.set(__self__, "delinea_store", delinea_store)
         if gcp_store is not None:
             pulumi.set(__self__, "gcp_store", gcp_store)
         if vault_approle is not None:
@@ -68,24 +69,30 @@
     @azure_store.setter
     def azure_store(self, value: Optional[pulumi.Input['SecretStoreAzureStoreArgs']]):
         pulumi.set(self, "azure_store", value)
 
     @property
     @pulumi.getter(name="cyberarkConjur")
     def cyberark_conjur(self) -> Optional[pulumi.Input['SecretStoreCyberarkConjurArgs']]:
-        """
-        CyberarkConjurStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "cyberark_conjur")
 
     @cyberark_conjur.setter
     def cyberark_conjur(self, value: Optional[pulumi.Input['SecretStoreCyberarkConjurArgs']]):
         pulumi.set(self, "cyberark_conjur", value)
 
     @property
+    @pulumi.getter(name="cyberarkPam")
+    def cyberark_pam(self) -> Optional[pulumi.Input['SecretStoreCyberarkPamArgs']]:
+        return pulumi.get(self, "cyberark_pam")
+
+    @cyberark_pam.setter
+    def cyberark_pam(self, value: Optional[pulumi.Input['SecretStoreCyberarkPamArgs']]):
+        pulumi.set(self, "cyberark_pam", value)
+
+    @property
     @pulumi.getter(name="cyberarkPamExperimental")
     def cyberark_pam_experimental(self) -> Optional[pulumi.Input['SecretStoreCyberarkPamExperimentalArgs']]:
         """
         CyberarkPAMExperimentalStore is currently unstable, and its API may change, or it may be removed, without a major
         version bump.
         """
         return pulumi.get(self, "cyberark_pam_experimental")
@@ -93,17 +100,14 @@
     @cyberark_pam_experimental.setter
     def cyberark_pam_experimental(self, value: Optional[pulumi.Input['SecretStoreCyberarkPamExperimentalArgs']]):
         pulumi.set(self, "cyberark_pam_experimental", value)
 
     @property
     @pulumi.getter(name="delineaStore")
     def delinea_store(self) -> Optional[pulumi.Input['SecretStoreDelineaStoreArgs']]:
-        """
-        DelineaStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "delinea_store")
 
     @delinea_store.setter
     def delinea_store(self, value: Optional[pulumi.Input['SecretStoreDelineaStoreArgs']]):
         pulumi.set(self, "delinea_store", value)
 
     @property
@@ -145,33 +149,34 @@
 
 @pulumi.input_type
 class _SecretStoreState:
     def __init__(__self__, *,
                  aws: Optional[pulumi.Input['SecretStoreAwsArgs']] = None,
                  azure_store: Optional[pulumi.Input['SecretStoreAzureStoreArgs']] = None,
                  cyberark_conjur: Optional[pulumi.Input['SecretStoreCyberarkConjurArgs']] = None,
+                 cyberark_pam: Optional[pulumi.Input['SecretStoreCyberarkPamArgs']] = None,
                  cyberark_pam_experimental: Optional[pulumi.Input['SecretStoreCyberarkPamExperimentalArgs']] = None,
                  delinea_store: Optional[pulumi.Input['SecretStoreDelineaStoreArgs']] = None,
                  gcp_store: Optional[pulumi.Input['SecretStoreGcpStoreArgs']] = None,
                  vault_approle: Optional[pulumi.Input['SecretStoreVaultApproleArgs']] = None,
                  vault_tls: Optional[pulumi.Input['SecretStoreVaultTlsArgs']] = None,
                  vault_token: Optional[pulumi.Input['SecretStoreVaultTokenArgs']] = None):
         """
         Input properties used for looking up and filtering SecretStore resources.
-        :param pulumi.Input['SecretStoreCyberarkConjurArgs'] cyberark_conjur: CyberarkConjurStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input['SecretStoreCyberarkPamExperimentalArgs'] cyberark_pam_experimental: CyberarkPAMExperimentalStore is currently unstable, and its API may change, or it may be removed, without a major
                version bump.
-        :param pulumi.Input['SecretStoreDelineaStoreArgs'] delinea_store: DelineaStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         if aws is not None:
             pulumi.set(__self__, "aws", aws)
         if azure_store is not None:
             pulumi.set(__self__, "azure_store", azure_store)
         if cyberark_conjur is not None:
             pulumi.set(__self__, "cyberark_conjur", cyberark_conjur)
+        if cyberark_pam is not None:
+            pulumi.set(__self__, "cyberark_pam", cyberark_pam)
         if cyberark_pam_experimental is not None:
             pulumi.set(__self__, "cyberark_pam_experimental", cyberark_pam_experimental)
         if delinea_store is not None:
             pulumi.set(__self__, "delinea_store", delinea_store)
         if gcp_store is not None:
             pulumi.set(__self__, "gcp_store", gcp_store)
         if vault_approle is not None:
@@ -198,24 +203,30 @@
     @azure_store.setter
     def azure_store(self, value: Optional[pulumi.Input['SecretStoreAzureStoreArgs']]):
         pulumi.set(self, "azure_store", value)
 
     @property
     @pulumi.getter(name="cyberarkConjur")
     def cyberark_conjur(self) -> Optional[pulumi.Input['SecretStoreCyberarkConjurArgs']]:
-        """
-        CyberarkConjurStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "cyberark_conjur")
 
     @cyberark_conjur.setter
     def cyberark_conjur(self, value: Optional[pulumi.Input['SecretStoreCyberarkConjurArgs']]):
         pulumi.set(self, "cyberark_conjur", value)
 
     @property
+    @pulumi.getter(name="cyberarkPam")
+    def cyberark_pam(self) -> Optional[pulumi.Input['SecretStoreCyberarkPamArgs']]:
+        return pulumi.get(self, "cyberark_pam")
+
+    @cyberark_pam.setter
+    def cyberark_pam(self, value: Optional[pulumi.Input['SecretStoreCyberarkPamArgs']]):
+        pulumi.set(self, "cyberark_pam", value)
+
+    @property
     @pulumi.getter(name="cyberarkPamExperimental")
     def cyberark_pam_experimental(self) -> Optional[pulumi.Input['SecretStoreCyberarkPamExperimentalArgs']]:
         """
         CyberarkPAMExperimentalStore is currently unstable, and its API may change, or it may be removed, without a major
         version bump.
         """
         return pulumi.get(self, "cyberark_pam_experimental")
@@ -223,17 +234,14 @@
     @cyberark_pam_experimental.setter
     def cyberark_pam_experimental(self, value: Optional[pulumi.Input['SecretStoreCyberarkPamExperimentalArgs']]):
         pulumi.set(self, "cyberark_pam_experimental", value)
 
     @property
     @pulumi.getter(name="delineaStore")
     def delinea_store(self) -> Optional[pulumi.Input['SecretStoreDelineaStoreArgs']]:
-        """
-        DelineaStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "delinea_store")
 
     @delinea_store.setter
     def delinea_store(self, value: Optional[pulumi.Input['SecretStoreDelineaStoreArgs']]):
         pulumi.set(self, "delinea_store", value)
 
     @property
@@ -277,14 +285,15 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aws: Optional[pulumi.Input[pulumi.InputType['SecretStoreAwsArgs']]] = None,
                  azure_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreAzureStoreArgs']]] = None,
                  cyberark_conjur: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkConjurArgs']]] = None,
+                 cyberark_pam: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkPamArgs']]] = None,
                  cyberark_pam_experimental: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkPamExperimentalArgs']]] = None,
                  delinea_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreDelineaStoreArgs']]] = None,
                  gcp_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreGcpStoreArgs']]] = None,
                  vault_approle: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultApproleArgs']]] = None,
                  vault_tls: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultTlsArgs']]] = None,
                  vault_token: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultTokenArgs']]] = None,
                  __props__=None):
@@ -295,18 +304,16 @@
 
         ```sh
          $ pulumi import sdm:index/secretStore:SecretStore example se-12345678
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['SecretStoreCyberarkConjurArgs']] cyberark_conjur: CyberarkConjurStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['SecretStoreCyberarkPamExperimentalArgs']] cyberark_pam_experimental: CyberarkPAMExperimentalStore is currently unstable, and its API may change, or it may be removed, without a major
                version bump.
-        :param pulumi.Input[pulumi.InputType['SecretStoreDelineaStoreArgs']] delinea_store: DelineaStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[SecretStoreArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -333,14 +340,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  aws: Optional[pulumi.Input[pulumi.InputType['SecretStoreAwsArgs']]] = None,
                  azure_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreAzureStoreArgs']]] = None,
                  cyberark_conjur: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkConjurArgs']]] = None,
+                 cyberark_pam: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkPamArgs']]] = None,
                  cyberark_pam_experimental: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkPamExperimentalArgs']]] = None,
                  delinea_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreDelineaStoreArgs']]] = None,
                  gcp_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreGcpStoreArgs']]] = None,
                  vault_approle: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultApproleArgs']]] = None,
                  vault_tls: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultTlsArgs']]] = None,
                  vault_token: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultTokenArgs']]] = None,
                  __props__=None):
@@ -351,14 +359,15 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = SecretStoreArgs.__new__(SecretStoreArgs)
 
             __props__.__dict__["aws"] = aws
             __props__.__dict__["azure_store"] = azure_store
             __props__.__dict__["cyberark_conjur"] = cyberark_conjur
+            __props__.__dict__["cyberark_pam"] = cyberark_pam
             __props__.__dict__["cyberark_pam_experimental"] = cyberark_pam_experimental
             __props__.__dict__["delinea_store"] = delinea_store
             __props__.__dict__["gcp_store"] = gcp_store
             __props__.__dict__["vault_approle"] = vault_approle
             __props__.__dict__["vault_tls"] = vault_tls
             __props__.__dict__["vault_token"] = vault_token
         super(SecretStore, __self__).__init__(
@@ -370,39 +379,39 @@
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             aws: Optional[pulumi.Input[pulumi.InputType['SecretStoreAwsArgs']]] = None,
             azure_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreAzureStoreArgs']]] = None,
             cyberark_conjur: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkConjurArgs']]] = None,
+            cyberark_pam: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkPamArgs']]] = None,
             cyberark_pam_experimental: Optional[pulumi.Input[pulumi.InputType['SecretStoreCyberarkPamExperimentalArgs']]] = None,
             delinea_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreDelineaStoreArgs']]] = None,
             gcp_store: Optional[pulumi.Input[pulumi.InputType['SecretStoreGcpStoreArgs']]] = None,
             vault_approle: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultApproleArgs']]] = None,
             vault_tls: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultTlsArgs']]] = None,
             vault_token: Optional[pulumi.Input[pulumi.InputType['SecretStoreVaultTokenArgs']]] = None) -> 'SecretStore':
         """
         Get an existing SecretStore resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['SecretStoreCyberarkConjurArgs']] cyberark_conjur: CyberarkConjurStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
         :param pulumi.Input[pulumi.InputType['SecretStoreCyberarkPamExperimentalArgs']] cyberark_pam_experimental: CyberarkPAMExperimentalStore is currently unstable, and its API may change, or it may be removed, without a major
                version bump.
-        :param pulumi.Input[pulumi.InputType['SecretStoreDelineaStoreArgs']] delinea_store: DelineaStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _SecretStoreState.__new__(_SecretStoreState)
 
         __props__.__dict__["aws"] = aws
         __props__.__dict__["azure_store"] = azure_store
         __props__.__dict__["cyberark_conjur"] = cyberark_conjur
+        __props__.__dict__["cyberark_pam"] = cyberark_pam
         __props__.__dict__["cyberark_pam_experimental"] = cyberark_pam_experimental
         __props__.__dict__["delinea_store"] = delinea_store
         __props__.__dict__["gcp_store"] = gcp_store
         __props__.__dict__["vault_approle"] = vault_approle
         __props__.__dict__["vault_tls"] = vault_tls
         __props__.__dict__["vault_token"] = vault_token
         return SecretStore(resource_name, opts=opts, __props__=__props__)
@@ -416,34 +425,33 @@
     @pulumi.getter(name="azureStore")
     def azure_store(self) -> pulumi.Output[Optional['outputs.SecretStoreAzureStore']]:
         return pulumi.get(self, "azure_store")
 
     @property
     @pulumi.getter(name="cyberarkConjur")
     def cyberark_conjur(self) -> pulumi.Output[Optional['outputs.SecretStoreCyberarkConjur']]:
-        """
-        CyberarkConjurStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "cyberark_conjur")
 
     @property
+    @pulumi.getter(name="cyberarkPam")
+    def cyberark_pam(self) -> pulumi.Output[Optional['outputs.SecretStoreCyberarkPam']]:
+        return pulumi.get(self, "cyberark_pam")
+
+    @property
     @pulumi.getter(name="cyberarkPamExperimental")
     def cyberark_pam_experimental(self) -> pulumi.Output[Optional['outputs.SecretStoreCyberarkPamExperimental']]:
         """
         CyberarkPAMExperimentalStore is currently unstable, and its API may change, or it may be removed, without a major
         version bump.
         """
         return pulumi.get(self, "cyberark_pam_experimental")
 
     @property
     @pulumi.getter(name="delineaStore")
     def delinea_store(self) -> pulumi.Output[Optional['outputs.SecretStoreDelineaStore']]:
-        """
-        DelineaStore is currently unstable, and its API may change, or it may be removed, without a major version bump.
-        """
         return pulumi.get(self, "delinea_store")
 
     @property
     @pulumi.getter(name="gcpStore")
     def gcp_store(self) -> pulumi.Output[Optional['outputs.SecretStoreGcpStore']]:
         return pulumi.get(self, "gcp_store")
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm.egg-info/PKG-INFO` & `pulumi_sdm-0.4.0/pulumi_sdm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-sdm
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pulumi_sdm-0.3.0/pulumi_sdm.egg-info/SOURCES.txt` & `pulumi_sdm-0.4.0/pulumi_sdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.3.0/setup.py` & `pulumi_sdm-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.3.0"
-PLUGIN_VERSION = "0.3.0"
+VERSION = "0.4.0"
+PLUGIN_VERSION = "0.4.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'sdm', PLUGIN_VERSION, '--server', 'https://github.com/pierskarsenbarg/pulumi-sdm/releases/download/v${VERSION}'])
         except OSError as error:
```

