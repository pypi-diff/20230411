# Comparing `tmp/tencentcloud-sdk-python-mongodb-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-mongodb-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.869.tar", last modified: Mon Apr 10 03:09:41 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mongodb-3.0.870.tar", last modified: Tue Apr 11 03:43:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mongodb-3.0.869.tar` & `tencentcloud-sdk-python-mongodb-3.0.870.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/
--rw-r--r--   0 root         (0) root         (0)    46677 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13571 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/
--rw-r--r--   0 root         (0) root         (0)   147320 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35476 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)     7304 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:09:41.000000 tencentcloud-sdk-python-mongodb-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    46677 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13571 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20180408/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20190725/
+-rw-r--r--   0 root         (0) root         (0)   149931 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20190725/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20190725/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36443 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20190725/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)     7304 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20190725/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud_sdk_python_mongodb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud_sdk_python_mongodb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud_sdk_python_mongodb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:43:11.000000 tencentcloud-sdk-python-mongodb-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.870/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/models.py` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20180408/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20180408/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/models.py` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20190725/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,19 +350,21 @@
 class CreateBackupDBInstanceRequest(AbstractModel):
     """CreateBackupDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例id
+        :param InstanceId: 实例 ID。例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
         :type InstanceId: str
-        :param BackupMethod: 0-逻辑备份，1-物理备份
+        :param BackupMethod: 设置备份方式。
+- 0：逻辑备份。
+- 1：物理备份。
         :type BackupMethod: int
-        :param BackupRemark: 备份备注
+        :param BackupRemark: 备份备注信息。
         :type BackupRemark: str
         """
         self.InstanceId = None
         self.BackupMethod = None
         self.BackupRemark = None
 
 
@@ -382,15 +384,15 @@
 class CreateBackupDBInstanceResponse(AbstractModel):
     """CreateBackupDBInstance返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param AsyncRequestId: 查询备份流程的状态
+        :param AsyncRequestId: 查询备份流程的状态。
         :type AsyncRequestId: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.AsyncRequestId = None
         self.RequestId = None
 
@@ -934,14 +936,68 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DeleteAccountUserRequest(AbstractModel):
+    """DeleteAccountUser请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 指定待删除账号的实例 ID。例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
+
+        :type InstanceId: str
+        :param UserName: 配置待删除的账号名。
+        :type UserName: str
+        :param MongoUserPassword: 配置 mongouser 对应的密码。mongouser为系统默认账号，输入其对应的密码。
+        :type MongoUserPassword: str
+        """
+        self.InstanceId = None
+        self.UserName = None
+        self.MongoUserPassword = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.UserName = params.get("UserName")
+        self.MongoUserPassword = params.get("MongoUserPassword")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteAccountUserResponse(AbstractModel):
+    """DeleteAccountUser返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 账户删除任务ID。
+        :type FlowId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeAccountUsersRequest(AbstractModel):
     """DescribeAccountUsers请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1607,15 +1663,15 @@
 class DescribeInstanceParamsRequest(AbstractModel):
     """DescribeInstanceParams请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID
+        :param InstanceId: 指定待查询参数列表的实例ID。例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
         :type InstanceId: str
         """
         self.InstanceId = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
@@ -1631,21 +1687,21 @@
 class DescribeInstanceParamsResponse(AbstractModel):
     """DescribeInstanceParams返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceEnumParam: 值为枚举类型参数集合
+        :param InstanceEnumParam: 参数值为枚举类型参数集合。
         :type InstanceEnumParam: list of InstanceEnumParam
-        :param InstanceIntegerParam: 值为integer类型参数集合
+        :param InstanceIntegerParam: 参数值为 Integer 类型参数集合。
         :type InstanceIntegerParam: list of InstanceIntegerParam
-        :param InstanceTextParam: 值为text类型的参数集合
+        :param InstanceTextParam: 参数值为 Text 类型的参数集合。
         :type InstanceTextParam: list of InstanceTextParam
-        :param InstanceMultiParam: 值为混合类型的参数集合
+        :param InstanceMultiParam: 参数值为混合类型的参数集合。
         :type InstanceMultiParam: list of InstanceMultiParam
         :param TotalCount: 当前实例支持修改的参数个数统计 如0
         :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.InstanceEnumParam = None
@@ -2482,29 +2538,33 @@
 class InstanceEnumParam(AbstractModel):
     """实例可修改参数枚举类型集合。
 
     """
 
     def __init__(self):
         r"""
-        :param CurrentValue: 参数当前值
+        :param CurrentValue: 参数当前值。
         :type CurrentValue: str
-        :param DefaultValue: 默认值
+        :param DefaultValue: 参数默认值。
         :type DefaultValue: str
-        :param EnumValue: 枚举值，所有支持的值
+        :param EnumValue: 枚举值，所有支持的值。
         :type EnumValue: list of str
-        :param NeedRestart: 是否需要重启生效 1:需要重启后生效；0：无需重启，设置成功即可生效；
+        :param NeedRestart: 参数修改之后是否需要重启生效。
+- 1：需要重启后生效。
+- 0：无需重启，设置成功即可生效。
         :type NeedRestart: str
-        :param ParamName: 参数名称
+        :param ParamName: 参数名称。
         :type ParamName: str
-        :param Tips: 中英文说明
+        :param Tips: 参数说明。
         :type Tips: list of str
-        :param ValueType: 参数值类型说明
+        :param ValueType: 参数值类型说明。
         :type ValueType: str
-        :param Status: 是否为运行中参数值 1:运行中参数值；0：非运行中参数值；
+        :param Status: 是否为运行中参数值。
+- 1：运行中参数值。
+- 0：非运行中参数值。
         :type Status: int
         """
         self.CurrentValue = None
         self.DefaultValue = None
         self.EnumValue = None
         self.NeedRestart = None
         self.ParamName = None
@@ -2528,39 +2588,43 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class InstanceIntegerParam(AbstractModel):
-    """实例可修改参数integer类型集合。
+    """实例可修改参数 Integer 类型集合。
 
     """
 
     def __init__(self):
         r"""
-        :param CurrentValue: 当前值
+        :param CurrentValue: 参数当前值。
         :type CurrentValue: str
-        :param DefaultValue: 默认值
+        :param DefaultValue: 参数默认值。
         :type DefaultValue: str
-        :param Max: 最大值
+        :param Max: 参数最大值。
         :type Max: str
-        :param Min: 最小值
+        :param Min: 最小值。
         :type Min: str
-        :param NeedRestart: 是否需要重启生效 1:需要重启后生效；0：无需重启，设置成功即可生效；
+        :param NeedRestart: 参数修改之后是否需要重启生效。
+- 1:需要重启后生效。
+- 0：无需重启，设置成功即可生效。
         :type NeedRestart: str
-        :param ParamName: 参数名称
+        :param ParamName: 参数名称。
         :type ParamName: str
-        :param Tips: 参数说明
+        :param Tips: 参数说明。
         :type Tips: list of str
-        :param ValueType: 参数类型
+        :param ValueType: 参数类型。
         :type ValueType: str
-        :param Status: 是否为运行中参数值 1:运行中参数值；0：非运行中参数值；
+        :param Status: 是否为运行中参数值。
+- 1：运行中参数值。
+- 0：非运行中参数值。
         :type Status: int
-        :param Unit: 冗余字段，可忽略
+        :param Unit: 冗余字段，可忽略。
         :type Unit: str
         """
         self.CurrentValue = None
         self.DefaultValue = None
         self.Max = None
         self.Min = None
         self.NeedRestart = None
@@ -2594,29 +2658,33 @@
 class InstanceMultiParam(AbstractModel):
     """实例可修改参数Multi类型集合。
 
     """
 
     def __init__(self):
         r"""
-        :param CurrentValue: 当前值
+        :param CurrentValue: 参数当前值。
         :type CurrentValue: str
-        :param DefaultValue: 默认值
+        :param DefaultValue: 参数默认值。
         :type DefaultValue: str
-        :param EnumValue: 指导值范围
+        :param EnumValue: 参考值范围。
         :type EnumValue: list of str
-        :param NeedRestart: 是否需要重启生效 1:需要重启后生效；0：无需重启，设置成功即可生效；
+        :param NeedRestart: 参数修改后是否需要重启才会生效。
+- 1：需要重启后生效。
+- 0：无需重启，设置成功即可生效。
         :type NeedRestart: str
-        :param ParamName: 参数名称
+        :param ParamName: 参数名称。
         :type ParamName: str
-        :param Status: 是否为运行中参数值 1:运行中参数值；0：非运行中参数值；
+        :param Status: 是否为运行中参数值。
+- 1：运行中参数值。
+- 0：非运行中参数值。
         :type Status: int
-        :param Tips: 参数说明
+        :param Tips: 参数说明。
         :type Tips: list of str
-        :param ValueType: 当前值的类型描述，默认为multi
+        :param ValueType: 当前值的类型描述，默认为multi。
         :type ValueType: str
         """
         self.CurrentValue = None
         self.DefaultValue = None
         self.EnumValue = None
         self.NeedRestart = None
         self.ParamName = None
@@ -2640,35 +2708,37 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class InstanceTextParam(AbstractModel):
-    """实例可修改参数text类型集合。
+    """实例可修改参数为 Text 类型的参数集合。
 
     """
 
     def __init__(self):
         r"""
-        :param CurrentValue: 当前值
+        :param CurrentValue: 参数当前值。
         :type CurrentValue: str
-        :param DefaultValue: 默认值
+        :param DefaultValue: 参数默认值。
         :type DefaultValue: str
-        :param NeedRestart: 是否需要重启
+        :param NeedRestart: 修改参数值之后是否需要重启。
         :type NeedRestart: str
-        :param ParamName: 参数名称
+        :param ParamName: 参数名称。
         :type ParamName: str
-        :param TextValue: text类型值
+        :param TextValue: Text 类型参数对应的值。
         :type TextValue: str
-        :param Tips: 参数说明
+        :param Tips: 参数说明。
         :type Tips: list of str
-        :param ValueType: 值类型说明
+        :param ValueType: 参数值类型说明。
         :type ValueType: str
-        :param Status: 是否为运行中参数值 1:运行中参数值；0：非运行中参数值；
+        :param Status: 是否为运行中的参数值。
+- 1：运行中参数值。
+- 0：非运行中参数值。
         :type Status: str
         """
         self.CurrentValue = None
         self.DefaultValue = None
         self.NeedRestart = None
         self.ParamName = None
         self.TextValue = None
@@ -3493,19 +3563,19 @@
 class SetAccountUserPrivilegeRequest(AbstractModel):
     """SetAccountUserPrivilege请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param InstanceId: 实例ID。
+        :param InstanceId: 指定待设置账号的实例ID。例如：cmgo-p8vn****。请登录 [MongoDB 控制台](https://console.cloud.tencent.com/mongodb)在实例列表复制实例 ID。
         :type InstanceId: str
-        :param UserName: 账号名称。
+        :param UserName: 设置账号名称。
         :type UserName: str
-        :param AuthRole: 权限信息。
+        :param AuthRole: 设置权限信息。
         :type AuthRole: list of Auth
         """
         self.InstanceId = None
         self.UserName = None
         self.AuthRole = None
 
 
@@ -3530,15 +3600,15 @@
 class SetAccountUserPrivilegeResponse(AbstractModel):
     """SetAccountUserPrivilege返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param FlowId: 设置任务ID,用于查询是否设置完成
+        :param FlowId: 任务ID。
         :type FlowId: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.FlowId = None
         self.RequestId = None
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/mongodb_client.py` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20190725/mongodb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateBackupDBInstance(self, request):
-        """备份实例接口
+        """本接口（CreateBackupDBInstance）用于备份实例。
 
         :param request: Request instance for CreateBackupDBInstance.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.CreateBackupDBInstanceRequest`
         :rtype: :class:`tencentcloud.mongodb.v20190725.models.CreateBackupDBInstanceResponse`
 
         """
         try:
@@ -160,14 +160,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteAccountUser(self, request):
+        """本接口（DeleteAccountUser）用于删除实例的自定义账号。
+
+        :param request: Request instance for DeleteAccountUser.
+        :type request: :class:`tencentcloud.mongodb.v20190725.models.DeleteAccountUserRequest`
+        :rtype: :class:`tencentcloud.mongodb.v20190725.models.DeleteAccountUserResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteAccountUser", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteAccountUserResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeAccountUsers(self, request):
         """本接口（DescribeAccountUsers）用于获取当前实例的全部账号。
 
         :param request: Request instance for DescribeAccountUsers.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeAccountUsersRequest`
         :rtype: :class:`tencentcloud.mongodb.v20190725.models.DescribeAccountUsersResponse`
 
@@ -368,15 +391,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeInstanceParams(self, request):
-        """本接口(DescribeInstanceParams)用于查询当前实例可修改的参数列表。
+        """本接口（DescribeInstanceParams）用于查询当前实例可修改的参数列表。
 
         :param request: Request instance for DescribeInstanceParams.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.DescribeInstanceParamsRequest`
         :rtype: :class:`tencentcloud.mongodb.v20190725.models.DescribeInstanceParamsResponse`
 
         """
         try:
@@ -782,15 +805,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def SetAccountUserPrivilege(self, request):
-        """本接口(SetAccountUserPrivilege)用于设置mongodb实例的账号权限。
+        """本接口（SetAccountUserPrivilege）用于设置实例的账号权限。
 
         :param request: Request instance for SetAccountUserPrivilege.
         :type request: :class:`tencentcloud.mongodb.v20190725.models.SetAccountUserPrivilegeRequest`
         :rtype: :class:`tencentcloud.mongodb.v20190725.models.SetAccountUserPrivilegeResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud/mongodb/v20190725/errorcodes.py` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud/mongodb/v20190725/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud_sdk_python_mongodb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mongodb
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Mongodb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-mongodb-3.0.870/tencentcloud_sdk_python_mongodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/README.rst` & `tencentcloud-sdk-python-mongodb-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mongodb-3.0.869/setup.py` & `tencentcloud-sdk-python-mongodb-3.0.870/setup.py`

 * *Files identical despite different names*

