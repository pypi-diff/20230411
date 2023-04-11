# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.869.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.869.tar", last modified: Mon Apr 10 03:15:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.870.tar", last modified: Tue Apr 11 03:55:23 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.869.tar` & `tencentcloud-sdk-python-teo-3.0.870.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)   468214 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7631 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    87643 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)   504971 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20753 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    81864 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-10 03:15:36.000000 tencentcloud-sdk-python-teo-3.0.869/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)   468214 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    87643 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)   504971 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20875 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    81864 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-11 03:55:23.000000 tencentcloud-sdk-python-teo-3.0.870/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.869/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.870/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 后台处理出错。
 INTERNALERROR_BACKENDERROR = 'InternalError.BackendError'
 
+# 配置已被锁定，请解除配置锁定之后在重试。
+INTERNALERROR_CONFIGLOCKED = 'InternalError.ConfigLocked'
+
 # 数据库错误。
 INTERNALERROR_DBERROR = 'InternalError.DBError'
 
 # 获取配置失败。
 INTERNALERROR_DOMAINCONFIG = 'InternalError.DomainConfig'
 
 # 上传链接生成失败。
```

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.869/README.rst` & `tencentcloud-sdk-python-teo-3.0.870/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.869
+Version: 3.0.870
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.869/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.870/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.869/setup.py` & `tencentcloud-sdk-python-teo-3.0.870/setup.py`

 * *Files identical despite different names*

