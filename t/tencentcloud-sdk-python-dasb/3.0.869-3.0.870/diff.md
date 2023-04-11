# Comparing `tmp/tencentcloud-sdk-python-dasb-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-dasb-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.869.tar", last modified: Mon Apr 10 03:00:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.870.tar", last modified: Tue Apr 11 03:31:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dasb-3.0.869.tar` & `tencentcloud-sdk-python-dasb-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)   107559 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37810 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/v20191018/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud_sdk_python_dasb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:00:02.000000 tencentcloud-sdk-python-dasb-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)   152157 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45577 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/v20191018/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud_sdk_python_dasb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:31:38.000000 tencentcloud-sdk-python-dasb-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.870/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.869'
+__version__ = '3.0.870'
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/v20191018/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -294,14 +294,78 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AuditLogResult(AbstractModel):
+    """审计日志
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Sid: 被审计会话的Sid
+        :type Sid: str
+        :param Uin: 审计者的编号
+        :type Uin: str
+        :param Time: 审计动作发生的时间
+        :type Time: str
+        :param ClientIp: 审计者的Ip
+        :type ClientIp: str
+        :param Operation: 审计动作类型，1--回放、2--中断、3--监控
+        :type Operation: int
+        :param InstanceId: 被审计主机的Id
+        :type InstanceId: str
+        :param DeviceName: 被审计主机的主机名
+        :type DeviceName: str
+        :param Protocol: 被审计会话所属的类型，如字符会话
+        :type Protocol: str
+        :param PrivateIp: 被审计主机的内部Ip
+        :type PrivateIp: str
+        :param PublicIp: 被审计主机的外部Ip
+        :type PublicIp: str
+        :param SubAccountUin: 审计者的子账号
+        :type SubAccountUin: str
+        """
+        self.Sid = None
+        self.Uin = None
+        self.Time = None
+        self.ClientIp = None
+        self.Operation = None
+        self.InstanceId = None
+        self.DeviceName = None
+        self.Protocol = None
+        self.PrivateIp = None
+        self.PublicIp = None
+        self.SubAccountUin = None
+
+
+    def _deserialize(self, params):
+        self.Sid = params.get("Sid")
+        self.Uin = params.get("Uin")
+        self.Time = params.get("Time")
+        self.ClientIp = params.get("ClientIp")
+        self.Operation = params.get("Operation")
+        self.InstanceId = params.get("InstanceId")
+        self.DeviceName = params.get("DeviceName")
+        self.Protocol = params.get("Protocol")
+        self.PrivateIp = params.get("PrivateIp")
+        self.PublicIp = params.get("PublicIp")
+        self.SubAccountUin = params.get("SubAccountUin")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BindDeviceAccountPasswordRequest(AbstractModel):
     """BindDeviceAccountPassword请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -465,14 +529,50 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class Command(AbstractModel):
+    """命令集合
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Cmd: 命令
+        :type Cmd: str
+        :param Time: 命令输入的时间
+        :type Time: str
+        :param TimeOffset: 命令执行时间相对于所属会话开始时间的偏移量，单位ms
+        :type TimeOffset: int
+        :param Action: 命令执行情况，1--允许，2--拒绝，3--确认
+        :type Action: int
+        """
+        self.Cmd = None
+        self.Time = None
+        self.TimeOffset = None
+        self.Action = None
+
+
+    def _deserialize(self, params):
+        self.Cmd = params.get("Cmd")
+        self.Time = params.get("Time")
+        self.TimeOffset = params.get("TimeOffset")
+        self.Action = params.get("Action")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CreateAclRequest(AbstractModel):
     """CreateAcl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1981,14 +2081,186 @@
             for item in params.get("DeviceSet"):
                 obj = Device()
                 obj._deserialize(item)
                 self.DeviceSet.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLoginEventRequest(AbstractModel):
+    """DescribeLoginEvent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserName: 用户名，如果不包含其他条件时对user_name or real_name两个字段模糊查询
+        :type UserName: str
+        :param RealName: 姓名，模糊查询
+        :type RealName: str
+        :param StartTime: 查询时间范围，起始时间
+        :type StartTime: str
+        :param EndTime: 查询时间范围，结束时间
+        :type EndTime: str
+        :param SourceIp: 来源IP，模糊查询
+        :type SourceIp: str
+        :param Entry: 登录入口：1-字符界面,2-图形界面，3-web页面, 4-API
+        :type Entry: int
+        :param Result: 操作结果，1-成功，2-失败
+        :type Result: int
+        :param Offset: 分页偏移位置，默认值为0
+        :type Offset: int
+        :param Limit: 分页每页记录数，默认20
+        :type Limit: int
+        """
+        self.UserName = None
+        self.RealName = None
+        self.StartTime = None
+        self.EndTime = None
+        self.SourceIp = None
+        self.Entry = None
+        self.Result = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.SourceIp = params.get("SourceIp")
+        self.Entry = params.get("Entry")
+        self.Result = params.get("Result")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeLoginEventResponse(AbstractModel):
+    """DescribeLoginEvent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param LoginEventSet: 登录日志列表
+        :type LoginEventSet: list of LoginEvent
+        :param TotalCount: 总记录数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.LoginEventSet = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("LoginEventSet") is not None:
+            self.LoginEventSet = []
+            for item in params.get("LoginEventSet"):
+                obj = LoginEvent()
+                obj._deserialize(item)
+                self.LoginEventSet.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeOperationEventRequest(AbstractModel):
+    """DescribeOperationEvent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserName: 用户名，如果不包含其他条件时对user_name or real_name两个字段模糊查询
+        :type UserName: str
+        :param RealName: 姓名，模糊查询
+        :type RealName: str
+        :param StartTime: 查询时间范围，起始时间
+        :type StartTime: str
+        :param EndTime: 查询时间范围，结束时间
+        :type EndTime: str
+        :param SourceIp: 来源IP，模糊查询
+        :type SourceIp: str
+        :param Kind: 操作类型，参考DescribeOperationType返回结果
+        :type Kind: int
+        :param Result: 操作结果，1-成功，2-失败
+        :type Result: int
+        :param Offset: 分页偏移位置，默认值为0
+        :type Offset: int
+        :param Limit: 分页每页记录数，默认20
+        :type Limit: int
+        """
+        self.UserName = None
+        self.RealName = None
+        self.StartTime = None
+        self.EndTime = None
+        self.SourceIp = None
+        self.Kind = None
+        self.Result = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.SourceIp = params.get("SourceIp")
+        self.Kind = params.get("Kind")
+        self.Result = params.get("Result")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeOperationEventResponse(AbstractModel):
+    """DescribeOperationEvent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param OperationEventSet: 操作日志列表
+        :type OperationEventSet: list of OperationEvent
+        :param TotalCount: 总记录数
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.OperationEventSet = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("OperationEventSet") is not None:
+            self.OperationEventSet = []
+            for item in params.get("OperationEventSet"):
+                obj = OperationEvent()
+                obj._deserialize(item)
+                self.OperationEventSet.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeResourcesRequest(AbstractModel):
     """DescribeResources请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2557,14 +2829,58 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class LoginEvent(AbstractModel):
+    """登录日志
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserName: 用户名
+        :type UserName: str
+        :param RealName: 姓名
+        :type RealName: str
+        :param Time: 操作时间
+        :type Time: str
+        :param SourceIp: 来源IP
+        :type SourceIp: str
+        :param Entry: 登录入口：1-字符界面,2-图形界面，3-web页面, 4-API
+        :type Entry: int
+        :param Result: 操作结果，1-成功，2-失败
+        :type Result: int
+        """
+        self.UserName = None
+        self.RealName = None
+        self.Time = None
+        self.SourceIp = None
+        self.Entry = None
+        self.Result = None
+
+
+    def _deserialize(self, params):
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.Time = params.get("Time")
+        self.SourceIp = params.get("SourceIp")
+        self.Entry = params.get("Entry")
+        self.Result = params.get("Result")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ModifyAclRequest(AbstractModel):
     """ModifyAcl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2881,14 +3197,62 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class OperationEvent(AbstractModel):
+    """操作日志
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserName: 用户名
+        :type UserName: str
+        :param RealName: 姓名
+        :type RealName: str
+        :param Time: 操作时间
+        :type Time: str
+        :param SourceIp: 来源IP
+        :type SourceIp: str
+        :param Kind: 操作类型
+        :type Kind: int
+        :param Operation: 具体操作内容
+        :type Operation: str
+        :param Result: 操作结果，1-成功，2-失败
+        :type Result: int
+        """
+        self.UserName = None
+        self.RealName = None
+        self.Time = None
+        self.SourceIp = None
+        self.Kind = None
+        self.Operation = None
+        self.Result = None
+
+
+    def _deserialize(self, params):
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.Time = params.get("Time")
+        self.SourceIp = params.get("SourceIp")
+        self.Kind = params.get("Kind")
+        self.Operation = params.get("Operation")
+        self.Result = params.get("Result")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ResetDeviceAccountPasswordRequest(AbstractModel):
     """ResetDeviceAccountPassword请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3139,14 +3503,982 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SearchAuditLogRequest(AbstractModel):
+    """SearchAuditLog请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param StartTime: 开始时间，不得早于当前时间的180天前
+        :type StartTime: str
+        :param EndTime: 结束时间
+        :type EndTime: str
+        :param Offset: 偏移量
+        :type Offset: int
+        :param Limit: 每页容量，默认为20，最大200
+        :type Limit: int
+        """
+        self.StartTime = None
+        self.EndTime = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchAuditLogResponse(AbstractModel):
+    """SearchAuditLog返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AuditLogSet: 审计日志
+        :type AuditLogSet: list of AuditLogResult
+        :param TotalCount: 日志总数量
+        :type TotalCount: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.AuditLogSet = None
+        self.TotalCount = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("AuditLogSet") is not None:
+            self.AuditLogSet = []
+            for item in params.get("AuditLogSet"):
+                obj = AuditLogResult()
+                obj._deserialize(item)
+                self.AuditLogSet.append(obj)
+        self.TotalCount = params.get("TotalCount")
+        self.RequestId = params.get("RequestId")
+
+
+class SearchCommandBySidRequest(AbstractModel):
+    """SearchCommandBySid请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Sid: 会话Id
+        :type Sid: str
+        :param Cmd: 命令，可模糊搜索
+        :type Cmd: str
+        :param Offset: 偏移量
+        :type Offset: int
+        :param Limit: 每页容量，默认20，最大200
+        :type Limit: int
+        :param AuditAction: 根据拦截状态进行过滤
+        :type AuditAction: list of int non-negative
+        """
+        self.Sid = None
+        self.Cmd = None
+        self.Offset = None
+        self.Limit = None
+        self.AuditAction = None
+
+
+    def _deserialize(self, params):
+        self.Sid = params.get("Sid")
+        self.Cmd = params.get("Cmd")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.AuditAction = params.get("AuditAction")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchCommandBySidResponse(AbstractModel):
+    """SearchCommandBySid返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总记录数
+        :type TotalCount: int
+        :param CommandSet: 命令列表
+        :type CommandSet: list of Command
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.CommandSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("CommandSet") is not None:
+            self.CommandSet = []
+            for item in params.get("CommandSet"):
+                obj = Command()
+                obj._deserialize(item)
+                self.CommandSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class SearchCommandRequest(AbstractModel):
+    """SearchCommand请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param StartTime: 搜索区间的开始时间
+        :type StartTime: str
+        :param EndTime: 搜索区间的结束时间，不填默认为开始时间到现在为止
+        :type EndTime: str
+        :param UserName: 用户名
+        :type UserName: str
+        :param RealName: 姓名
+        :type RealName: str
+        :param InstanceId: 资产实例ID
+        :type InstanceId: str
+        :param DeviceName: 资产名称
+        :type DeviceName: str
+        :param PublicIp: 资产的公网IP
+        :type PublicIp: str
+        :param PrivateIp: 资产的内网IP
+        :type PrivateIp: str
+        :param Cmd: 执行的命令
+        :type Cmd: str
+        :param AuditAction: 根据拦截状态进行过滤：1 - 已执行，2 - 被阻断
+        :type AuditAction: list of int non-negative
+        :param Limit: 每页容量，默认20，最大200
+        :type Limit: int
+        :param Offset: 分页偏移位置，默认值为0
+        :type Offset: int
+        """
+        self.StartTime = None
+        self.EndTime = None
+        self.UserName = None
+        self.RealName = None
+        self.InstanceId = None
+        self.DeviceName = None
+        self.PublicIp = None
+        self.PrivateIp = None
+        self.Cmd = None
+        self.AuditAction = None
+        self.Limit = None
+        self.Offset = None
+
+
+    def _deserialize(self, params):
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.InstanceId = params.get("InstanceId")
+        self.DeviceName = params.get("DeviceName")
+        self.PublicIp = params.get("PublicIp")
+        self.PrivateIp = params.get("PrivateIp")
+        self.Cmd = params.get("Cmd")
+        self.AuditAction = params.get("AuditAction")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchCommandResponse(AbstractModel):
+    """SearchCommand返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 总记录数
+        :type TotalCount: int
+        :param Commands: 命令列表
+        :type Commands: list of SearchCommandResult
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Commands = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Commands") is not None:
+            self.Commands = []
+            for item in params.get("Commands"):
+                obj = SearchCommandResult()
+                obj._deserialize(item)
+                self.Commands.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class SearchCommandResult(AbstractModel):
+    """命令执行检索结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Time: 命令输入的时间
+        :type Time: str
+        :param UserName: 用户名
+        :type UserName: str
+        :param RealName: 姓名
+        :type RealName: str
+        :param InstanceId: 资产ID
+        :type InstanceId: str
+        :param DeviceName: 资产名称
+        :type DeviceName: str
+        :param PublicIp: 资产公网IP
+        :type PublicIp: str
+        :param PrivateIp: 资产内网IP
+        :type PrivateIp: str
+        :param Cmd: 命令
+        :type Cmd: str
+        :param Action: 命令执行情况，1--允许，2--拒绝
+        :type Action: int
+        :param Sid: 命令所属的会话ID
+        :type Sid: str
+        :param TimeOffset: 命令执行时间相对于所属会话开始时间的偏移量，单位ms
+        :type TimeOffset: int
+        """
+        self.Time = None
+        self.UserName = None
+        self.RealName = None
+        self.InstanceId = None
+        self.DeviceName = None
+        self.PublicIp = None
+        self.PrivateIp = None
+        self.Cmd = None
+        self.Action = None
+        self.Sid = None
+        self.TimeOffset = None
+
+
+    def _deserialize(self, params):
+        self.Time = params.get("Time")
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.InstanceId = params.get("InstanceId")
+        self.DeviceName = params.get("DeviceName")
+        self.PublicIp = params.get("PublicIp")
+        self.PrivateIp = params.get("PrivateIp")
+        self.Cmd = params.get("Cmd")
+        self.Action = params.get("Action")
+        self.Sid = params.get("Sid")
+        self.TimeOffset = params.get("TimeOffset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchFileBySidRequest(AbstractModel):
+    """SearchFileBySid请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Sid: 若入参为Id，则其他入参字段不作为搜索依据，仅按照Id来搜索会话
+        :type Sid: str
+        :param AuditLog: 是否创建审计日志,通过查看按钮调用时为true,其他为false
+        :type AuditLog: bool
+        :param Limit: 分页的页内记录数，默认为20，最大200
+        :type Limit: int
+        :param FileName: 可填写路径名或文件名
+        :type FileName: str
+        :param Offset: 分页用偏移量
+        :type Offset: int
+        :param AuditAction: 1-已执行，  2-被阻断
+        :type AuditAction: int
+        :param TypeFilters: 以Protocol和Method为条件查询
+        :type TypeFilters: list of SearchFileTypeFilter
+        """
+        self.Sid = None
+        self.AuditLog = None
+        self.Limit = None
+        self.FileName = None
+        self.Offset = None
+        self.AuditAction = None
+        self.TypeFilters = None
+
+
+    def _deserialize(self, params):
+        self.Sid = params.get("Sid")
+        self.AuditLog = params.get("AuditLog")
+        self.Limit = params.get("Limit")
+        self.FileName = params.get("FileName")
+        self.Offset = params.get("Offset")
+        self.AuditAction = params.get("AuditAction")
+        if params.get("TypeFilters") is not None:
+            self.TypeFilters = []
+            for item in params.get("TypeFilters"):
+                obj = SearchFileTypeFilter()
+                obj._deserialize(item)
+                self.TypeFilters.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchFileBySidResponse(AbstractModel):
+    """SearchFileBySid返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 记录数
+        :type TotalCount: int
+        :param SearchFileBySidResult: 某会话的文件操作列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SearchFileBySidResult: list of SearchFileBySidResult
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.SearchFileBySidResult = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("SearchFileBySidResult") is not None:
+            self.SearchFileBySidResult = []
+            for item in params.get("SearchFileBySidResult"):
+                obj = SearchFileBySidResult()
+                obj._deserialize(item)
+                self.SearchFileBySidResult.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class SearchFileBySidResult(AbstractModel):
+    """文件操作搜索结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Time: 文件操作时间
+        :type Time: str
+        :param Method: 1-上传文件 2-下载文件 3-删除文件 4-移动文件 5-重命名文件 6-新建文件夹 7-移动文件夹 8-重命名文件夹 9-删除文件夹
+        :type Method: int
+        :param Protocol: 文件传输协议
+        :type Protocol: str
+        :param FileCurr: method为上传、下载、删除时文件在服务器上的位置, 或重命名、移动文件前文件的位置
+        :type FileCurr: str
+        :param FileNew: method为重命名、移动文件时代表移动后的新位置.其他情况为null
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileNew: str
+        :param Size: method为上传文件、下载文件、删除文件时显示文件大小。其他情况为null
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Size: int
+        :param Action: 堡垒机拦截情况, 1-已执行，  2-被阻断
+        :type Action: int
+        """
+        self.Time = None
+        self.Method = None
+        self.Protocol = None
+        self.FileCurr = None
+        self.FileNew = None
+        self.Size = None
+        self.Action = None
+
+
+    def _deserialize(self, params):
+        self.Time = params.get("Time")
+        self.Method = params.get("Method")
+        self.Protocol = params.get("Protocol")
+        self.FileCurr = params.get("FileCurr")
+        self.FileNew = params.get("FileNew")
+        self.Size = params.get("Size")
+        self.Action = params.get("Action")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchFileRequest(AbstractModel):
+    """SearchFile请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param StartTime: 查询开始时间
+        :type StartTime: str
+        :param EndTime: 查询结束时间
+        :type EndTime: str
+        :param UserName: 用户名
+        :type UserName: str
+        :param RealName: 姓名
+        :type RealName: str
+        :param InstanceId: 资产ID
+        :type InstanceId: str
+        :param DeviceName: 资产名称
+        :type DeviceName: str
+        :param PublicIp: 资产公网IP
+        :type PublicIp: str
+        :param PrivateIp: 资产内网IP
+        :type PrivateIp: str
+        :param Method: 操作类型：1 - 文件上传，2 - 文件下载，3 - 文件删除，4 - 文件(夹)移动，5 - 文件(夹)重命名，6 - 新建文件夹，9 - 删除文件夹
+        :type Method: list of int non-negative
+        :param FileName: 可填写路径名或文件（夹）名
+        :type FileName: str
+        :param AuditAction: 1-已执行，  2-被阻断
+        :type AuditAction: list of int non-negative
+        :param Limit: 分页的页内记录数，默认为20，最大200
+        :type Limit: int
+        :param Offset: 分页偏移位置，默认值为0
+        :type Offset: int
+        """
+        self.StartTime = None
+        self.EndTime = None
+        self.UserName = None
+        self.RealName = None
+        self.InstanceId = None
+        self.DeviceName = None
+        self.PublicIp = None
+        self.PrivateIp = None
+        self.Method = None
+        self.FileName = None
+        self.AuditAction = None
+        self.Limit = None
+        self.Offset = None
+
+
+    def _deserialize(self, params):
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.InstanceId = params.get("InstanceId")
+        self.DeviceName = params.get("DeviceName")
+        self.PublicIp = params.get("PublicIp")
+        self.PrivateIp = params.get("PrivateIp")
+        self.Method = params.get("Method")
+        self.FileName = params.get("FileName")
+        self.AuditAction = params.get("AuditAction")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchFileResponse(AbstractModel):
+    """SearchFile返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 记录数
+        :type TotalCount: int
+        :param Files: 文件操作列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Files: list of SearchFileResult
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Files = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Files") is not None:
+            self.Files = []
+            for item in params.get("Files"):
+                obj = SearchFileResult()
+                obj._deserialize(item)
+                self.Files.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class SearchFileResult(AbstractModel):
+    """文件传输检索结果
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Time: 文件传输的时间
+        :type Time: str
+        :param UserName: 用户名
+        :type UserName: str
+        :param RealName: 姓名
+        :type RealName: str
+        :param InstanceId: 资产ID
+        :type InstanceId: str
+        :param DeviceName: 资产名称
+        :type DeviceName: str
+        :param PublicIp: 资产公网IP
+        :type PublicIp: str
+        :param PrivateIp: 资产内网IP
+        :type PrivateIp: str
+        :param Action: 操作结果：1 - 已执行，2 - 已阻断
+        :type Action: int
+        :param Method: 操作类型：1 - 文件上传，2 - 文件下载，3 - 文件删除，4 - 文件(夹)移动，5 - 文件(夹)重命名，6 - 新建文件夹，9 - 删除文件夹
+        :type Method: int
+        :param FileCurr: 下载的文件（夹）路径及名称
+        :type FileCurr: str
+        :param FileNew: 上传或新建文件（夹）路径及名称
+        :type FileNew: str
+        """
+        self.Time = None
+        self.UserName = None
+        self.RealName = None
+        self.InstanceId = None
+        self.DeviceName = None
+        self.PublicIp = None
+        self.PrivateIp = None
+        self.Action = None
+        self.Method = None
+        self.FileCurr = None
+        self.FileNew = None
+
+
+    def _deserialize(self, params):
+        self.Time = params.get("Time")
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.InstanceId = params.get("InstanceId")
+        self.DeviceName = params.get("DeviceName")
+        self.PublicIp = params.get("PublicIp")
+        self.PrivateIp = params.get("PrivateIp")
+        self.Action = params.get("Action")
+        self.Method = params.get("Method")
+        self.FileCurr = params.get("FileCurr")
+        self.FileNew = params.get("FileNew")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchFileTypeFilter(AbstractModel):
+    """用于搜索文件传输记录等日志时按照protocol和method进行过滤
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Protocol: 需要查询的文件传输类型，如SFTP/CLIP/RDP/RZSZ
+        :type Protocol: str
+        :param Method: 在当前指定的protocol下进一步过滤具体操作类型,如剪贴板文件上传，剪贴板文件下载等
+        :type Method: list of int
+        """
+        self.Protocol = None
+        self.Method = None
+
+
+    def _deserialize(self, params):
+        self.Protocol = params.get("Protocol")
+        self.Method = params.get("Method")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchSessionCommandRequest(AbstractModel):
+    """SearchSessionCommand请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Cmd: 检索的目标命令，为模糊搜索
+        :type Cmd: str
+        :param StartTime: 开始时间，不得早于当前时间的180天前
+        :type StartTime: str
+        :param Offset: 分页偏移位置，默认值为0
+        :type Offset: int
+        :param Limit: 默认值为20，最大200
+        :type Limit: int
+        :param EndTime: 结束时间
+        :type EndTime: str
+        """
+        self.Cmd = None
+        self.StartTime = None
+        self.Offset = None
+        self.Limit = None
+        self.EndTime = None
+
+
+    def _deserialize(self, params):
+        self.Cmd = params.get("Cmd")
+        self.StartTime = params.get("StartTime")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.EndTime = params.get("EndTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchSessionCommandResponse(AbstractModel):
+    """SearchSessionCommand返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 记录总数
+        :type TotalCount: int
+        :param CommandSessionSet: 命令和所属会话
+        :type CommandSessionSet: list of SessionCommand
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.CommandSessionSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("CommandSessionSet") is not None:
+            self.CommandSessionSet = []
+            for item in params.get("CommandSessionSet"):
+                obj = SessionCommand()
+                obj._deserialize(item)
+                self.CommandSessionSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class SearchSessionRequest(AbstractModel):
+    """SearchSession请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PrivateIp: 内部Ip
+        :type PrivateIp: str
+        :param PublicIp: 外部Ip
+        :type PublicIp: str
+        :param UserName: 用户名，长度不超过20
+        :type UserName: str
+        :param Account: 账号，长度不超过64
+        :type Account: str
+        :param FromIp: 来源Ip
+        :type FromIp: str
+        :param StartTime: 搜索区间的开始时间。若入参是Id，则非必传，否则为必传。
+        :type StartTime: str
+        :param EndTime: 搜索区间的结束时间
+        :type EndTime: str
+        :param Kind: 会话协议类型，只能是1、2、3或4 对应关系为1-tui 2-gui 3-file 4-数据库。若入参是Id，则非必传，否则为必传。
+        :type Kind: int
+        :param Offset: 偏移量
+        :type Offset: int
+        :param Limit: 分页的页内记录数，默认为20，最大200
+        :type Limit: int
+        :param RealName: 姓名，长度不超过20
+        :type RealName: str
+        :param DeviceName: 主机名，长度不超过64
+        :type DeviceName: str
+        :param Status: 状态，1为活跃，2为结束，3为强制离线，4为其他错误
+        :type Status: int
+        :param Id: 若入参为Id，则其他入参字段不作为搜索依据，仅按照Id来搜索会话
+        :type Id: str
+        """
+        self.PrivateIp = None
+        self.PublicIp = None
+        self.UserName = None
+        self.Account = None
+        self.FromIp = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Kind = None
+        self.Offset = None
+        self.Limit = None
+        self.RealName = None
+        self.DeviceName = None
+        self.Status = None
+        self.Id = None
+
+
+    def _deserialize(self, params):
+        self.PrivateIp = params.get("PrivateIp")
+        self.PublicIp = params.get("PublicIp")
+        self.UserName = params.get("UserName")
+        self.Account = params.get("Account")
+        self.FromIp = params.get("FromIp")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.Kind = params.get("Kind")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.RealName = params.get("RealName")
+        self.DeviceName = params.get("DeviceName")
+        self.Status = params.get("Status")
+        self.Id = params.get("Id")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SearchSessionResponse(AbstractModel):
+    """SearchSession返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 记录数
+        :type TotalCount: int
+        :param SessionSet: 会话信息列表
+        :type SessionSet: list of SessionResult
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.SessionSet = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("SessionSet") is not None:
+            self.SessionSet = []
+            for item in params.get("SessionSet"):
+                obj = SessionResult()
+                obj._deserialize(item)
+                self.SessionSet.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class SessionCommand(AbstractModel):
+    """命令和所属会话
+
+    """
+
+    def __init__(self):
+        r"""
+        :param StartTime: 开始时间
+        :type StartTime: str
+        :param EndTime: 结束时间
+        :type EndTime: str
+        :param UserName: 用户名
+        :type UserName: str
+        :param RealName: 账号
+        :type RealName: str
+        :param DeviceName: 设备名
+        :type DeviceName: str
+        :param PrivateIp: 内部Ip
+        :type PrivateIp: str
+        :param PublicIp: 外部Ip
+        :type PublicIp: str
+        :param Commands: 命令列表
+        :type Commands: list of Command
+        :param Count: 记录数
+        :type Count: int
+        :param Id: 会话Id
+        :type Id: str
+        :param InstanceId: 设备id
+        :type InstanceId: str
+        :param ApCode: 设备所属的地域
+        :type ApCode: str
+        """
+        self.StartTime = None
+        self.EndTime = None
+        self.UserName = None
+        self.RealName = None
+        self.DeviceName = None
+        self.PrivateIp = None
+        self.PublicIp = None
+        self.Commands = None
+        self.Count = None
+        self.Id = None
+        self.InstanceId = None
+        self.ApCode = None
+
+
+    def _deserialize(self, params):
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.DeviceName = params.get("DeviceName")
+        self.PrivateIp = params.get("PrivateIp")
+        self.PublicIp = params.get("PublicIp")
+        if params.get("Commands") is not None:
+            self.Commands = []
+            for item in params.get("Commands"):
+                obj = Command()
+                obj._deserialize(item)
+                self.Commands.append(obj)
+        self.Count = params.get("Count")
+        self.Id = params.get("Id")
+        self.InstanceId = params.get("InstanceId")
+        self.ApCode = params.get("ApCode")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SessionResult(AbstractModel):
+    """搜索字符或图形会话时返回的SessionResul结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserName: 用户名
+        :type UserName: str
+        :param RealName: 姓名
+        :type RealName: str
+        :param Account: 主机账号
+        :type Account: str
+        :param StartTime: 开始时间
+        :type StartTime: str
+        :param EndTime: 结束时间
+        :type EndTime: str
+        :param Size: 会话大小
+        :type Size: int
+        :param InstanceId: 设备ID
+        :type InstanceId: str
+        :param DeviceName: 设备名
+        :type DeviceName: str
+        :param PrivateIp: 内部Ip
+        :type PrivateIp: str
+        :param PublicIp: 外部Ip
+        :type PublicIp: str
+        :param FromIp: 来源Ip
+        :type FromIp: str
+        :param Duration: 会话持续时长
+        :type Duration: float
+        :param Count: 该会话内命令数量 ，搜索图形会话时该字段无意义
+        :type Count: int
+        :param DangerCount: 该会话内高危命令数，搜索图形时该字段无意义
+        :type DangerCount: int
+        :param Status: 会话状态，如1会话活跃  2会话结束  3强制离线  4其他错误
+        :type Status: int
+        :param Id: 会话Id
+        :type Id: str
+        :param ApCode: 设备所属的地域
+        :type ApCode: str
+        :param Protocol: 会话协议
+        :type Protocol: str
+        """
+        self.UserName = None
+        self.RealName = None
+        self.Account = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Size = None
+        self.InstanceId = None
+        self.DeviceName = None
+        self.PrivateIp = None
+        self.PublicIp = None
+        self.FromIp = None
+        self.Duration = None
+        self.Count = None
+        self.DangerCount = None
+        self.Status = None
+        self.Id = None
+        self.ApCode = None
+        self.Protocol = None
+
+
+    def _deserialize(self, params):
+        self.UserName = params.get("UserName")
+        self.RealName = params.get("RealName")
+        self.Account = params.get("Account")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.Size = params.get("Size")
+        self.InstanceId = params.get("InstanceId")
+        self.DeviceName = params.get("DeviceName")
+        self.PrivateIp = params.get("PrivateIp")
+        self.PublicIp = params.get("PublicIp")
+        self.FromIp = params.get("FromIp")
+        self.Duration = params.get("Duration")
+        self.Count = params.get("Count")
+        self.DangerCount = params.get("DangerCount")
+        self.Status = params.get("Status")
+        self.Id = params.get("Id")
+        self.ApCode = params.get("ApCode")
+        self.Protocol = params.get("Protocol")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class TagFilter(AbstractModel):
     """资产标签
 
     """
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -712,14 +712,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeLoginEvent(self, request):
+        """查询登录日志
+
+        :param request: Request instance for DescribeLoginEvent.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeLoginEventRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.DescribeLoginEventResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLoginEvent", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLoginEventResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeOperationEvent(self, request):
+        """查询操作日志
+
+        :param request: Request instance for DescribeOperationEvent.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeOperationEventRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.DescribeOperationEventResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeOperationEvent", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeOperationEventResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeResources(self, request):
         """查询用户购买的堡垒机服务信息，包括资源ID、授权点数、VPC、过期时间等。
 
         :param request: Request instance for DescribeResources.
         :type request: :class:`tencentcloud.dasb.v20191018.models.DescribeResourcesRequest`
         :rtype: :class:`tencentcloud.dasb.v20191018.models.DescribeResourcesResponse`
 
@@ -985,8 +1031,169 @@
             model = models.ResetUserResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SearchAuditLog(self, request):
+        """搜索审计日志
+
+        :param request: Request instance for SearchAuditLog.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.SearchAuditLogRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.SearchAuditLogResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SearchAuditLog", params, headers=headers)
+            response = json.loads(body)
+            model = models.SearchAuditLogResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SearchCommand(self, request):
+        """命令执行检索
+
+        :param request: Request instance for SearchCommand.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.SearchCommandRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.SearchCommandResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SearchCommand", params, headers=headers)
+            response = json.loads(body)
+            model = models.SearchCommandResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SearchCommandBySid(self, request):
+        """根据会话Id搜索Command
+
+        :param request: Request instance for SearchCommandBySid.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.SearchCommandBySidRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.SearchCommandBySidResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SearchCommandBySid", params, headers=headers)
+            response = json.loads(body)
+            model = models.SearchCommandBySidResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SearchFile(self, request):
+        """文件传输检索
+
+        :param request: Request instance for SearchFile.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.SearchFileRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.SearchFileResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SearchFile", params, headers=headers)
+            response = json.loads(body)
+            model = models.SearchFileResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SearchFileBySid(self, request):
+        """搜索文件传输会话下文件操作列表
+
+        :param request: Request instance for SearchFileBySid.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.SearchFileBySidRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.SearchFileBySidResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SearchFileBySid", params, headers=headers)
+            response = json.loads(body)
+            model = models.SearchFileBySidResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SearchSession(self, request):
+        """搜索会话
+
+        :param request: Request instance for SearchSession.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.SearchSessionRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.SearchSessionResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SearchSession", params, headers=headers)
+            response = json.loads(body)
+            model = models.SearchSessionResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SearchSessionCommand(self, request):
+        """命令检索
+
+        :param request: Request instance for SearchSessionCommand.
+        :type request: :class:`tencentcloud.dasb.v20191018.models.SearchSessionCommandRequest`
+        :rtype: :class:`tencentcloud.dasb.v20191018.models.SearchSessionCommandResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SearchSessionCommand", params, headers=headers)
+            response = json.loads(body)
+            model = models.SearchSessionCommandResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.869/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-dasb-3.0.870/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.869/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.870/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.869/README.rst` & `tencentcloud-sdk-python-dasb-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.869/setup.py` & `tencentcloud-sdk-python-dasb-3.0.870/setup.py`

 * *Files identical despite different names*

