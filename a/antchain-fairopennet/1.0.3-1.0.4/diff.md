# Comparing `tmp/antchain_fairopennet-1.0.3.tar.gz` & `tmp/antchain_fairopennet-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_fairopennet-1.0.3.tar", last modified: Mon Apr 10 02:05:06 2023, max compression
+gzip compressed data, was "dist/antchain_fairopennet-1.0.4.tar", last modified: Tue Apr 11 12:02:00 2023, max compression
```

## Comparing `antchain_fairopennet-1.0.3.tar` & `antchain_fairopennet-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:05:06.000000 antchain_fairopennet-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2210 2023-04-10 02:05:06.000000 antchain_fairopennet-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      828 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:05:06.000000 antchain_fairopennet-1.0.3/antchain_fairopennet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2210 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/antchain_fairopennet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2023-04-10 02:05:06.000000 antchain_fairopennet-1.0.3/antchain_fairopennet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/antchain_fairopennet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/antchain_fairopennet.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/antchain_fairopennet.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:05:06.000000 antchain_fairopennet-1.0.3/antchain_sdk_fairopennet/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/antchain_sdk_fairopennet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73774 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/antchain_sdk_fairopennet/client.py
--rw-r--r--   0 root         (0) root         (0)   114232 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/antchain_sdk_fairopennet/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-10 02:05:06.000000 antchain_fairopennet-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2528 2023-04-10 02:05:05.000000 antchain_fairopennet-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      828 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80220 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/client.py
+-rw-r--r--   0 root         (0) root         (0)   124064 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2528 2023-04-11 12:02:00.000000 antchain_fairopennet-1.0.4/setup.py
```

### Comparing `antchain_fairopennet-1.0.3/LICENSE` & `antchain_fairopennet-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_fairopennet-1.0.3/PKG-INFO` & `antchain_fairopennet-1.0.4/antchain_fairopennet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_fairopennet
-Version: 1.0.3
+Name: antchain-fairopennet
+Version: 1.0.4
 Summary: Ant Chain FAIROPENNET SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_fairopennet-1.0.3/README-CN.md` & `antchain_fairopennet-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_fairopennet-1.0.3/README.md` & `antchain_fairopennet-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `antchain_fairopennet-1.0.3/antchain_fairopennet.egg-info/PKG-INFO` & `antchain_fairopennet-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-fairopennet
-Version: 1.0.3
+Name: antchain_fairopennet
+Version: 1.0.4
 Summary: Ant Chain FAIROPENNET SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_fairopennet-1.0.3/antchain_sdk_fairopennet/client.py` & `antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.3',
+                    'sdk_version': '1.0.4',
                     '_prod_code': 'FAIROPENNET',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.3',
+                    'sdk_version': '1.0.4',
                     '_prod_code': 'FAIROPENNET',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1683,14 +1683,182 @@
             request.file_id = upload_resp.file_id
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             fairopennet_models.DownloadFileResponse(),
             await self.do_request_async('1.0', 'antchain.fairopennet.file.download', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def get_node_list(
+        self,
+        request: fairopennet_models.GetNodeListRequest,
+    ) -> fairopennet_models.GetNodeListResponse:
+        """
+        Description: 查询可用的fair节点nodeId
+        Summary: 查询fair node列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_node_list_ex(request, headers, runtime)
+
+    async def get_node_list_async(
+        self,
+        request: fairopennet_models.GetNodeListRequest,
+    ) -> fairopennet_models.GetNodeListResponse:
+        """
+        Description: 查询可用的fair节点nodeId
+        Summary: 查询fair node列表
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_node_list_ex_async(request, headers, runtime)
+
+    def get_node_list_ex(
+        self,
+        request: fairopennet_models.GetNodeListRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fairopennet_models.GetNodeListResponse:
+        """
+        Description: 查询可用的fair节点nodeId
+        Summary: 查询fair node列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            fairopennet_models.GetNodeListResponse(),
+            self.do_request('1.0', 'antchain.fairopennet.node.list.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_node_list_ex_async(
+        self,
+        request: fairopennet_models.GetNodeListRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fairopennet_models.GetNodeListResponse:
+        """
+        Description: 查询可用的fair节点nodeId
+        Summary: 查询fair node列表
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            fairopennet_models.GetNodeListResponse(),
+            await self.do_request_async('1.0', 'antchain.fairopennet.node.list.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def register_party(
+        self,
+        request: fairopennet_models.RegisterPartyRequest,
+    ) -> fairopennet_models.RegisterPartyResponse:
+        """
+        Description: 注册新用户
+        Summary: 注册新用户
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.register_party_ex(request, headers, runtime)
+
+    async def register_party_async(
+        self,
+        request: fairopennet_models.RegisterPartyRequest,
+    ) -> fairopennet_models.RegisterPartyResponse:
+        """
+        Description: 注册新用户
+        Summary: 注册新用户
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.register_party_ex_async(request, headers, runtime)
+
+    def register_party_ex(
+        self,
+        request: fairopennet_models.RegisterPartyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fairopennet_models.RegisterPartyResponse:
+        """
+        Description: 注册新用户
+        Summary: 注册新用户
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            fairopennet_models.RegisterPartyResponse(),
+            self.do_request('1.0', 'antchain.fairopennet.party.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def register_party_ex_async(
+        self,
+        request: fairopennet_models.RegisterPartyRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fairopennet_models.RegisterPartyResponse:
+        """
+        Description: 注册新用户
+        Summary: 注册新用户
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            fairopennet_models.RegisterPartyResponse(),
+            await self.do_request_async('1.0', 'antchain.fairopennet.party.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_party_registerstatus(
+        self,
+        request: fairopennet_models.QueryPartyRegisterstatusRequest,
+    ) -> fairopennet_models.QueryPartyRegisterstatusResponse:
+        """
+        Description: 查询用户是否注册成功
+        Summary: 查询用户注册进度
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_party_registerstatus_ex(request, headers, runtime)
+
+    async def query_party_registerstatus_async(
+        self,
+        request: fairopennet_models.QueryPartyRegisterstatusRequest,
+    ) -> fairopennet_models.QueryPartyRegisterstatusResponse:
+        """
+        Description: 查询用户是否注册成功
+        Summary: 查询用户注册进度
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_party_registerstatus_ex_async(request, headers, runtime)
+
+    def query_party_registerstatus_ex(
+        self,
+        request: fairopennet_models.QueryPartyRegisterstatusRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fairopennet_models.QueryPartyRegisterstatusResponse:
+        """
+        Description: 查询用户是否注册成功
+        Summary: 查询用户注册进度
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            fairopennet_models.QueryPartyRegisterstatusResponse(),
+            self.do_request('1.0', 'antchain.fairopennet.party.registerstatus.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_party_registerstatus_ex_async(
+        self,
+        request: fairopennet_models.QueryPartyRegisterstatusRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> fairopennet_models.QueryPartyRegisterstatusResponse:
+        """
+        Description: 查询用户是否注册成功
+        Summary: 查询用户注册进度
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            fairopennet_models.QueryPartyRegisterstatusResponse(),
+            await self.do_request_async('1.0', 'antchain.fairopennet.party.registerstatus.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_antcloud_gatewayx_file_upload(
         self,
         request: fairopennet_models.CreateAntcloudGatewayxFileUploadRequest,
     ) -> fairopennet_models.CreateAntcloudGatewayxFileUploadResponse:
         """
         Description: 创建HTTP PUT提交的文件上传
         Summary: 文件上传创建
```

### Comparing `antchain_fairopennet-1.0.3/antchain_sdk_fairopennet/models.py` & `antchain_fairopennet-1.0.4/antchain_sdk_fairopennet/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,50 @@
         if m.get('auto_start') is not None:
             self.auto_start = m.get('auto_start')
         if m.get('parameters') is not None:
             self.parameters = m.get('parameters')
         return self
 
 
+class NodeEndpoint(TeaModel):
+    def __init__(
+        self,
+        ip: str = None,
+        port: str = None,
+    ):
+        # 
+        self.ip = ip
+        # 
+        self.port = port
+
+    def validate(self):
+        self.validate_required(self.ip, 'ip')
+        self.validate_required(self.port, 'port')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ip is not None:
+            result['ip'] = self.ip
+        if self.port is not None:
+            result['port'] = self.port
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ip') is not None:
+            self.ip = m.get('ip')
+        if m.get('port') is not None:
+            self.port = m.get('port')
+        return self
+
+
 class GetNetworkStatusInput(TeaModel):
     def __init__(
         self,
         network_id: str = None,
     ):
         # 网络的networkId
         self.network_id = network_id
@@ -964,24 +1000,24 @@
         return self
 
 
 class CubeNode(TeaModel):
     def __init__(
         self,
         domain: str = None,
-        endpoints: List[str] = None,
+        endpoints: List[NodeEndpoint] = None,
         node_id: str = None,
         node_id_hash: str = None,
         node_public_key: str = None,
         is_connected: bool = None,
         type: int = None,
     ):
         # 无
         self.domain = domain
-        # 无
+        # 
         self.endpoints = endpoints
         # 
         self.node_id = node_id
         # 
         self.node_id_hash = node_id_hash
         # 
         self.node_public_key = node_public_key
@@ -989,30 +1025,36 @@
         self.is_connected = is_connected
         # 
         self.type = type
 
     def validate(self):
         self.validate_required(self.domain, 'domain')
         self.validate_required(self.endpoints, 'endpoints')
+        if self.endpoints:
+            for k in self.endpoints:
+                if k:
+                    k.validate()
         self.validate_required(self.node_id, 'node_id')
         self.validate_required(self.node_id_hash, 'node_id_hash')
         self.validate_required(self.node_public_key, 'node_public_key')
         self.validate_required(self.is_connected, 'is_connected')
         self.validate_required(self.type, 'type')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.domain is not None:
             result['domain'] = self.domain
+        result['endpoints'] = []
         if self.endpoints is not None:
-            result['endpoints'] = self.endpoints
+            for k in self.endpoints:
+                result['endpoints'].append(k.to_map() if k else None)
         if self.node_id is not None:
             result['node_id'] = self.node_id
         if self.node_id_hash is not None:
             result['node_id_hash'] = self.node_id_hash
         if self.node_public_key is not None:
             result['node_public_key'] = self.node_public_key
         if self.is_connected is not None:
@@ -1021,16 +1063,19 @@
             result['type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('domain') is not None:
             self.domain = m.get('domain')
+        self.endpoints = []
         if m.get('endpoints') is not None:
-            self.endpoints = m.get('endpoints')
+            for k in m.get('endpoints'):
+                temp_model = NodeEndpoint()
+                self.endpoints.append(temp_model.from_map(k))
         if m.get('node_id') is not None:
             self.node_id = m.get('node_id')
         if m.get('node_id_hash') is not None:
             self.node_id_hash = m.get('node_id_hash')
         if m.get('node_public_key') is not None:
             self.node_public_key = m.get('node_public_key')
         if m.get('is_connected') is not None:
@@ -3330,14 +3375,287 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class GetNodeListRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class GetNodeListResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        node_list: List[str] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # nodeId列表
+        self.node_list = node_list
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.node_list is not None:
+            result['node_list'] = self.node_list
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('node_list') is not None:
+            self.node_list = m.get('node_list')
+        return self
+
+
+class RegisterPartyRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        party_id: str = None,
+        party_desc: str = None,
+        node_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 参与方的partyId
+        self.party_id = party_id
+        # 描述party
+        self.party_desc = party_desc
+        # 节点的nodeId
+        self.node_id = node_id
+
+    def validate(self):
+        self.validate_required(self.party_id, 'party_id')
+        self.validate_required(self.party_desc, 'party_desc')
+        self.validate_required(self.node_id, 'node_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.party_id is not None:
+            result['party_id'] = self.party_id
+        if self.party_desc is not None:
+            result['party_desc'] = self.party_desc
+        if self.node_id is not None:
+            result['node_id'] = self.node_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('party_id') is not None:
+            self.party_id = m.get('party_id')
+        if m.get('party_desc') is not None:
+            self.party_desc = m.get('party_desc')
+        if m.get('node_id') is not None:
+            self.node_id = m.get('node_id')
+        return self
+
+
+class RegisterPartyResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class QueryPartyRegisterstatusRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        node_id: str = None,
+        party_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 节点的nodeId
+        self.node_id = node_id
+        # 用户的partyId
+        self.party_id = party_id
+
+    def validate(self):
+        self.validate_required(self.node_id, 'node_id')
+        self.validate_required(self.party_id, 'party_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.node_id is not None:
+            result['node_id'] = self.node_id
+        if self.party_id is not None:
+            result['party_id'] = self.party_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('node_id') is not None:
+            self.node_id = m.get('node_id')
+        if m.get('party_id') is not None:
+            self.party_id = m.get('party_id')
+        return self
+
+
+class QueryPartyRegisterstatusResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
 
     def validate(self):
```

### Comparing `antchain_fairopennet-1.0.3/setup.py` & `antchain_fairopennet-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_fairopennet.
 
-Created on 10/04/2023
+Created on 11/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_fairopennet"
 NAME = "antchain_fairopennet" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain FAIROPENNET SDK Library for Python"
```

