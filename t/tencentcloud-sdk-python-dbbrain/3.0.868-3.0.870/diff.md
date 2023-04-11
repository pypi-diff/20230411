# Comparing `tmp/tencentcloud-sdk-python-dbbrain-3.0.868.tar.gz` & `tmp/tencentcloud-sdk-python-dbbrain-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.868.tar", last modified: Fri Apr  7 00:26:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dbbrain-3.0.870.tar", last modified: Tue Apr 11 03:31:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dbbrain-3.0.868.tar` & `tencentcloud-sdk-python-dbbrain-3.0.870.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)    27659 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20191016/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)   111297 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20191016/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)    43983 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)   164841 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20210527/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20210527/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud_sdk_python_dbbrain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      663 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/README.rst
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-07 00:26:38.000000 tencentcloud-sdk-python-dbbrain-3.0.868/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)    27659 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)   111297 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)    45821 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)   171969 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      663 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:31:56.000000 tencentcloud-sdk-python-dbbrain-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.870/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.868
+Version: 3.0.870
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.868'
+__version__ = '3.0.870'
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteDBDiagReportTasks(self, request):
+        """根据任务id删除健康报告生成任务
+
+        :param request: Request instance for DeleteDBDiagReportTasks.
+        :type request: :class:`tencentcloud.dbbrain.v20210527.models.DeleteDBDiagReportTasksRequest`
+        :rtype: :class:`tencentcloud.dbbrain.v20210527.models.DeleteDBDiagReportTasksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteDBDiagReportTasks", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteDBDiagReportTasksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteSecurityAuditLogExportTasks(self, request):
         """删除安全审计日志导出任务。
 
         :param request: Request instance for DeleteSecurityAuditLogExportTasks.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DeleteSecurityAuditLogExportTasksRequest`
         :rtype: :class:`tencentcloud.dbbrain.v20210527.models.DeleteSecurityAuditLogExportTasksResponse`
 
@@ -779,14 +802,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeSlowLogs(self, request):
+        """获取指定时间内某个sql模版的慢日志明细
+
+        :param request: Request instance for DescribeSlowLogs.
+        :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSlowLogsRequest`
+        :rtype: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSlowLogsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeSlowLogs", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeSlowLogsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSqlFilters(self, request):
         """查询实例SQL限流任务列表。
 
         :param request: Request instance for DescribeSqlFilters.
         :type request: :class:`tencentcloud.dbbrain.v20210527.models.DescribeSqlFiltersRequest`
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,14 +653,68 @@
 
 
     def _deserialize(self, params):
         self.FilterId = params.get("FilterId")
         self.RequestId = params.get("RequestId")
 
 
+class DeleteDBDiagReportTasksRequest(AbstractModel):
+    """DeleteDBDiagReportTasks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AsyncRequestIds: 需要删除的任务id列表
+        :type AsyncRequestIds: list of int
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        :param Product: 服务产品类型，支持值包括： "mysql" - 云数据库 MySQL， "cynosdb" - 云数据库 CynosDB for MySQL， "mongodb" - 云数据库 CynosDB for MySQL，
+默认值为"mysql"。
+        :type Product: str
+        """
+        self.AsyncRequestIds = None
+        self.InstanceId = None
+        self.Product = None
+
+
+    def _deserialize(self, params):
+        self.AsyncRequestIds = params.get("AsyncRequestIds")
+        self.InstanceId = params.get("InstanceId")
+        self.Product = params.get("Product")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteDBDiagReportTasksResponse(AbstractModel):
+    """DeleteDBDiagReportTasks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: 任务删除状态, 0-删除成功
+        :type Status: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Status = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteSecurityAuditLogExportTasksRequest(AbstractModel):
     """DeleteSecurityAuditLogExportTasks请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2260,14 +2314,112 @@
             for item in params.get("Items"):
                 obj = SlowLogHost()
                 obj._deserialize(item)
                 self.Items.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeSlowLogsRequest(AbstractModel):
+    """DescribeSlowLogs请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Product: 服务产品类型，支持值包括： "mysql" - 云数据库 MySQL， "cynosdb" - 云数据库 CynosDB for MySQL，默认为"mysql"。
+        :type Product: str
+        :param InstanceId: 实例id。
+        :type InstanceId: str
+        :param Md5: sql模版的md5值
+        :type Md5: str
+        :param StartTime: 开始时间，如“2019-09-10 12:13:14”。
+        :type StartTime: str
+        :param EndTime: 截止时间，如“2019-09-11 10:13:14”，截止时间与开始时间的间隔小于7天。
+        :type EndTime: str
+        :param Offset: 分页参数
+        :type Offset: int
+        :param Limit: 分页参数
+        :type Limit: int
+        :param DB: 数据库列表
+        :type DB: list of str
+        :param Key: 关键字
+        :type Key: list of str
+        :param User: 用户
+        :type User: list of str
+        :param Ip: ip
+        :type Ip: list of str
+        :param Time: 耗时区间,耗时区间的左右边界分别对应数组的第0个元素和第一个元素
+        :type Time: list of int
+        """
+        self.Product = None
+        self.InstanceId = None
+        self.Md5 = None
+        self.StartTime = None
+        self.EndTime = None
+        self.Offset = None
+        self.Limit = None
+        self.DB = None
+        self.Key = None
+        self.User = None
+        self.Ip = None
+        self.Time = None
+
+
+    def _deserialize(self, params):
+        self.Product = params.get("Product")
+        self.InstanceId = params.get("InstanceId")
+        self.Md5 = params.get("Md5")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.DB = params.get("DB")
+        self.Key = params.get("Key")
+        self.User = params.get("User")
+        self.Ip = params.get("Ip")
+        self.Time = params.get("Time")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeSlowLogsResponse(AbstractModel):
+    """DescribeSlowLogs返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TotalCount: 符合条件的记录总数。
+        :type TotalCount: int
+        :param Rows: 慢日志明细
+        :type Rows: list of SlowLogInfoItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TotalCount = None
+        self.Rows = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TotalCount = params.get("TotalCount")
+        if params.get("Rows") is not None:
+            self.Rows = []
+            for item in params.get("Rows"):
+                obj = SlowLogInfoItem()
+                obj._deserialize(item)
+                self.Rows.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeSqlFiltersRequest(AbstractModel):
     """DescribeSqlFilters请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4248,14 +4400,75 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class SlowLogInfoItem(AbstractModel):
+    """慢日志详细信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Timestamp: 慢日志开始时间
+        :type Timestamp: str
+        :param SqlText: sql语句
+        :type SqlText: str
+        :param Database: 数据库
+        :type Database: str
+        :param UserName: User来源
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserName: str
+        :param UserHost: IP来源
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserHost: str
+        :param QueryTime: 执行时间,单位秒
+        :type QueryTime: int
+        :param LockTime: 锁时间,单位秒
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LockTime: int
+        :param RowsExamined: 扫描行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RowsExamined: int
+        :param RowsSent: 返回行数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RowsSent: int
+        """
+        self.Timestamp = None
+        self.SqlText = None
+        self.Database = None
+        self.UserName = None
+        self.UserHost = None
+        self.QueryTime = None
+        self.LockTime = None
+        self.RowsExamined = None
+        self.RowsSent = None
+
+
+    def _deserialize(self, params):
+        self.Timestamp = params.get("Timestamp")
+        self.SqlText = params.get("SqlText")
+        self.Database = params.get("Database")
+        self.UserName = params.get("UserName")
+        self.UserHost = params.get("UserHost")
+        self.QueryTime = params.get("QueryTime")
+        self.LockTime = params.get("LockTime")
+        self.RowsExamined = params.get("RowsExamined")
+        self.RowsSent = params.get("RowsSent")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class SlowLogTopSqlItem(AbstractModel):
     """慢日志TopSql
 
     """
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dbbrain
-Version: 3.0.868
+Version: 3.0.870
 Summary: Tencent Cloud Dbbrain SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-dbbrain-3.0.870/tencentcloud_sdk_python_dbbrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/README.rst` & `tencentcloud-sdk-python-dbbrain-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dbbrain-3.0.868/setup.py` & `tencentcloud-sdk-python-dbbrain-3.0.870/setup.py`

 * *Files identical despite different names*

