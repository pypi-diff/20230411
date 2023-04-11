# Comparing `tmp/tencentcloud-sdk-python-iotexplorer-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-iotexplorer-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.869.tar", last modified: Mon Apr 10 03:07:46 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotexplorer-3.0.870.tar", last modified: Tue Apr 11 03:41:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869.tar` & `tencentcloud-sdk-python-iotexplorer-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1699 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:07:45.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/v20190423/
--rw-r--r--   0 root         (0) root         (0)    82835 2023-04-10 03:07:45.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
--rw-r--r--   0 root         (0) root         (0)   224109 2023-04-10 03:07:45.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/v20190423/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:07:45.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/v20190423/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20131 2023-04-10 03:07:45.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/v20190423/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:07:45.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      761 2023-04-10 03:07:45.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud_sdk_python_iotexplorer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1699 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      525 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1022 2023-04-10 03:07:45.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:07:46.000000 tencentcloud-sdk-python-iotexplorer-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/v20190423/
+-rw-r--r--   0 root         (0) root         (0)    82835 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
+-rw-r--r--   0 root         (0) root         (0)   224109 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/v20190423/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/v20190423/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20392 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/v20190423/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      761 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud_sdk_python_iotexplorer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1699 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud_sdk_python_iotexplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud_sdk_python_iotexplorer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      525 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:41:13.000000 tencentcloud-sdk-python-iotexplorer-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.870/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py` & `tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/v20190423/models.py` & `tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/v20190423/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/iotexplorer/v20190423/errorcodes.py` & `tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/iotexplorer/v20190423/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,14 +427,17 @@
 
 # 实例ACL错误。
 UNAUTHORIZEDOPERATION_NOPERMISSIONTOSTUDIOINSTANCE = 'UnauthorizedOperation.NoPermissionToStudioInstance'
 
 # 产品ACL错误。
 UNAUTHORIZEDOPERATION_NOPERMISSIONTOSTUDIOPRODUCT = 'UnauthorizedOperation.NoPermissionToStudioProduct'
 
+# 您的帐号未实名认证，请登录腾讯云进行实名认证
+UNAUTHORIZEDOPERATION_NOVERIFIED = 'UnauthorizedOperation.NoVerified'
+
 # 没有权限。
 UNAUTHORIZEDOPERATION_PERMISSIONDENIED = 'UnauthorizedOperation.PermissionDenied'
 
 # 产品不支持密钥认证。
 UNAUTHORIZEDOPERATION_PRODUCTNOTSUPPORTPSK = 'UnauthorizedOperation.ProductNotSupportPSK'
 
 # License数量不足。
@@ -522,7 +525,10 @@
 UNSUPPORTEDOPERATION_VPNDUPKEYEXIST = 'UnsupportedOperation.VPNDupKeyExist'
 
 # Video账户未创建，请检查后重新操作。
 UNSUPPORTEDOPERATION_VIDEOACCOUNTNOTEXIST = 'UnsupportedOperation.VideoAccountNotExist'
 
 # Video平台license数量不足。
 UNSUPPORTEDOPERATION_VIDEOINSUFFICIENTLICENSES = 'UnsupportedOperation.VideoInsufficientLicenses'
+
+# Video平台产品不存在。
+UNSUPPORTEDOPERATION_VIDEOPRODUCTNOTEXIST = 'UnsupportedOperation.VideoProductNotExist'
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/README.rst` & `tencentcloud-sdk-python-iotexplorer-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud_sdk_python_iotexplorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotexplorer
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Iotexplorer SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotexplorer-3.0.870/tencentcloud_sdk_python_iotexplorer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotexplorer-3.0.869/setup.py` & `tencentcloud-sdk-python-iotexplorer-3.0.870/setup.py`

 * *Files identical despite different names*

