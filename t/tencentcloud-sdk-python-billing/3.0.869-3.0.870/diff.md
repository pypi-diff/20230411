# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.869.tar", last modified: Mon Apr 10 02:55:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.870.tar", last modified: Tue Apr 11 03:20:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.869.tar` & `tencentcloud-sdk-python-billing-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)   148023 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19523 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)     2904 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud_sdk_python_billing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:55:19.000000 tencentcloud-sdk-python-billing-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)   148244 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19523 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:20:41.000000 tencentcloud-sdk-python-billing-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-billing-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.870/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/v20180709/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,17 @@
 注意：此字段可能返回 null，表示取不到有效值。
         :type ActionType: str
         :param RegionId: 区域ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegionId: str
         :param ProjectId: 项目ID:资源所属项目ID
         :type ProjectId: int
+        :param PriceInfo: 价格属性
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PriceInfo: list of str
         """
         self.BusinessCodeName = None
         self.ProductCodeName = None
         self.PayModeName = None
         self.ProjectName = None
         self.RegionName = None
         self.ZoneName = None
@@ -183,14 +186,15 @@
         self.OperateUin = None
         self.Tags = None
         self.BusinessCode = None
         self.ProductCode = None
         self.ActionType = None
         self.RegionId = None
         self.ProjectId = None
+        self.PriceInfo = None
 
 
     def _deserialize(self, params):
         self.BusinessCodeName = params.get("BusinessCodeName")
         self.ProductCodeName = params.get("ProductCodeName")
         self.PayModeName = params.get("PayModeName")
         self.ProjectName = params.get("ProjectName")
@@ -220,14 +224,15 @@
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.BusinessCode = params.get("BusinessCode")
         self.ProductCode = params.get("ProductCode")
         self.ActionType = params.get("ActionType")
         self.RegionId = params.get("RegionId")
         self.ProjectId = params.get("ProjectId")
+        self.PriceInfo = params.get("PriceInfo")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/v20180709/billing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.869/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.870/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.869/README.rst` & `tencentcloud-sdk-python-billing-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.869/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.870/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.869/setup.py` & `tencentcloud-sdk-python-billing-3.0.870/setup.py`

 * *Files identical despite different names*

