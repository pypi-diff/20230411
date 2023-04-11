# Comparing `tmp/tencentcloud-sdk-python-cfs-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-cfs-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.869.tar", last modified: Mon Apr 10 02:57:44 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfs-3.0.870.tar", last modified: Tue Apr 11 03:26:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfs-3.0.869.tar` & `tencentcloud-sdk-python-cfs-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud_sdk_python_cfs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)    95341 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33132 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)    13386 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:57:44.000000 tencentcloud-sdk-python-cfs-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud_sdk_python_cfs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud_sdk_python_cfs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud_sdk_python_cfs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud_sdk_python_cfs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)    95368 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33132 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)    13386 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:26:09.000000 tencentcloud-sdk-python-cfs-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.869/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.870/tencentcloud_sdk_python_cfs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-cfs-3.0.870/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfs
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cfs SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/v20190719/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         :type Hour: str
         :param PolicyName: 策略名称
         :type PolicyName: str
         :param DayOfWeek: 快照重复日期，星期一到星期日
         :type DayOfWeek: str
         :param AliveDays: 快照保留时长
         :type AliveDays: int
-        :param DayOfMonth: 快照按月重复，每月1-31号，选择一天，每月这一天打快照。
+        :param DayOfMonth: 快照按月重复，每月1-31号，选择一天，每月将在这一天自动创建快照。
         :type DayOfMonth: str
         :param IntervalDays: 间隔天数
         :type IntervalDays: int
         """
         self.Hour = None
         self.PolicyName = None
         self.DayOfWeek = None
@@ -2430,15 +2430,15 @@
         :type DayOfWeek: str
         :param Hour: 快照定期备份在一天的哪一小时
         :type Hour: str
         :param AliveDays: 快照保留日期
         :type AliveDays: int
         :param IsActivated: 是否激活定期快照功能
         :type IsActivated: int
-        :param DayOfMonth: 定期快照在月的某几天天，该参数与DayOfWeek互斥
+        :param DayOfMonth: 定期快照在每月的第几天创建快照，该参数与DayOfWeek互斥
         :type DayOfMonth: str
         :param IntervalDays: 间隔天数定期执行快照，该参数与DayOfWeek,DayOfMonth 互斥
         :type IntervalDays: int
         """
         self.AutoSnapshotPolicyId = None
         self.PolicyName = None
         self.DayOfWeek = None
```

### Comparing `tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfs-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfs-3.0.869/README.rst` & `tencentcloud-sdk-python-cfs-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfs-3.0.869/setup.py` & `tencentcloud-sdk-python-cfs-3.0.870/setup.py`

 * *Files identical despite different names*

