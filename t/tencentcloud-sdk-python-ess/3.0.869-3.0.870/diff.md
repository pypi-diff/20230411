# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.869.tar", last modified: Mon Apr 10 03:05:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.870.tar", last modified: Tue Apr 11 03:38:34 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.869.tar` & `tencentcloud-sdk-python-ess-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    46634 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)   212239 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:05:18.000000 tencentcloud-sdk-python-ess-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    47026 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)   212239 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:38:34.000000 tencentcloud-sdk-python-ess-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.870/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateDocument(self, request):
         """创建签署流程电子文档
-        适用场景：见创建签署流程接口。x0b
+        适用场景：见创建签署流程接口。
         注：该接口需要给对应的流程指定一个模板id，并且填充该模板中需要补充的信息。是“发起流程”接口的前置接口。
 
         :param request: Request instance for CreateDocument.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateDocumentRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateDocumentResponse`
 
         """
@@ -248,14 +248,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateFlowReminds(self, request):
         """指定需要批量催办的签署流程Id，批量催办合同，最多100个; 接口失败后返回错误信息
         注意:
         该接口不可直接调用，请联系客户经理申请使用
+        仅能催办当前状态为“待签署”的签署人，且只能催办一次
+        发起合同时，签署人的NotifyType需设置为sms，否则无法催办
 
         :param request: Request instance for CreateFlowReminds.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowRemindsRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowRemindsResponse`
 
         """
         try:
@@ -415,15 +417,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreatePreparedPersonalEsign(self, request):
-        """本接口（CreatePreparedPersonalEsign）由于创建导入个人印章。
+        """本接口（CreatePreparedPersonalEsign）用于创建导入个人印章。
 
         :param request: Request instance for CreatePreparedPersonalEsign.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreatePreparedPersonalEsignRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreatePreparedPersonalEsignResponse`
 
         """
         try:
@@ -913,15 +915,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def GetTaskResultApi(self, request):
-        """查询转换任务状态
+        """通过发起转换任务接口（CreateConvertTaskApi）返回的任务Id查询转换任务状态，通过本接口确认转换任务是否完成。大文件转换所需的时间可能会比较长。
 
         :param request: Request instance for GetTaskResultApi.
         :type request: :class:`tencentcloud.ess.v20201111.models.GetTaskResultApiRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.GetTaskResultApiResponse`
 
         """
         try:
@@ -1035,15 +1037,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def VerifyPdf(self, request):
-        """验证合同文件
+        """对流程的合同文件进行验证，判断文件是否合法。
 
         :param request: Request instance for VerifyPdf.
         :type request: :class:`tencentcloud.ess.v20201111.models.VerifyPdfRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.VerifyPdfResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.869/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.870/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.869/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.870/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.869/README.rst` & `tencentcloud-sdk-python-ess-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.869/setup.py` & `tencentcloud-sdk-python-ess-3.0.870/setup.py`

 * *Files identical despite different names*

