# Comparing `tmp/tencentcloud-sdk-python-cvm-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-cvm-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.869.tar", last modified: Mon Apr 10 02:59:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cvm-3.0.870.tar", last modified: Tue Apr 11 03:28:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cvm-3.0.869.tar` & `tencentcloud-sdk-python-cvm-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)   119282 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/v20170312/cvm_client.py
--rw-r--r--   0 root         (0) root         (0)   429343 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42551 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud_sdk_python_cvm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:59:37.000000 tencentcloud-sdk-python-cvm-3.0.869/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   119282 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/v20170312/cvm_client.py
+-rw-r--r--   0 root         (0) root         (0)   429546 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42551 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud_sdk_python_cvm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud_sdk_python_cvm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud_sdk_python_cvm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:28:11.000000 tencentcloud-sdk-python-cvm-3.0.870/tencentcloud_sdk_python_cvm.egg-info/SOURCES.txt
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.870/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4153,15 +4153,15 @@
 NORMAL-正常
 CREATEFAILED-创建失败
 USING-使用中
 SYNCING-同步中
 IMPORTING-导入中
 IMPORTFAILED-导入失败
         :type ImageState: str
-        :param Platform: 镜像来源平台
+        :param Platform: 镜像来源平台，包括如TencentOS、 CentOS、 Windows、 Ubuntu、 Debian、Fedora等。
         :type Platform: str
         :param ImageCreator: 镜像创建者
         :type ImageCreator: str
         :param ImageSource: 镜像来源
         :type ImageSource: str
         :param SyncPercent: 同步百分比
 注意：此字段可能返回 null，表示取不到有效值。
@@ -9259,15 +9259,15 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Tag(AbstractModel):
-    """标签键值对
+    """标签键值对，可以通过调用 [DescribeTags](https://cloud.tencent.com/document/api/651/35316) 返回值中的 Tags 字段来获取。
 
     """
 
     def __init__(self):
         r"""
         :param Key: 标签键
         :type Key: str
```

### Comparing `tencentcloud-sdk-python-cvm-3.0.869/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-cvm-3.0.870/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.869/README.rst` & `tencentcloud-sdk-python-cvm-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.869/setup.py` & `tencentcloud-sdk-python-cvm-3.0.870/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cvm-3.0.869/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cvm-3.0.870/tencentcloud_sdk_python_cvm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cvm
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cvm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

