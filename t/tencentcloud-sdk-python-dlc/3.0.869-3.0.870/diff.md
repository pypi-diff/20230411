# Comparing `tmp/tencentcloud-sdk-python-dlc-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-dlc-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.869.tar", last modified: Mon Apr 10 03:03:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dlc-3.0.870.tar", last modified: Tue Apr 11 03:33:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dlc-3.0.869.tar` & `tencentcloud-sdk-python-dlc-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud_sdk_python_dlc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)   320416 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78371 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/v20210125/dlc_client.py
--rw-r--r--   0 root         (0) root         (0)    11538 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:03:43.000000 tencentcloud-sdk-python-dlc-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud_sdk_python_dlc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud_sdk_python_dlc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud_sdk_python_dlc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud_sdk_python_dlc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:33:55.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:33:55.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)   320808 2023-04-11 03:33:55.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:33:55.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78371 2023-04-11 03:33:55.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/v20210125/dlc_client.py
+-rw-r--r--   0 root         (0) root         (0)    11538 2023-04-11 03:33:55.000000 tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:33:55.000000 tencentcloud-sdk-python-dlc-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:33:55.000000 tencentcloud-sdk-python-dlc-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:33:56.000000 tencentcloud-sdk-python-dlc-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.869/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.870/tencentcloud_sdk_python_dlc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-dlc-3.0.870/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dlc
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Dlc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/v20210125/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1159,14 +1159,18 @@
         :type ResourceType: str
         :param DataEngineConfigPairs: 集群高级配置
         :type DataEngineConfigPairs: list of DataEngineConfigPair
         :param ImageVersionName: 集群镜像版本名字。如SuperSQL-P 1.1;SuperSQL-S 3.2等,不传，默认创建最新镜像版本的集群
         :type ImageVersionName: str
         :param MainClusterName: 主集群名称
         :type MainClusterName: str
+        :param ElasticSwitch: spark jar 包年包月集群是否开启弹性
+        :type ElasticSwitch: bool
+        :param ElasticLimit: spark jar 包年包月集群弹性上限
+        :type ElasticLimit: int
         """
         self.EngineType = None
         self.DataEngineName = None
         self.ClusterType = None
         self.Mode = None
         self.AutoResume = None
         self.MinClusters = None
@@ -1187,14 +1191,16 @@
         self.MaxConcurrency = None
         self.TolerableQueueTime = None
         self.AutoSuspendTime = None
         self.ResourceType = None
         self.DataEngineConfigPairs = None
         self.ImageVersionName = None
         self.MainClusterName = None
+        self.ElasticSwitch = None
+        self.ElasticLimit = None
 
 
     def _deserialize(self, params):
         self.EngineType = params.get("EngineType")
         self.DataEngineName = params.get("DataEngineName")
         self.ClusterType = params.get("ClusterType")
         self.Mode = params.get("Mode")
@@ -1229,14 +1235,16 @@
             self.DataEngineConfigPairs = []
             for item in params.get("DataEngineConfigPairs"):
                 obj = DataEngineConfigPair()
                 obj._deserialize(item)
                 self.DataEngineConfigPairs.append(obj)
         self.ImageVersionName = params.get("ImageVersionName")
         self.MainClusterName = params.get("MainClusterName")
+        self.ElasticSwitch = params.get("ElasticSwitch")
+        self.ElasticLimit = params.get("ElasticLimit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.869/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-dlc-3.0.870/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.869/README.rst` & `tencentcloud-sdk-python-dlc-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dlc-3.0.869/setup.py` & `tencentcloud-sdk-python-dlc-3.0.870/setup.py`

 * *Files identical despite different names*

