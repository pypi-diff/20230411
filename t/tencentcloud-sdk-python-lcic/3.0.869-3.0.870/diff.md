# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.869.tar", last modified: Mon Apr 10 03:08:34 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.870.tar", last modified: Tue Apr 11 03:42:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.869.tar` & `tencentcloud-sdk-python-lcic-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)   126627 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43349 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)     4332 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:08:34.000000 tencentcloud-sdk-python-lcic-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)   127315 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43349 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)     4332 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:42:05.000000 tencentcloud-sdk-python-lcic-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.870/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -867,59 +867,73 @@
         :type SubType: str
         :param TeacherId: 老师ID。通过[注册用户]接口获取的UserId。指定后该用户在房间内拥有老师权限。
         :type TeacherId: str
         :param AutoMic: 进入课堂时是否自动连麦。可以有以下取值：
 0 不自动连麦（需要手动申请上麦，默认值）
 1 自动连麦
         :type AutoMic: int
+        :param TurnOffMic: 释放音视频权限后是否自动取消连麦。可以有以下取值：
+0 自动取消连麦（默认值）
+1 保持连麦状态
+        :type TurnOffMic: int
         :param AudioQuality: 高音质模式。可以有以下取值：
 0 不开启高音质（默认值）
 1 开启高音质
         :type AudioQuality: int
         :param DisableRecord: 上课后是否禁止自动录制。可以有以下取值：
 0 不禁止录制（自动开启录制，默认值）
 1 禁止录制
 注：如果该配置取值为0，录制将从上课后开始，课堂结束后停止。
         :type DisableRecord: int
         :param Assistants: 助教Id列表。通过[注册用户]接口获取的UserId。指定后该用户在房间内拥有助教权限。
         :type Assistants: list of str
+        :param RTCAudienceNumber: rtc人数。
+        :type RTCAudienceNumber: int
+        :param AudienceType: 观看类型。0未知，1互动，2cdn或直播。 目前仅支持互动类型
+        :type AudienceType: int
         :param RecordLayout: 录制布局。录制模板枚举值参考：https://cloud.tencent.com/document/product/1639/89744
         :type RecordLayout: int
         :param GroupId: 房间绑定的群组ID,非空时限制组成员进入
         :type GroupId: str
         """
         self.Name = None
         self.StartTime = None
         self.EndTime = None
         self.SdkAppId = None
         self.Resolution = None
         self.MaxMicNumber = None
         self.SubType = None
         self.TeacherId = None
         self.AutoMic = None
+        self.TurnOffMic = None
         self.AudioQuality = None
         self.DisableRecord = None
         self.Assistants = None
+        self.RTCAudienceNumber = None
+        self.AudienceType = None
         self.RecordLayout = None
         self.GroupId = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.SdkAppId = params.get("SdkAppId")
         self.Resolution = params.get("Resolution")
         self.MaxMicNumber = params.get("MaxMicNumber")
         self.SubType = params.get("SubType")
         self.TeacherId = params.get("TeacherId")
         self.AutoMic = params.get("AutoMic")
+        self.TurnOffMic = params.get("TurnOffMic")
         self.AudioQuality = params.get("AudioQuality")
         self.DisableRecord = params.get("DisableRecord")
         self.Assistants = params.get("Assistants")
+        self.RTCAudienceNumber = params.get("RTCAudienceNumber")
+        self.AudienceType = params.get("AudienceType")
         self.RecordLayout = params.get("RecordLayout")
         self.GroupId = params.get("GroupId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.869/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.870/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.869/README.rst` & `tencentcloud-sdk-python-lcic-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.869/setup.py` & `tencentcloud-sdk-python-lcic-3.0.870/setup.py`

 * *Files identical despite different names*

