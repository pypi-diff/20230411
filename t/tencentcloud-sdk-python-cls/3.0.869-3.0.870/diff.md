# Comparing `tmp/tencentcloud-sdk-python-cls-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-cls-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.869.tar", last modified: Mon Apr 10 02:58:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cls-3.0.870.tar", last modified: Tue Apr 11 03:27:18 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cls-3.0.869.tar` & `tencentcloud-sdk-python-cls-3.0.870.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)   238657 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)    66970 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/cls_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/README.rst
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 02:58:55.000000 tencentcloud-sdk-python-cls-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)   240074 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)    66970 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/v20201016/cls_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud_sdk_python_cls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud_sdk_python_cls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud_sdk_python_cls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud_sdk_python_cls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/tencentcloud_sdk_python_cls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:27:18.000000 tencentcloud-sdk-python-cls-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cls-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.870/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cls-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/v20201016/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4062,14 +4062,39 @@
                 obj = TopicInfo()
                 obj._deserialize(item)
                 self.Topics.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DynamicIndex(AbstractModel):
+    """动态更新索引配置
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: 动态索引配置开关
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: bool
+        """
+        self.Status = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ExcludePathInfo(AbstractModel):
     """黑名单path信息
 
     """
 
     def __init__(self):
         r"""
@@ -6220,30 +6245,37 @@
         :type FullText: :class:`tencentcloud.cls.v20201016.models.FullTextInfo`
         :param KeyValue: 键值索引配置，如果为空时代表未开启键值索引
 注意：此字段可能返回 null，表示取不到有效值。
         :type KeyValue: :class:`tencentcloud.cls.v20201016.models.RuleKeyValueInfo`
         :param Tag: 元字段索引配置，如果为空时代表未开启元字段索引
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tag: :class:`tencentcloud.cls.v20201016.models.RuleTagInfo`
+        :param DynamicIndex: 动态索引配置，如果为空时代表未开启动态段索引
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DynamicIndex: :class:`tencentcloud.cls.v20201016.models.DynamicIndex`
         """
         self.FullText = None
         self.KeyValue = None
         self.Tag = None
+        self.DynamicIndex = None
 
 
     def _deserialize(self, params):
         if params.get("FullText") is not None:
             self.FullText = FullTextInfo()
             self.FullText._deserialize(params.get("FullText"))
         if params.get("KeyValue") is not None:
             self.KeyValue = RuleKeyValueInfo()
             self.KeyValue._deserialize(params.get("KeyValue"))
         if params.get("Tag") is not None:
             self.Tag = RuleTagInfo()
             self.Tag._deserialize(params.get("Tag"))
+        if params.get("DynamicIndex") is not None:
+            self.DynamicIndex = DynamicIndex()
+            self.DynamicIndex._deserialize(params.get("DynamicIndex"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6356,15 +6388,15 @@
 0：自动采样;
 0～1：按指定采样率采样，例如0.02;
 1：不采样，即精确分析
 默认值为1
         :type SamplingRate: float
         :param SyntaxRule: 检索语法规则，默认值为0。
 0：Lucene语法，1：CQL语法。
-详细说明参见https://cloud.tencent.com/document/product/614/47044#RetrievesConditionalRules
+详细说明参见<a href="https://cloud.tencent.com/document/product/614/47044#RetrievesConditionalRules" target="_blank">检索条件语法规则</a>
         :type SyntaxRule: int
         """
         self.From = None
         self.To = None
         self.Query = None
         self.TopicId = None
         self.Limit = None
@@ -6424,25 +6456,29 @@
 当UseNewAnalysis为true时生效
 注意：此字段可能返回 null，表示取不到有效值。
         :type AnalysisRecords: list of str
         :param Columns: 日志统计分析结果的列属性
 当UseNewAnalysis为true时生效
 注意：此字段可能返回 null，表示取不到有效值。
         :type Columns: list of Column
+        :param SamplingRate: 本次统计分析使用的采样率
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SamplingRate: float
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.Context = None
         self.ListOver = None
         self.Analysis = None
         self.Results = None
         self.ColNames = None
         self.AnalysisResults = None
         self.AnalysisRecords = None
         self.Columns = None
+        self.SamplingRate = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.Context = params.get("Context")
         self.ListOver = params.get("ListOver")
         self.Analysis = params.get("Analysis")
@@ -6462,14 +6498,15 @@
         self.AnalysisRecords = params.get("AnalysisRecords")
         if params.get("Columns") is not None:
             self.Columns = []
             for item in params.get("Columns"):
                 obj = Column()
                 obj._deserialize(item)
                 self.Columns.append(obj)
+        self.SamplingRate = params.get("SamplingRate")
         self.RequestId = params.get("RequestId")
 
 
 class ShipperInfo(AbstractModel):
     """投递规则
 
     """
```

### Comparing `tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.869/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-cls-3.0.870/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.869/tencentcloud_sdk_python_cls.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cls-3.0.870/tencentcloud_sdk_python_cls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cls
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Cls SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cls-3.0.869/README.rst` & `tencentcloud-sdk-python-cls-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cls-3.0.869/setup.py` & `tencentcloud-sdk-python-cls-3.0.870/setup.py`

 * *Files identical despite different names*

