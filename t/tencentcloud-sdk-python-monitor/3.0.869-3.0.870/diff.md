# Comparing `tmp/tencentcloud-sdk-python-monitor-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-monitor-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.869.tar", last modified: Mon Apr 10 03:09:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.870.tar", last modified: Tue Apr 11 03:43:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-monitor-3.0.869.tar` & `tencentcloud-sdk-python-monitor-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)   551746 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143620 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)    10246 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-10 03:09:48.000000 tencentcloud-sdk-python-monitor-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:09:49.000000 tencentcloud-sdk-python-monitor-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)   551751 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143620 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)    10246 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud_sdk_python_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:43:17.000000 tencentcloud-sdk-python-monitor-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.870/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/v20180724/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -12345,15 +12345,15 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ProductSimple(AbstractModel):
-    """云监控支持的产品简要信息
+    """云产品监控支持的产品简要信息
 
     """
 
     def __init__(self):
         r"""
         :param Namespace: 命名空间
         :type Namespace: str
@@ -12695,15 +12695,15 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class PrometheusClusterAgentBasic(AbstractModel):
-    """与云监控融合托管prometheus实例，关联集群基础信息
+    """与腾讯云可观测平台融合托管 Prometheus 实例，关联集群基础信息
 
     """
 
     def __init__(self):
         r"""
         :param Region: 集群ID
         :type Region: str
@@ -14670,15 +14670,15 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class URLNotice(AbstractModel):
-    """云监控告警通知模板 - 回调通知详情
+    """告警通知模板 - 回调通知详情
 
     """
 
     def __init__(self):
         r"""
         :param URL: 回调 url（限长256字符）
 注意：此字段可能返回 null，表示取不到有效值。
@@ -15899,15 +15899,15 @@
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
 class UserNotice(AbstractModel):
-    """云监控告警通知模板 - 用户通知详情
+    """告警通知模板 - 用户通知详情
 
     """
 
     def __init__(self):
         r"""
         :param ReceiverType: 接收者类型 USER=用户 GROUP=用户组
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-monitor-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-monitor-3.0.869/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.870/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.869/README.rst` & `tencentcloud-sdk-python-monitor-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.869/setup.py` & `tencentcloud-sdk-python-monitor-3.0.870/setup.py`

 * *Files identical despite different names*

