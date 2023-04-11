# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.869.tar", last modified: Mon Apr 10 02:57:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.870.tar", last modified: Tue Apr 11 03:25:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.869.tar` & `tencentcloud-sdk-python-cdb-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   485265 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18041 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   141262 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:57:05.000000 tencentcloud-sdk-python-cdb-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:57:06.000000 tencentcloud-sdk-python-cdb-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   485639 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   141262 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:25:30.000000 tencentcloud-sdk-python-cdb-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.870/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13058,14 +13058,16 @@
         :type FastUpgrade: int
         :param MaxDelayTime: 延迟阈值。取值范围1~10，默认值为10。
         :type MaxDelayTime: int
         :param CrossCluster: 是否跨区迁移。0-普通迁移，1-跨区迁移，默认值为0。该值为1时支持变更实例主节点可用区。
         :type CrossCluster: int
         :param ZoneId: 主节点可用区，该值仅在跨区迁移时生效。仅支持同地域下的可用区进行迁移。
         :type ZoneId: str
+        :param RoTransType: 针对跨集群搬迁场景，选择同可用区RO的处理逻辑。together-同可用区RO跟随主实例迁移至目标可用区（默认选项），severally-同可用区RO保持原部署模式、不迁移至目标可用区。
+        :type RoTransType: str
         """
         self.InstanceId = None
         self.Memory = None
         self.Volume = None
         self.ProtectMode = None
         self.DeployMode = None
         self.SlaveZone = None
@@ -13075,14 +13077,15 @@
         self.InstanceRole = None
         self.DeviceType = None
         self.Cpu = None
         self.FastUpgrade = None
         self.MaxDelayTime = None
         self.CrossCluster = None
         self.ZoneId = None
+        self.RoTransType = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.Memory = params.get("Memory")
         self.Volume = params.get("Volume")
         self.ProtectMode = params.get("ProtectMode")
@@ -13094,14 +13097,15 @@
         self.InstanceRole = params.get("InstanceRole")
         self.DeviceType = params.get("DeviceType")
         self.Cpu = params.get("Cpu")
         self.FastUpgrade = params.get("FastUpgrade")
         self.MaxDelayTime = params.get("MaxDelayTime")
         self.CrossCluster = params.get("CrossCluster")
         self.ZoneId = params.get("ZoneId")
+        self.RoTransType = params.get("RoTransType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.870/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.869/README.rst` & `tencentcloud-sdk-python-cdb-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.869/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.870/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.869/setup.py` & `tencentcloud-sdk-python-cdb-3.0.870/setup.py`

 * *Files identical despite different names*

