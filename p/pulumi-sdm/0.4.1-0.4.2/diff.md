# Comparing `tmp/pulumi_sdm-0.4.1.tar.gz` & `tmp/pulumi_sdm-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_sdm-0.4.1.tar", last modified: Tue Apr 11 10:01:09 2023, max compression
+gzip compressed data, was "dist/pulumi_sdm-0.4.2.tar", last modified: Tue Apr 11 10:23:30 2023, max compression
```

## Comparing `pulumi_sdm-0.4.1.tar` & `pulumi_sdm-0.4.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm/
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   769508 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/account_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_account_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_remote_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_secret_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/get_ssh_ca_pubkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/node.py
--rw-r--r--   0 runner    (1001) docker     (123)  1110292 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/remote_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)   145518 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/pulumi_sdm/secret_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/pulumi_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:01:09.000000 pulumi_sdm-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-11 10:01:08.000000 pulumi_sdm-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   769508 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/account_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_account_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_remote_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_secret_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/get_ssh_ca_pubkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1110292 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/remote_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145518 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22700 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/pulumi_sdm/secret_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/pulumi_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:23:30.000000 pulumi_sdm-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-11 10:23:29.000000 pulumi_sdm-0.4.2/setup.py
```

### Comparing `pulumi_sdm-0.4.1/PKG-INFO` & `pulumi_sdm-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_sdm
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pulumi_sdm-0.4.1/README.md` & `pulumi_sdm-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/__init__.py` & `pulumi_sdm-0.4.2/pulumi_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/_inputs.py` & `pulumi_sdm-0.4.2/pulumi_sdm/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/_utilities.py` & `pulumi_sdm-0.4.2/pulumi_sdm/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/account.py` & `pulumi_sdm-0.4.2/pulumi_sdm/account.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/account_attachment.py` & `pulumi_sdm-0.4.2/pulumi_sdm/account_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/config/vars.py` & `pulumi_sdm-0.4.2/pulumi_sdm/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_account.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_account_attachment.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_account_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_node.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_remote_identity.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_remote_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_remote_identity_group.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_remote_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_resource.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_role.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_secret_store.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_secret_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/get_ssh_ca_pubkey.py` & `pulumi_sdm-0.4.2/pulumi_sdm/get_ssh_ca_pubkey.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/node.py` & `pulumi_sdm-0.4.2/pulumi_sdm/node.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/outputs.py` & `pulumi_sdm-0.4.2/pulumi_sdm/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/provider.py` & `pulumi_sdm-0.4.2/pulumi_sdm/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/remote_identity.py` & `pulumi_sdm-0.4.2/pulumi_sdm/remote_identity.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/resource.py` & `pulumi_sdm-0.4.2/pulumi_sdm/resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/role.py` & `pulumi_sdm-0.4.2/pulumi_sdm/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm/secret_store.py` & `pulumi_sdm-0.4.2/pulumi_sdm/secret_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm.egg-info/PKG-INFO` & `pulumi_sdm-0.4.2/pulumi_sdm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-sdm
-Version: 0.4.1
+Version: 0.4.2
 Summary: A Pulumi package for creating and managing StrongDM cloud resources.
 Home-page: https://github.com/pierskarsenbarg/pulumi-sdm
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pierskarsenbarg/pulumi-sdm
 Description: # StrongDM Resource Provider
         
         The StrongDM Resource Provider lets you manage [StrongDM](http://strongdm.com) resources.
```

### Comparing `pulumi_sdm-0.4.1/pulumi_sdm.egg-info/SOURCES.txt` & `pulumi_sdm-0.4.2/pulumi_sdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_sdm-0.4.1/setup.py` & `pulumi_sdm-0.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.1"
-PLUGIN_VERSION = "0.4.1"
+VERSION = "0.4.2"
+PLUGIN_VERSION = "0.4.2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'sdm', PLUGIN_VERSION, '--server', 'github://api.github.com/pierskarsenbarg/pulumi-sdm'])
         except OSError as error:
```

