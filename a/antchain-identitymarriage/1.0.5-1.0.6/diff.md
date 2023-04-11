# Comparing `tmp/antchain_identitymarriage-1.0.5.tar.gz` & `tmp/antchain_identitymarriage-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_identitymarriage-1.0.5.tar", last modified: Mon Apr 10 08:49:47 2023, max compression
+gzip compressed data, was "dist/antchain_identitymarriage-1.0.6.tar", last modified: Tue Apr 11 11:32:24 2023, max compression
```

## Comparing `antchain_identitymarriage-1.0.5.tar` & `antchain_identitymarriage-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 08:49:46.000000 antchain_identitymarriage-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 08:49:46.000000 antchain_identitymarriage-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2240 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      843 2023-04-10 08:49:46.000000 antchain_identitymarriage-1.0.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1029 2023-04-10 08:49:46.000000 antchain_identitymarriage-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/antchain_identitymarriage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2240 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/antchain_identitymarriage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/antchain_identitymarriage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/antchain_identitymarriage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/antchain_identitymarriage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/antchain_identitymarriage.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/antchain_sdk_identitymarriage/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 08:49:46.000000 antchain_identitymarriage-1.0.5/antchain_sdk_identitymarriage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19253 2023-04-10 08:49:46.000000 antchain_identitymarriage-1.0.5/antchain_sdk_identitymarriage/client.py
--rw-r--r--   0 root         (0) root         (0)    14597 2023-04-10 08:49:46.000000 antchain_identitymarriage-1.0.5/antchain_sdk_identitymarriage/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 08:49:47.000000 antchain_identitymarriage-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2553 2023-04-10 08:49:46.000000 antchain_identitymarriage-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 11:32:23.000000 antchain_identitymarriage-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 11:32:23.000000 antchain_identitymarriage-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      843 2023-04-11 11:32:23.000000 antchain_identitymarriage-1.0.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-04-11 11:32:23.000000 antchain_identitymarriage-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/antchain_identitymarriage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2240 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/antchain_identitymarriage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      427 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/antchain_identitymarriage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/antchain_identitymarriage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/antchain_identitymarriage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/antchain_identitymarriage.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/antchain_sdk_identitymarriage/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 11:32:23.000000 antchain_identitymarriage-1.0.6/antchain_sdk_identitymarriage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19253 2023-04-11 11:32:23.000000 antchain_identitymarriage-1.0.6/antchain_sdk_identitymarriage/client.py
+-rw-r--r--   0 root         (0) root         (0)    14848 2023-04-11 11:32:23.000000 antchain_identitymarriage-1.0.6/antchain_sdk_identitymarriage/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 11:32:24.000000 antchain_identitymarriage-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-04-11 11:32:23.000000 antchain_identitymarriage-1.0.6/setup.py
```

### Comparing `antchain_identitymarriage-1.0.5/LICENSE` & `antchain_identitymarriage-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_identitymarriage-1.0.5/PKG-INFO` & `antchain_identitymarriage-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_identitymarriage
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ant Chain IDENTITYMARRIAGE SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_identitymarriage-1.0.5/README-CN.md` & `antchain_identitymarriage-1.0.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_identitymarriage-1.0.5/README.md` & `antchain_identitymarriage-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `antchain_identitymarriage-1.0.5/antchain_identitymarriage.egg-info/PKG-INFO` & `antchain_identitymarriage-1.0.6/antchain_identitymarriage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-identitymarriage
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ant Chain IDENTITYMARRIAGE SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_identitymarriage-1.0.5/antchain_sdk_identitymarriage/client.py` & `antchain_identitymarriage-1.0.6/antchain_sdk_identitymarriage/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.5',
+                    'sdk_version': '1.0.6',
                     '_prod_code': 'IDENTITYMARRIAGE',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.5',
+                    'sdk_version': '1.0.6',
                     '_prod_code': 'IDENTITYMARRIAGE',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_identitymarriage-1.0.5/antchain_sdk_identitymarriage/models.py` & `antchain_identitymarriage-1.0.6/antchain_sdk_identitymarriage/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,47 +334,55 @@
 
 
 class UploadFileDataRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
-        biz_content: str = None,
+        file_name: str = None,
+        file: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
-        # 文件
-        self.biz_content = biz_content
+        # 文件名
+        self.file_name = file_name
+        # 文件流
+        self.file = file
 
     def validate(self):
-        self.validate_required(self.biz_content, 'biz_content')
+        self.validate_required(self.file_name, 'file_name')
+        self.validate_required(self.file, 'file')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
-        if self.biz_content is not None:
-            result['biz_content'] = self.biz_content
+        if self.file_name is not None:
+            result['file_name'] = self.file_name
+        if self.file is not None:
+            result['file'] = self.file
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
-        if m.get('biz_content') is not None:
-            self.biz_content = m.get('biz_content')
+        if m.get('file_name') is not None:
+            self.file_name = m.get('file_name')
+        if m.get('file') is not None:
+            self.file = m.get('file')
         return self
 
 
 class UploadFileDataResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_identitymarriage-1.0.5/setup.py` & `antchain_identitymarriage-1.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_identitymarriage.
 
-Created on 10/04/2023
+Created on 11/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_identitymarriage"
 NAME = "antchain_identitymarriage" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain IDENTITYMARRIAGE SDK Library for Python"
```

