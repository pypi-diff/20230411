# Comparing `tmp/alibabacloud_alb20200616-1.0.8.tar.gz` & `tmp/alibabacloud_alb20200616-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alb20200616-1.0.8.tar", last modified: Tue Jan 25 12:31:11 2022, max compression
+gzip compressed data, was "dist/alibabacloud_alb20200616-1.0.9.tar", last modified: Wed Mar 16 02:24:06 2022, max compression
```

## Comparing `alibabacloud_alb20200616-1.0.8.tar` & `alibabacloud_alb20200616-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      411 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2328 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1022 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1107 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616/
--rw-r--r--   0 root         (0) root         (0)       21 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616/__init__.py
--rw-r--r--   0 root         (0) root         (0)   259315 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616/client.py
--rw-r--r--   0 root         (0) root         (0)   676109 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2328 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2610 2022-01-25 12:31:11.000000 alibabacloud_alb20200616-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 02:24:06.000000 alibabacloud_alb20200616-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      461 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-03-16 02:24:06.000000 alibabacloud_alb20200616-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1022 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1107 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 02:24:06.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   259315 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616/client.py
+-rw-r--r--   0 root         (0) root         (0)   681585 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-16 02:24:06.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2328 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-03-16 02:24:06.000000 alibabacloud_alb20200616-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2610 2022-03-16 02:24:05.000000 alibabacloud_alb20200616-1.0.9/setup.py
```

### Comparing `alibabacloud_alb20200616-1.0.8/LICENSE` & `alibabacloud_alb20200616-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alb20200616-1.0.8/PKG-INFO` & `alibabacloud_alb20200616-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alb20200616
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Alb (20200616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alb20200616-1.0.8/README-CN.md` & `alibabacloud_alb20200616-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alb20200616-1.0.8/README.md` & `alibabacloud_alb20200616-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616/client.py` & `alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616/models.py` & `alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1536,15 +1536,15 @@
         self.ca_enabled = ca_enabled
         # 监听默认服务器证书列表，N当前取值范围为1
         self.certificates = certificates
         # 幂等标识
         self.client_token = client_token
         # 监听默认动作
         self.default_actions = default_actions
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 是否开启Gzip压缩
         self.gzip_enabled = gzip_enabled
         # 是否开启HTTP/2特性
         self.http_2enabled = http_2enabled
         # 连接空闲超时时间
         self.idle_timeout = idle_timeout
@@ -1878,15 +1878,15 @@
         self.address_allocated_mode = address_allocated_mode
         # 负载均衡的地址类型
         self.address_type = address_type
         # 幂等标识
         self.client_token = client_token
         # 是否开启删除保护
         self.deletion_protection_enabled = deletion_protection_enabled
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 计费相关配置信息
         self.load_balancer_billing_config = load_balancer_billing_config
         # 负载均衡的版本
         self.load_balancer_edition = load_balancer_edition
         # 名称
         self.load_balancer_name = load_balancer_name
@@ -2972,15 +2972,15 @@
         priority: int = None,
         rule_actions: List[CreateRuleRequestRuleActions] = None,
         rule_conditions: List[CreateRuleRequestRuleConditions] = None,
         rule_name: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 监听标识
         self.listener_id = listener_id
         # 转发规则优先级
         self.priority = priority
         # 转发规则动作
         self.rule_actions = rule_actions
@@ -4167,15 +4167,15 @@
         client_token: str = None,
         dry_run: bool = None,
         listener_id: str = None,
         rules: List[CreateRulesRequestRules] = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 监听标识
         self.listener_id = listener_id
         # 转发规则列表
         self.rules = rules
 
     def validate(self):
@@ -4350,15 +4350,15 @@
         security_policy_name: str = None,
         tlsversions: List[str] = None,
     ):
         # 加密套件
         self.ciphers = ciphers
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 资源组id
         self.resource_group_id = resource_group_id
         # 安全策略名称
         self.security_policy_name = security_policy_name
         # tls版本
         self.tlsversions = tlsversions
@@ -4642,15 +4642,15 @@
         server_group_type: str = None,
         service_name: str = None,
         sticky_session_config: CreateServerGroupRequestStickySessionConfig = None,
         vpc_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 健康检查配置
         self.health_check_config = health_check_config
         # 后端协议类型
         self.protocol = protocol
         # 资源组id
         self.resource_group_id = resource_group_id
@@ -5037,15 +5037,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         listener_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 监听id
         self.listener_id = listener_id
 
     def validate(self):
         pass
 
@@ -5151,15 +5151,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         load_balancer_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 实例id
         self.load_balancer_id = load_balancer_id
 
     def validate(self):
         pass
 
@@ -5265,15 +5265,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         rule_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 转发规则标识
         self.rule_id = rule_id
 
     def validate(self):
         pass
 
@@ -5379,15 +5379,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         rule_ids: List[str] = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 同一个监听下的转发规则标识列表
         self.rule_ids = rule_ids
 
     def validate(self):
         pass
 
@@ -5493,15 +5493,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         security_policy_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 安全策略Id
         self.security_policy_id = security_policy_id
 
     def validate(self):
         pass
 
@@ -6107,15 +6107,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         resource_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 实例id
         self.resource_id = resource_id
 
     def validate(self):
         pass
 
@@ -6214,15 +6214,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         load_balancer_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 实例id
         self.load_balancer_id = load_balancer_id
 
     def validate(self):
         pass
 
@@ -6599,15 +6599,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         resource_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 实例id
         self.resource_id = resource_id
 
     def validate(self):
         pass
 
@@ -6708,15 +6708,15 @@
         dry_run: bool = None,
         load_balancer_id: str = None,
         log_project: str = None,
         log_store: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 实例id
         self.load_balancer_id = load_balancer_id
         # 日志Project
         self.log_project = log_project
         # 日志Store
         self.log_store = log_store
@@ -9617,15 +9617,15 @@
         self.jobs = jobs
         # 本次查询返回记录数量
         self.max_results = max_results
         # 分页查询标识
         self.next_token = next_token
         # Id of the request
         self.request_id = request_id
-        # 总记录数	
+        # 总记录数
         self.total_count = total_count
 
     def validate(self):
         if self.jobs:
             for k in self.jobs:
                 if k:
                     k.validate()
@@ -10548,14 +10548,15 @@
             self.xforwarded_for_slbport_enabled = m.get('XForwardedForSLBPortEnabled')
         return self
 
 
 class ListListenersResponseBodyListeners(TeaModel):
     def __init__(
         self,
+        ca_enabled: str = None,
         default_actions: List[ListListenersResponseBodyListenersDefaultActions] = None,
         gzip_enabled: bool = None,
         http_2enabled: bool = None,
         idle_timeout: int = None,
         listener_description: str = None,
         listener_id: str = None,
         listener_port: int = None,
@@ -10564,14 +10565,16 @@
         load_balancer_id: str = None,
         log_config: ListListenersResponseBodyListenersLogConfig = None,
         quic_config: ListListenersResponseBodyListenersQuicConfig = None,
         request_timeout: int = None,
         security_policy_id: str = None,
         xforwarded_for_config: ListListenersResponseBodyListenersXForwardedForConfig = None,
     ):
+        # 是否开启双向认证
+        self.ca_enabled = ca_enabled
         # 默认动作
         self.default_actions = default_actions
         # 是否开启Gzip压缩
         self.gzip_enabled = gzip_enabled
         # 是否开启HTTP/2特性
         self.http_2enabled = http_2enabled
         # 连接空闲超时时间
@@ -10613,14 +10616,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.ca_enabled is not None:
+            result['CaEnabled'] = self.ca_enabled
         result['DefaultActions'] = []
         if self.default_actions is not None:
             for k in self.default_actions:
                 result['DefaultActions'].append(k.to_map() if k else None)
         if self.gzip_enabled is not None:
             result['GzipEnabled'] = self.gzip_enabled
         if self.http_2enabled is not None:
@@ -10649,14 +10654,16 @@
             result['SecurityPolicyId'] = self.security_policy_id
         if self.xforwarded_for_config is not None:
             result['XForwardedForConfig'] = self.xforwarded_for_config.to_map()
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('CaEnabled') is not None:
+            self.ca_enabled = m.get('CaEnabled')
         self.default_actions = []
         if m.get('DefaultActions') is not None:
             for k in m.get('DefaultActions'):
                 temp_model = ListListenersResponseBodyListenersDefaultActions()
                 self.default_actions.append(temp_model.from_map(k))
         if m.get('GzipEnabled') is not None:
             self.gzip_enabled = m.get('GzipEnabled')
@@ -11740,51 +11747,186 @@
         if m.get('Path') is not None:
             self.path = m.get('Path')
         if m.get('Query') is not None:
             self.query = m.get('Query')
         return self
 
 
+class ListRulesResponseBodyRulesRuleActionsTrafficLimitConfig(TeaModel):
+    def __init__(
+        self,
+        qps: int = None,
+    ):
+        self.qps = qps
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
+        if self.qps is not None:
+            result['QPS'] = self.qps
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('QPS') is not None:
+            self.qps = m.get('QPS')
+        return self
+
+
+class ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfigMirrorGroupConfigServerGroupTuples(TeaModel):
+    def __init__(
+        self,
+        server_group_id: str = None,
+    ):
+        self.server_group_id = server_group_id
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
+        if self.server_group_id is not None:
+            result['ServerGroupId'] = self.server_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ServerGroupId') is not None:
+            self.server_group_id = m.get('ServerGroupId')
+        return self
+
+
+class ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfigMirrorGroupConfig(TeaModel):
+    def __init__(
+        self,
+        server_group_tuples: List[ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfigMirrorGroupConfigServerGroupTuples] = None,
+    ):
+        self.server_group_tuples = server_group_tuples
+
+    def validate(self):
+        if self.server_group_tuples:
+            for k in self.server_group_tuples:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ServerGroupTuples'] = []
+        if self.server_group_tuples is not None:
+            for k in self.server_group_tuples:
+                result['ServerGroupTuples'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.server_group_tuples = []
+        if m.get('ServerGroupTuples') is not None:
+            for k in m.get('ServerGroupTuples'):
+                temp_model = ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfigMirrorGroupConfigServerGroupTuples()
+                self.server_group_tuples.append(temp_model.from_map(k))
+        return self
+
+
+class ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfig(TeaModel):
+    def __init__(
+        self,
+        mirror_group_config: ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfigMirrorGroupConfig = None,
+        target_type: str = None,
+    ):
+        # TargetType为服务器组时必选，目标服务器组
+        self.mirror_group_config = mirror_group_config
+        # 流量镜像的目的，可以是服务器组
+        self.target_type = target_type
+
+    def validate(self):
+        if self.mirror_group_config:
+            self.mirror_group_config.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.mirror_group_config is not None:
+            result['MirrorGroupConfig'] = self.mirror_group_config.to_map()
+        if self.target_type is not None:
+            result['TargetType'] = self.target_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MirrorGroupConfig') is not None:
+            temp_model = ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfigMirrorGroupConfig()
+            self.mirror_group_config = temp_model.from_map(m['MirrorGroupConfig'])
+        if m.get('TargetType') is not None:
+            self.target_type = m.get('TargetType')
+        return self
+
+
 class ListRulesResponseBodyRulesRuleActions(TeaModel):
     def __init__(
         self,
         fixed_response_config: ListRulesResponseBodyRulesRuleActionsFixedResponseConfig = None,
         forward_group_config: ListRulesResponseBodyRulesRuleActionsForwardGroupConfig = None,
         insert_header_config: ListRulesResponseBodyRulesRuleActionsInsertHeaderConfig = None,
         order: int = None,
         redirect_config: ListRulesResponseBodyRulesRuleActionsRedirectConfig = None,
         rewrite_config: ListRulesResponseBodyRulesRuleActionsRewriteConfig = None,
+        traffic_limit_config: ListRulesResponseBodyRulesRuleActionsTrafficLimitConfig = None,
+        traffic_mirror_config: ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfig = None,
         type: str = None,
     ):
         # 返回固定内容动作配置
         self.fixed_response_config = fixed_response_config
         # 转发组动作配置
         self.forward_group_config = forward_group_config
         # 插入头部动作配置
         self.insert_header_config = insert_header_config
         # 优先级
         self.order = order
         # 重定向动作配置
         self.redirect_config = redirect_config
         # 内部重定向动作配置
         self.rewrite_config = rewrite_config
+        self.traffic_limit_config = traffic_limit_config
+        # 流量镜像Action对应的配置，type为TrafficMirror时必填且有效
+        self.traffic_mirror_config = traffic_mirror_config
         # 转发规则动作类型
         self.type = type
 
     def validate(self):
         if self.fixed_response_config:
             self.fixed_response_config.validate()
         if self.forward_group_config:
             self.forward_group_config.validate()
         if self.insert_header_config:
             self.insert_header_config.validate()
         if self.redirect_config:
             self.redirect_config.validate()
         if self.rewrite_config:
             self.rewrite_config.validate()
+        if self.traffic_limit_config:
+            self.traffic_limit_config.validate()
+        if self.traffic_mirror_config:
+            self.traffic_mirror_config.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -11796,14 +11938,18 @@
             result['InsertHeaderConfig'] = self.insert_header_config.to_map()
         if self.order is not None:
             result['Order'] = self.order
         if self.redirect_config is not None:
             result['RedirectConfig'] = self.redirect_config.to_map()
         if self.rewrite_config is not None:
             result['RewriteConfig'] = self.rewrite_config.to_map()
+        if self.traffic_limit_config is not None:
+            result['TrafficLimitConfig'] = self.traffic_limit_config.to_map()
+        if self.traffic_mirror_config is not None:
+            result['TrafficMirrorConfig'] = self.traffic_mirror_config.to_map()
         if self.type is not None:
             result['Type'] = self.type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('FixedResponseConfig') is not None:
@@ -11819,14 +11965,20 @@
             self.order = m.get('Order')
         if m.get('RedirectConfig') is not None:
             temp_model = ListRulesResponseBodyRulesRuleActionsRedirectConfig()
             self.redirect_config = temp_model.from_map(m['RedirectConfig'])
         if m.get('RewriteConfig') is not None:
             temp_model = ListRulesResponseBodyRulesRuleActionsRewriteConfig()
             self.rewrite_config = temp_model.from_map(m['RewriteConfig'])
+        if m.get('TrafficLimitConfig') is not None:
+            temp_model = ListRulesResponseBodyRulesRuleActionsTrafficLimitConfig()
+            self.traffic_limit_config = temp_model.from_map(m['TrafficLimitConfig'])
+        if m.get('TrafficMirrorConfig') is not None:
+            temp_model = ListRulesResponseBodyRulesRuleActionsTrafficMirrorConfig()
+            self.traffic_mirror_config = temp_model.from_map(m['TrafficMirrorConfig'])
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class ListRulesResponseBodyRulesRuleConditionsCookieConfigValues(TeaModel):
     def __init__(
@@ -14443,15 +14595,15 @@
         dry_run: bool = None,
         entries: List[str] = None,
     ):
         # 访问控制策略Id
         self.acl_id = acl_id
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 条目列表
         self.entries = entries
 
     def validate(self):
         pass
 
@@ -14611,15 +14763,15 @@
         client_token: str = None,
         dry_run: bool = None,
         server_group_id: str = None,
         servers: List[RemoveServersFromServerGroupRequestServers] = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 后端服务器Id
         self.server_group_id = server_group_id
         # 后端服务器
         self.servers = servers
 
     def validate(self):
@@ -14996,15 +15148,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         listener_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 监听id
         self.listener_id = listener_id
 
     def validate(self):
         pass
 
@@ -15110,15 +15262,15 @@
         self,
         client_token: str = None,
         dry_run: bool = None,
         listener_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 监听id
         self.listener_id = listener_id
 
     def validate(self):
         pass
 
@@ -16152,15 +16304,15 @@
         self.ca_enabled = ca_enabled
         # 监听默认服务器证书列表，N当前取值范围为1
         self.certificates = certificates
         # 幂等标识
         self.client_token = client_token
         # 监听默认动作
         self.default_actions = default_actions
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 是否开启Gzip压缩
         self.gzip_enabled = gzip_enabled
         # 是否开启HTTP/2特性
         self.http_2enabled = http_2enabled
         # 连接空闲超时时间
         self.idle_timeout = idle_timeout
@@ -16410,15 +16562,15 @@
     ):
         # 是否开启携带自定义Header
         self.access_log_record_customized_headers_enabled = access_log_record_customized_headers_enabled
         # 访问日志xtrace字段相关的配置
         self.access_log_tracing_config = access_log_tracing_config
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 监听标识
         self.listener_id = listener_id
 
     def validate(self):
         if self.access_log_tracing_config:
             self.access_log_tracing_config.validate()
@@ -16749,15 +16901,15 @@
         dry_run: bool = None,
         load_balancer_id: str = None,
         load_balancer_name: str = None,
         modification_protection_config: UpdateLoadBalancerAttributeRequestModificationProtectionConfig = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 实例id
         self.load_balancer_id = load_balancer_id
         # 名称
         self.load_balancer_name = load_balancer_name
         # 负载均衡修改保护相关信息
         self.modification_protection_config = modification_protection_config
@@ -16878,15 +17030,15 @@
         client_token: str = None,
         dry_run: bool = None,
         load_balancer_edition: str = None,
         load_balancer_id: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 实例版本
         self.load_balancer_edition = load_balancer_edition
         # 实例Id
         self.load_balancer_id = load_balancer_id
 
     def validate(self):
@@ -17027,15 +17179,15 @@
         client_token: str = None,
         dry_run: bool = None,
         load_balancer_id: str = None,
         zone_mappings: List[UpdateLoadBalancerZonesRequestZoneMappings] = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 实例id
         self.load_balancer_id = load_balancer_id
         # 可用区及交换机映射列表
         self.zone_mappings = zone_mappings
 
     def validate(self):
@@ -18073,15 +18225,15 @@
         rule_actions: List[UpdateRuleAttributeRequestRuleActions] = None,
         rule_conditions: List[UpdateRuleAttributeRequestRuleConditions] = None,
         rule_id: str = None,
         rule_name: str = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 转发规则优先级
         self.priority = priority
         # 转发规则动作
         self.rule_actions = rule_actions
         # 转发规则条件
         self.rule_conditions = rule_conditions
@@ -19476,15 +19628,15 @@
         security_policy_name: str = None,
         tlsversions: List[str] = None,
     ):
         # 加密套件
         self.ciphers = ciphers
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 安全策略id
         self.security_policy_id = security_policy_id
         # 安全策略名称
         self.security_policy_name = security_policy_name
         # TLS版本
         self.tlsversions = tlsversions
@@ -19765,15 +19917,15 @@
         server_group_id: str = None,
         server_group_name: str = None,
         service_name: str = None,
         sticky_session_config: UpdateServerGroupAttributeRequestStickySessionConfig = None,
     ):
         # 幂等标识
         self.client_token = client_token
-        #  是否只预检此次请求
+        # 是否只预检此次请求
         self.dry_run = dry_run
         # 健康检查配置
         self.health_check_config = health_check_config
         # 调度策略
         self.scheduler = scheduler
         # 服务器组Id
         self.server_group_id = server_group_id
```

### Comparing `alibabacloud_alb20200616-1.0.8/alibabacloud_alb20200616.egg-info/PKG-INFO` & `alibabacloud_alb20200616-1.0.9/alibabacloud_alb20200616.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alb20200616
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Alb (20200616) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alb20200616-1.0.8/setup.py` & `alibabacloud_alb20200616-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alb20200616.
 
-Created on 25/01/2022
+Created on 16/03/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alb20200616"
 NAME = "alibabacloud_alb20200616" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Alb (20200616) SDK Library for Python"
```

