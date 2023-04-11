# Comparing `tmp/tencentcloud-sdk-python-tiw-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-tiw-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.869.tar", last modified: Mon Apr 10 03:16:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tiw-3.0.870.tar", last modified: Tue Apr 11 03:56:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tiw-3.0.869.tar` & `tencentcloud-sdk-python-tiw-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/v20190919/
--rw-r--r--   0 root         (0) root         (0)   166407 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/v20190919/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/v20190919/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5672 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/v20190919/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    52622 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/v20190919/tiw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud_sdk_python_tiw.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:16:32.000000 tencentcloud-sdk-python-tiw-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/v20190919/
+-rw-r--r--   0 root         (0) root         (0)   185677 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/v20190919/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/v20190919/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6089 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/v20190919/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60210 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/v20190919/tiw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud_sdk_python_tiw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud_sdk_python_tiw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud_sdk_python_tiw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/tencentcloud_sdk_python_tiw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:56:18.000000 tencentcloud-sdk-python-tiw-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.870/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/v20190919/models.py` & `tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/v20190919/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -305,14 +305,72 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class CreatePPTCheckTaskRequest(AbstractModel):
+    """CreatePPTCheckTask请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 客户的SdkAppId
+        :type SdkAppId: int
+        :param Url: 经过URL编码后的PPT文件地址。URL 编码会将字符转换为可通过因特网传输的格式，比如文档地址为http://example.com/测试.pptx，经过URL编码之后为http://example.com/%E6%B5%8B%E8%AF%95.pptx。为了提高URL解析的成功率，请对URL进行编码。
+        :type Url: str
+        :param AutoHandleUnsupportedElement: 是否对不支持元素开启自动处理的功能。默认不开启。
+
+在开启自动处理的情况下，会自动进行如下处理：
+1. 墨迹：移除不支持的墨迹（比如使用WPS画的）
+2. 自动翻页：移除PPT上所有的自动翻页设置，并设置为单击鼠标翻页
+3. 已损坏音视频：移除PPT上对损坏音视频的引用
+        :type AutoHandleUnsupportedElement: bool
+        """
+        self.SdkAppId = None
+        self.Url = None
+        self.AutoHandleUnsupportedElement = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        self.Url = params.get("Url")
+        self.AutoHandleUnsupportedElement = params.get("AutoHandleUnsupportedElement")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreatePPTCheckTaskResponse(AbstractModel):
+    """CreatePPTCheckTask返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 检测任务的唯一标识Id，用于查询该任务的进度以及检测结果
+        :type TaskId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateSnapshotTaskRequest(AbstractModel):
     """CreateSnapshotTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1170,14 +1228,139 @@
             for item in params.get("Interrupts"):
                 obj = Interrupt()
                 obj._deserialize(item)
                 self.Interrupts.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribePPTCheckCallbackRequest(AbstractModel):
+    """DescribePPTCheckCallback请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 应用的SdkAppId
+        :type SdkAppId: int
+        """
+        self.SdkAppId = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribePPTCheckCallbackResponse(AbstractModel):
+    """DescribePPTCheckCallback返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Callback: 回调地址
+        :type Callback: str
+        :param CallbackKey: 回调鉴权密钥
+        :type CallbackKey: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Callback = None
+        self.CallbackKey = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Callback = params.get("Callback")
+        self.CallbackKey = params.get("CallbackKey")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribePPTCheckRequest(AbstractModel):
+    """DescribePPTCheck请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 客户的SdkAppId
+        :type SdkAppId: int
+        :param TaskId: 任务的唯一标识Id
+        :type TaskId: str
+        """
+        self.SdkAppId = None
+        self.TaskId = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        self.TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribePPTCheckResponse(AbstractModel):
+    """DescribePPTCheck返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务的唯一标识Id
+        :type TaskId: str
+        :param IsOK: PPT文件是否正常
+        :type IsOK: bool
+        :param ResultUrl: 修复后的PPT URL，只有创建任务时参数AutoHandleUnsupportedElement=true，才返回此参数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResultUrl: str
+        :param Slides: 错误PPT页面列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Slides: list of PPTErrSlide
+        :param Status: 任务的当前状态 - QUEUED: 正在排队等待 - PROCESSING: 执行中 - FINISHED: 执行完成	
+        :type Status: str
+        :param Progress: 当前进度,取值范围为0~100
+        :type Progress: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskId = None
+        self.IsOK = None
+        self.ResultUrl = None
+        self.Slides = None
+        self.Status = None
+        self.Progress = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        self.IsOK = params.get("IsOK")
+        self.ResultUrl = params.get("ResultUrl")
+        if params.get("Slides") is not None:
+            self.Slides = []
+            for item in params.get("Slides"):
+                obj = PPTErrSlide()
+                obj._deserialize(item)
+                self.Slides.append(obj)
+        self.Status = params.get("Status")
+        self.Progress = params.get("Progress")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribePostpaidUsageRequest(AbstractModel):
     """DescribePostpaidUsage请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1394,14 +1577,86 @@
             for item in params.get("RoomList"):
                 obj = RoomListItem()
                 obj._deserialize(item)
                 self.RoomList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeRunningTasksRequest(AbstractModel):
+    """DescribeRunningTasks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppID: 应用的SdkAppID
+        :type SdkAppID: int
+        :param TaskType: 指定需要获取的任务类型。
+有效取值如下：
+- TranscodeH5: 动态转码任务，文档转HTML5页面
+- TranscodeJPG: 静态转码任务，文档转图片
+- WhiteboardPush: 白板推流任务
+- OnlineRecord: 实时录制任务
+        :type TaskType: str
+        :param Offset: 分页获取时的任务偏移量，默认为0。
+        :type Offset: int
+        :param Limit: 每次获取任务列表时最大获取任务数，默认值为100。
+有效取值范围：[1, 500]
+        :type Limit: int
+        """
+        self.SdkAppID = None
+        self.TaskType = None
+        self.Offset = None
+        self.Limit = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppID = params.get("SdkAppID")
+        self.TaskType = params.get("TaskType")
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
+class DescribeRunningTasksResponse(AbstractModel):
+    """DescribeRunningTasks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Total: 当前正在执行中的任务总数
+        :type Total: int
+        :param Tasks: 任务信息列表
+        :type Tasks: list of RunningTaskItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Total = None
+        self.Tasks = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Total = params.get("Total")
+        if params.get("Tasks") is not None:
+            self.Tasks = []
+            for item in params.get("Tasks"):
+                obj = RunningTaskItem()
+                obj._deserialize(item)
+                self.Tasks.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeSnapshotTaskRequest(AbstractModel):
     """DescribeSnapshotTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2130,14 +2385,63 @@
             for item in params.get("VideoInfoList"):
                 obj = VideoInfo()
                 obj._deserialize(item)
                 self.VideoInfoList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeWarningCallbackRequest(AbstractModel):
+    """DescribeWarningCallback请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 应用的SdkAppId
+        :type SdkAppId: int
+        """
+        self.SdkAppId = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeWarningCallbackResponse(AbstractModel):
+    """DescribeWarningCallback返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Callback: 告警事件回调地址，如果未设置回调地址，该字段为空字符串
+        :type Callback: str
+        :param CallbackKey: 告警回调鉴权密钥
+        :type CallbackKey: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Callback = None
+        self.CallbackKey = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Callback = params.get("Callback")
+        self.CallbackKey = params.get("CallbackKey")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeWhiteboardApplicationConfigRequest(AbstractModel):
     """DescribeWhiteboardApplicationConfig请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2810,14 +3114,84 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PPTErr(AbstractModel):
+    """PPT错误元素
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: 元素名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param Type: 0: 不支持的墨迹类型，1: 不支持自动翻页，2: 存在已损坏音视频，3: 存在不可访问资源，4: 只读文件
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: int
+        :param Detail: 错误详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Detail: str
+        """
+        self.Name = None
+        self.Type = None
+        self.Detail = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.Type = params.get("Type")
+        self.Detail = params.get("Detail")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PPTErrSlide(AbstractModel):
+    """PPT错误页面列表
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Page: 异常元素存在的页面，由页面类型+页码组成，页码类型包括：幻灯片、幻灯片母版、幻灯片布局等
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Page: str
+        :param Errs: 错误元素列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Errs: list of PPTErr
+        """
+        self.Page = None
+        self.Errs = None
+
+
+    def _deserialize(self, params):
+        self.Page = params.get("Page")
+        if params.get("Errs") is not None:
+            self.Errs = []
+            for item in params.get("Errs"):
+                obj = PPTErr()
+                obj._deserialize(item)
+                self.Errs.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class PauseOnlineRecordRequest(AbstractModel):
     """PauseOnlineRecord请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3168,14 +3542,83 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RunningTaskItem(AbstractModel):
+    """正在运行的任务列表项
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppID: 应用SdkAppID
+        :type SdkAppID: int
+        :param TaskID: 任务ID
+        :type TaskID: str
+        :param TaskType: 任务类型
+- TranscodeH5: 动态转码任务，文档转HTML5页面
+- TranscodeJPG: 静态转码任务，文档转图片
+- WhiteboardPush: 白板推流任务
+- OnlineRecord: 实时录制任务
+        :type TaskType: str
+        :param CreateTime: 任务创建时间
+        :type CreateTime: str
+        :param CancelTime: 任务取消时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CancelTime: str
+        :param Status: 任务状态
+- QUEUED: 任务正在排队等待执行中
+- PROCESSING: 任务正在执行中 
+- FINISHED: 任务已完成
+        :type Status: str
+        :param Progress: 任务当前进度
+        :type Progress: int
+        :param FileURL: 转码任务中转码文件的原始URL
+此参数只有任务类型为TranscodeH5、TranscodeJPG类型时才会有有效值。其他任务类型为空字符串。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileURL: str
+        :param RoomID: 房间号
+
+当任务类型为TranscodeH5、TranscodeJPG时，房间号为0。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RoomID: int
+        """
+        self.SdkAppID = None
+        self.TaskID = None
+        self.TaskType = None
+        self.CreateTime = None
+        self.CancelTime = None
+        self.Status = None
+        self.Progress = None
+        self.FileURL = None
+        self.RoomID = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppID = params.get("SdkAppID")
+        self.TaskID = params.get("TaskID")
+        self.TaskType = params.get("TaskType")
+        self.CreateTime = params.get("CreateTime")
+        self.CancelTime = params.get("CancelTime")
+        self.Status = params.get("Status")
+        self.Progress = params.get("Progress")
+        self.FileURL = params.get("FileURL")
+        self.RoomID = params.get("RoomID")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SetOfflineRecordCallbackRequest(AbstractModel):
     """SetOfflineRecordCallback请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3303,14 +3746,104 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class SetPPTCheckCallbackKeyRequest(AbstractModel):
+    """SetPPTCheckCallbackKey请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 应用的SdkAppId
+        :type SdkAppId: int
+        :param CallbackKey: 设置回调鉴权密钥，最长64字符，如果传入空字符串，那么删除现有的鉴权回调密钥，回调鉴权方式请参考文档：https://cloud.tencent.com/document/product/1137/40257	
+        :type CallbackKey: str
+        """
+        self.SdkAppId = None
+        self.CallbackKey = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        self.CallbackKey = params.get("CallbackKey")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SetPPTCheckCallbackKeyResponse(AbstractModel):
+    """SetPPTCheckCallbackKey返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class SetPPTCheckCallbackRequest(AbstractModel):
+    """SetPPTCheckCallback请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 客户的SdkAppId	
+        :type SdkAppId: int
+        :param Callback: 进度回调地址，如果传空字符串会删除原来的回调地址配置，回调地址仅支持http或https协议，即回调地址以http://或https://开头。 回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260	
+        :type Callback: str
+        """
+        self.SdkAppId = None
+        self.Callback = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        self.Callback = params.get("Callback")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SetPPTCheckCallbackResponse(AbstractModel):
+    """SetPPTCheckCallback返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class SetTranscodeCallbackKeyRequest(AbstractModel):
     """SetTranscodeCallbackKey请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3476,14 +4009,64 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class SetWarningCallbackRequest(AbstractModel):
+    """SetWarningCallback请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SdkAppId: 客户的SdkAppId
+        :type SdkAppId: int
+        :param Callback: 告警回调地址，如果传空字符串会删除原来的回调地址配置，回调地址仅支持http或https协议，即回调地址以http://或https://开头。
+回调数据格式请参考文档：
+        :type Callback: str
+        :param CallbackKey: 设置告警回调鉴权密钥，最长64字符，如果传入空字符串，那么删除现有的鉴权回调密钥，回调鉴权方式请参考文档：https://cloud.tencent.com/document/product/1137/40257
+        :type CallbackKey: str
+        """
+        self.SdkAppId = None
+        self.Callback = None
+        self.CallbackKey = None
+
+
+    def _deserialize(self, params):
+        self.SdkAppId = params.get("SdkAppId")
+        self.Callback = params.get("Callback")
+        self.CallbackKey = params.get("CallbackKey")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class SetWarningCallbackResponse(AbstractModel):
+    """SetWarningCallback返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/v20190919/errorcodes.py` & `tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/v20190919/errorcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
 # 转码后上传结果失败，请稍候重试。
 FAILEDOPERATION_FILEUPLOADFAIL = 'FailedOperation.FileUploadFail'
 
 # 获取临时密钥失败。
 FAILEDOPERATION_GETCREDENTIALFAIL = 'FailedOperation.GetCredentialFail'
 
+# 转码预处理失败，具体请参考错误描述或联系客服人员。
+FAILEDOPERATION_PREPROCESS = 'FailedOperation.Preprocess'
+
+# 预处理服务出现内部错误，请稍候重试或联系客户人员。
+FAILEDOPERATION_PREPROCESSSERVERERROR = 'FailedOperation.PreprocessServerError'
+
 # 录制失败，具体请参考错误描述。
 FAILEDOPERATION_RECORD = 'FailedOperation.Record'
 
 # 转码失败，具体请参考错误描述或联系客服人员。
 FAILEDOPERATION_TRANSCODE = 'FailedOperation.Transcode'
 
 # 转码服务出现内部错误，请稍候重试或联系客户人员。
@@ -76,14 +82,17 @@
 
 # 额外指定的特殊功能不存在。
 INVALIDPARAMETER_INVALIDEXTRA = 'InvalidParameter.InvalidExtra'
 
 # 设置应用配置任务类型不支持。
 INVALIDPARAMETER_INVALIDTASKTYPE = 'InvalidParameter.InvalidTaskType'
 
+# 转码预处理参数格式不正确。
+INVALIDPARAMETER_PREPROCESSPARAMETER = 'InvalidParameter.PreprocessParameter'
+
 # 实时录制参数格式不正确。
 INVALIDPARAMETER_RECORDPARAMETER = 'InvalidParameter.RecordParameter'
 
 # SdkAppId不存在或格式错误。
 INVALIDPARAMETER_SDKAPPIDNOTFOUND = 'InvalidParameter.SdkAppIdNotFound'
 
 # 需要查询的任务不存在。
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.869/tencentcloud/tiw/v20190919/tiw_client.py` & `tencentcloud-sdk-python-tiw-3.0.870/tencentcloud/tiw/v20190919/tiw_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreatePPTCheckTask(self, request):
+        """检测PPT文件，识别PPT中包含的动态转码任务（Transcode）不支持的元素
+
+        :param request: Request instance for CreatePPTCheckTask.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.CreatePPTCheckTaskRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.CreatePPTCheckTaskResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreatePPTCheckTask", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreatePPTCheckTaskResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateSnapshotTask(self, request):
         """创建白板板书生成任务, 在任务结束后，如果提供了回调地址，将通过回调地址通知板书生成结果
 
         :param request: Request instance for CreateSnapshotTask.
         :type request: :class:`tencentcloud.tiw.v20190919.models.CreateSnapshotTaskRequest`
         :rtype: :class:`tencentcloud.tiw.v20190919.models.CreateSnapshotTaskResponse`
 
@@ -367,14 +390,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribePPTCheck(self, request):
+        """查询PPT检测任务的执行进度或结果
+
+        :param request: Request instance for DescribePPTCheck.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.DescribePPTCheckRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribePPTCheckResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribePPTCheck", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribePPTCheckResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribePPTCheckCallback(self, request):
+        """查询PPT检测任务回调地址
+
+        :param request: Request instance for DescribePPTCheckCallback.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.DescribePPTCheckCallbackRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribePPTCheckCallbackResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribePPTCheckCallback", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribePPTCheckCallbackResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribePostpaidUsage(self, request):
         """查询用户后付费用量
 
         :param request: Request instance for DescribePostpaidUsage.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribePostpaidUsageRequest`
         :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribePostpaidUsageResponse`
 
@@ -459,14 +528,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeRunningTasks(self, request):
+        """根据指定的任务类型，获取当前正在执行中的任务列表。只能查询最近3天内创建的任务。
+
+        :param request: Request instance for DescribeRunningTasks.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeRunningTasksRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribeRunningTasksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeRunningTasks", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeRunningTasksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeSnapshotTask(self, request):
         """获取指定白板板书生成任务信息
 
         :param request: Request instance for DescribeSnapshotTask.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeSnapshotTaskRequest`
         :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribeSnapshotTaskResponse`
 
@@ -739,14 +831,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeWarningCallback(self, request):
+        """查询告警回调地址。此功能需要申请白名单使用。
+
+        :param request: Request instance for DescribeWarningCallback.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeWarningCallbackRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribeWarningCallbackResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeWarningCallback", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeWarningCallbackResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeWhiteboardApplicationConfig(self, request):
         """查询白板应用任务相关的配置，包括存储桶、回调等
 
         :param request: Request instance for DescribeWhiteboardApplicationConfig.
         :type request: :class:`tencentcloud.tiw.v20190919.models.DescribeWhiteboardApplicationConfigRequest`
         :rtype: :class:`tencentcloud.tiw.v20190919.models.DescribeWhiteboardApplicationConfigResponse`
 
@@ -1061,14 +1176,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def SetPPTCheckCallback(self, request):
+        """设置PPT检测任务回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260
+
+        :param request: Request instance for SetPPTCheckCallback.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.SetPPTCheckCallbackRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.SetPPTCheckCallbackResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SetPPTCheckCallback", params, headers=headers)
+            response = json.loads(body)
+            model = models.SetPPTCheckCallbackResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SetPPTCheckCallbackKey(self, request):
+        """设置PPT检测任务回调密钥，回调鉴权方式请参考文档：https://cloud.tencent.com/document/product/1137/40257
+
+        :param request: Request instance for SetPPTCheckCallbackKey.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.SetPPTCheckCallbackKeyRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.SetPPTCheckCallbackKeyResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SetPPTCheckCallbackKey", params, headers=headers)
+            response = json.loads(body)
+            model = models.SetPPTCheckCallbackKeyResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def SetTranscodeCallback(self, request):
         """设置文档转码回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40260
 
         :param request: Request instance for SetTranscodeCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetTranscodeCallbackRequest`
         :rtype: :class:`tencentcloud.tiw.v20190919.models.SetTranscodeCallbackResponse`
 
@@ -1151,14 +1312,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def SetWarningCallback(self, request):
+        """设置告警回调地址。此功能需要申请白名单使用。
+
+        :param request: Request instance for SetWarningCallback.
+        :type request: :class:`tencentcloud.tiw.v20190919.models.SetWarningCallbackRequest`
+        :rtype: :class:`tencentcloud.tiw.v20190919.models.SetWarningCallbackResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("SetWarningCallback", params, headers=headers)
+            response = json.loads(body)
+            model = models.SetWarningCallbackResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def SetWhiteboardPushCallback(self, request):
         """设置白板推流回调地址，回调数据格式请参考文档：https://cloud.tencent.com/document/product/1137/40257
 
         :param request: Request instance for SetWhiteboardPushCallback.
         :type request: :class:`tencentcloud.tiw.v20190919.models.SetWhiteboardPushCallbackRequest`
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.869/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tiw-3.0.870/tencentcloud_sdk_python_tiw.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tiw
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Tiw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tiw-3.0.869/README.rst` & `tencentcloud-sdk-python-tiw-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tiw-3.0.869/setup.py` & `tencentcloud-sdk-python-tiw-3.0.870/setup.py`

 * *Files identical despite different names*

