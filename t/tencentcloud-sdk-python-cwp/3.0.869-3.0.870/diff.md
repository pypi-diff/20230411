# Comparing `tmp/tencentcloud-sdk-python-cwp-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-cwp-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.869.tar", last modified: Mon Apr 10 02:59:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cwp-3.0.870.tar", last modified: Tue Apr 11 03:28:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cwp-3.0.869.tar` & `tencentcloud-sdk-python-cwp-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)   900650 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250495 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)     3900 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:59:44.000000 tencentcloud-sdk-python-cwp-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:59:45.000000 tencentcloud-sdk-python-cwp-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)   900743 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250501 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:28:19.000000 tencentcloud-sdk-python-cwp-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.870/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4106,15 +4106,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: 数据ID
         :type Id: int
-        :param Uuid: 云镜ID
+        :param Uuid: 主机安全ID
         :type Uuid: str
         :param Quuid: 主机ID
         :type Quuid: str
         :param Hostip: 主机内网IP
         :type Hostip: str
         :param User: 执行用户名
         :type User: str
@@ -4208,15 +4208,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: 数据ID
         :type Id: int
-        :param Uuid: 云镜ID
+        :param Uuid: 主机安全ID
         :type Uuid: str
         :param Quuid: 主机ID
         :type Quuid: str
         :param HostIp: 主机内网IP
         :type HostIp: str
         :param User: 执行用户名
         :type User: str
@@ -4322,15 +4322,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: 数据ID
         :type Id: int
-        :param Uuid: 云镜ID
+        :param Uuid: 主机安全ID
         :type Uuid: str
         :param Quuid: 主机ID
         :type Quuid: str
         :param HostIp: 主机内网IP
         :type HostIp: str
         :param Platform: 平台类型
         :type Platform: int
@@ -4548,15 +4548,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: 唯一Id
         :type Id: int
-        :param Uuid: 云镜客户端唯一标识UUID
+        :param Uuid: 主机安全客户端唯一标识UUID
 注意：此字段可能返回 null，表示取不到有效值。
         :type Uuid: str
         :param MachineIp: 主机ip
 注意：此字段可能返回 null，表示取不到有效值。
         :type MachineIp: str
         :param MachineName: 主机名
 注意：此字段可能返回 null，表示取不到有效值。
@@ -5917,15 +5917,15 @@
 class DeleteMachineRequest(AbstractModel):
     """DeleteMachine请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Uuid: 云镜客户端Uuid。
+        :param Uuid: 主机安全客户端Uuid。
         :type Uuid: str
         """
         self.Uuid = None
 
 
     def _deserialize(self, params):
         self.Uuid = params.get("Uuid")
@@ -13765,15 +13765,15 @@
 class DescribeMachineInfoRequest(AbstractModel):
     """DescribeMachineInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Uuid: 云镜客户端唯一Uuid。
+        :param Uuid: 主机安全客户端唯一Uuid。
         :type Uuid: str
         :param Quuid: Quuid , Uuid 必填一项
         :type Quuid: str
         """
         self.Uuid = None
         self.Quuid = None
 
@@ -13795,15 +13795,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param MachineIp: 机器ip。
         :type MachineIp: str
-        :param ProtectDays: 受云镜保护天数。
+        :param ProtectDays: 受主机安全保护天数。
         :type ProtectDays: int
         :param MachineOs: 操作系统。
         :type MachineOs: str
         :param MachineName: 主机名称。
         :type MachineName: str
         :param MachineStatus: 在线状态。
 <li>ONLINE： 在线</li>
@@ -13811,15 +13811,15 @@
         :type MachineStatus: str
         :param InstanceId: CVM或BM主机唯一标识。
         :type InstanceId: str
         :param MachineWanIp: 主机外网IP。
         :type MachineWanIp: str
         :param Quuid: CVM或BM主机唯一Uuid。
         :type Quuid: str
-        :param Uuid: 云镜客户端唯一Uuid。
+        :param Uuid: 主机安全客户端唯一Uuid。
         :type Uuid: str
         :param IsProVersion: 是否开通专业版。
 <li>true：是</li>
 <li>false：否</li>
         :type IsProVersion: bool
         :param ProVersionOpenDate: 专业版开通时间。
         :type ProVersionOpenDate: str
@@ -13842,15 +13842,15 @@
         :type FreeVulsLeft: int
         :param AgentVersion: agent版本号
         :type AgentVersion: str
         :param ProVersionDeadline: 专业版到期时间(仅预付费)
         :type ProVersionDeadline: str
         :param HasAssetScan: 是否有资产扫描记录，0无，1有
         :type HasAssetScan: int
-        :param ProtectType: 防护版本 BASIC_VERSION 基础版, PRO_VERSION 专业版 Flagship 旗舰版.
+        :param ProtectType: 防护版本：BASIC_VERSION 基础版，PRO_VERSION 专业版，Flagship 旗舰版，GENERAL_DISCOUNT 普惠版
         :type ProtectType: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.MachineIp = None
         self.ProtectDays = None
         self.MachineOs = None
@@ -17143,15 +17143,15 @@
 class DescribeUsualLoginPlacesRequest(AbstractModel):
     """DescribeUsualLoginPlaces请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Uuid: 云镜客户端UUID
+        :param Uuid: 主机安全客户端UUID
         :type Uuid: str
         """
         self.Uuid = None
 
 
     def _deserialize(self, params):
         self.Uuid = params.get("Uuid")
@@ -20663,15 +20663,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param Id: 唯一ID。
         :type Id: int
-        :param Uuid: 云镜客户端唯一Uuid。
+        :param Uuid: 主机安全客户端唯一Uuid。
         :type Uuid: str
         :param MachineIp: 主机内网IP。
         :type MachineIp: str
         :param MachineName: 主机名。
         :type MachineName: str
         :param Username: 帐号名。
         :type Username: str
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,15 +509,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteMachine(self, request):
-        """本接口（DeleteMachine）用于卸载云镜客户端。
+        """本接口（DeleteMachine）用于卸载主机安全客户端。
 
         :param request: Request instance for DeleteMachine.
         :type request: :class:`tencentcloud.cwp.v20180228.models.DeleteMachineRequest`
         :rtype: :class:`tencentcloud.cwp.v20180228.models.DeleteMachineResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cwp-3.0.869/README.rst` & `tencentcloud-sdk-python-cwp-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cwp-3.0.869/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cwp-3.0.870/tencentcloud_sdk_python_cwp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cwp
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cwp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cwp-3.0.869/setup.py` & `tencentcloud-sdk-python-cwp-3.0.870/setup.py`

 * *Files identical despite different names*

