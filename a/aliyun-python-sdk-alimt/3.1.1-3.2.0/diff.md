# Comparing `tmp/aliyun-python-sdk-alimt-3.1.1.tar.gz` & `tmp/aliyun-python-sdk-alimt-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-alimt-3.1.1.tar", last modified: Mon Nov 15 06:45:05 2021, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-alimt-3.2.0.tar", last modified: Tue Apr 11 09:25:52 2023, max compression
```

## Comparing `aliyun-python-sdk-alimt-3.1.1.tar` & `aliyun-python-sdk-alimt-3.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/
--rw-r--r--   0 root         (0) root         (0)      575 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1547 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyun_python_sdk_alimt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1547 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyun_python_sdk_alimt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1576 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyun_python_sdk_alimt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyun_python_sdk_alimt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyun_python_sdk_alimt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyun_python_sdk_alimt.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/
--rw-r--r--   0 root         (0) root         (0)       21 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3396 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/
--rw-r--r--   0 root         (0) root         (0)     2436 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/CreateDocTranslateTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2244 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/CreateImageTranslateTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2414 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetBatchTranslateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1464 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetDetectLanguageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1444 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetDocTranslateTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1580 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetImageDiagnoseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2010 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetImageTranslateRequest.py
--rw-r--r--   0 root         (0) root         (0)     1448 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetImageTranslateTaskRequest.py
--rw-r--r--   0 root         (0) root         (0)     2138 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetTitleDiagnoseRequest.py
--rw-r--r--   0 root         (0) root         (0)     2506 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetTitleGenerateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2216 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetTitleIntelligenceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1968 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetTranslateReportRequest.py
--rw-r--r--   0 root         (0) root         (0)     1254 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1596 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/OpenAlimtServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2296 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateCertificateRequest.py
--rw-r--r--   0 root         (0) root         (0)     2244 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateECommerceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2240 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateGeneralRequest.py
--rw-r--r--   0 root         (0) root         (0)     2378 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateImageRequest.py
--rw-r--r--   0 root         (0) root         (0)     2226 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2462 2021-11-15 06:45:05.000000 aliyun-python-sdk-alimt-3.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyun_python_sdk_alimt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyun_python_sdk_alimt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyun_python_sdk_alimt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyun_python_sdk_alimt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyun_python_sdk_alimt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyun_python_sdk_alimt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/CreateDocTranslateTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/CreateImageTranslateTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetBatchTranslateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetDetectLanguageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetDocTranslateTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetImageDiagnoseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2010 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetImageTranslateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetImageTranslateTaskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTitleDiagnoseRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTitleGenerateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTitleIntelligenceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTranslateImageBatchResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTranslateReportRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/OpenAlimtServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateCertificateRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateECommerceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateGeneralRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateImageBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateImageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-04-11 09:25:52.000000 aliyun-python-sdk-alimt-3.2.0/setup.py
```

### Comparing `aliyun-python-sdk-alimt-3.1.1/LICENSE` & `aliyun-python-sdk-alimt-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/PKG-INFO` & `aliyun-python-sdk-alimt-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alimt
-Version: 3.1.1
+Version: 3.2.0
 Summary: The alimt module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alimt
```

### Comparing `aliyun-python-sdk-alimt-3.1.1/README.rst` & `aliyun-python-sdk-alimt-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyun_python_sdk_alimt.egg-info/PKG-INFO` & `aliyun-python-sdk-alimt-3.2.0/aliyun_python_sdk_alimt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alimt
-Version: 3.1.1
+Version: 3.2.0
 Summary: The alimt module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alimt
```

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyun_python_sdk_alimt.egg-info/SOURCES.txt` & `aliyun-python-sdk-alimt-3.2.0/aliyun_python_sdk_alimt.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 aliyunsdkalimt/request/v20181012/GetDocTranslateTaskRequest.py
 aliyunsdkalimt/request/v20181012/GetImageDiagnoseRequest.py
 aliyunsdkalimt/request/v20181012/GetImageTranslateRequest.py
 aliyunsdkalimt/request/v20181012/GetImageTranslateTaskRequest.py
 aliyunsdkalimt/request/v20181012/GetTitleDiagnoseRequest.py
 aliyunsdkalimt/request/v20181012/GetTitleGenerateRequest.py
 aliyunsdkalimt/request/v20181012/GetTitleIntelligenceRequest.py
+aliyunsdkalimt/request/v20181012/GetTranslateImageBatchResultRequest.py
 aliyunsdkalimt/request/v20181012/GetTranslateReportRequest.py
-aliyunsdkalimt/request/v20181012/GetUserRequest.py
 aliyunsdkalimt/request/v20181012/OpenAlimtServiceRequest.py
 aliyunsdkalimt/request/v20181012/TranslateCertificateRequest.py
 aliyunsdkalimt/request/v20181012/TranslateECommerceRequest.py
 aliyunsdkalimt/request/v20181012/TranslateGeneralRequest.py
+aliyunsdkalimt/request/v20181012/TranslateImageBatchRequest.py
 aliyunsdkalimt/request/v20181012/TranslateImageRequest.py
 aliyunsdkalimt/request/v20181012/TranslateRequest.py
 aliyunsdkalimt/request/v20181012/__init__.py
```

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/endpoint.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/CreateDocTranslateTaskRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/CreateDocTranslateTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/CreateImageTranslateTaskRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/CreateImageTranslateTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetBatchTranslateRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetBatchTranslateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetDetectLanguageRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetDetectLanguageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetDocTranslateTaskRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetDocTranslateTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetImageDiagnoseRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetImageDiagnoseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetImageTranslateRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetImageTranslateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetImageTranslateTaskRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetImageTranslateTaskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetTitleDiagnoseRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTitleDiagnoseRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetTitleGenerateRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTitleGenerateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetTitleIntelligenceRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTitleIntelligenceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetTranslateReportRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTranslateReportRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/GetUserRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/GetTranslateImageBatchResultRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,18 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalimt.endpoint import endpoint_data
 
-class GetUserRequest(RpcRequest):
+class GetTranslateImageBatchResultRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alimt', '2018-10-12', 'GetUser')
+		RpcRequest.__init__(self, 'alimt', '2018-10-12', 'GetTranslateImageBatchResult')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_TaskId(self): # String
+		return self.get_body_params().get('TaskId')
+
+	def set_TaskId(self, TaskId):  # String
+		self.add_body_params('TaskId', TaskId)
```

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/OpenAlimtServiceRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/OpenAlimtServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateCertificateRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateCertificateRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateECommerceRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalimt.endpoint import endpoint_data
 
-class TranslateECommerceRequest(RpcRequest):
+class TranslateRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alimt', '2018-10-12', 'TranslateECommerce')
+		RpcRequest.__init__(self, 'alimt', '2018-10-12', 'Translate')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -47,12 +47,17 @@
 	def set_FormatType(self, FormatType):  # String
 		self.add_body_params('FormatType', FormatType)
 	def get_Scene(self): # String
 		return self.get_body_params().get('Scene')
 
 	def set_Scene(self, Scene):  # String
 		self.add_body_params('Scene', Scene)
+	def get_Context(self): # String
+		return self.get_query_params().get('Context')
+
+	def set_Context(self, Context):  # String
+		self.add_query_param('Context', Context)
 	def get_TargetLanguage(self): # String
 		return self.get_body_params().get('TargetLanguage')
 
 	def set_TargetLanguage(self, TargetLanguage):  # String
 		self.add_body_params('TargetLanguage', TargetLanguage)
```

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateGeneralRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateECommerceRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalimt.endpoint import endpoint_data
 
-class TranslateGeneralRequest(RpcRequest):
+class TranslateECommerceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alimt', '2018-10-12', 'TranslateGeneral')
+		RpcRequest.__init__(self, 'alimt', '2018-10-12', 'TranslateECommerce')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -47,12 +47,17 @@
 	def set_FormatType(self, FormatType):  # String
 		self.add_body_params('FormatType', FormatType)
 	def get_Scene(self): # String
 		return self.get_body_params().get('Scene')
 
 	def set_Scene(self, Scene):  # String
 		self.add_body_params('Scene', Scene)
+	def get_Context(self): # String
+		return self.get_query_params().get('Context')
+
+	def set_Context(self, Context):  # String
+		self.add_query_param('Context', Context)
 	def get_TargetLanguage(self): # String
 		return self.get_body_params().get('TargetLanguage')
 
 	def set_TargetLanguage(self, TargetLanguage):  # String
 		self.add_body_params('TargetLanguage', TargetLanguage)
```

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateImageRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alimt-3.1.1/aliyunsdkalimt/request/v20181012/TranslateRequest.py` & `aliyun-python-sdk-alimt-3.2.0/aliyunsdkalimt/request/v20181012/TranslateGeneralRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalimt.endpoint import endpoint_data
 
-class TranslateRequest(RpcRequest):
+class TranslateGeneralRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alimt', '2018-10-12', 'Translate')
+		RpcRequest.__init__(self, 'alimt', '2018-10-12', 'TranslateGeneral')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -47,12 +47,17 @@
 	def set_FormatType(self, FormatType):  # String
 		self.add_body_params('FormatType', FormatType)
 	def get_Scene(self): # String
 		return self.get_body_params().get('Scene')
 
 	def set_Scene(self, Scene):  # String
 		self.add_body_params('Scene', Scene)
+	def get_Context(self): # String
+		return self.get_query_params().get('Context')
+
+	def set_Context(self, Context):  # String
+		self.add_query_param('Context', Context)
 	def get_TargetLanguage(self): # String
 		return self.get_body_params().get('TargetLanguage')
 
 	def set_TargetLanguage(self, TargetLanguage):  # String
 		self.add_body_params('TargetLanguage', TargetLanguage)
```

### Comparing `aliyun-python-sdk-alimt-3.1.1/setup.py` & `aliyun-python-sdk-alimt-3.2.0/setup.py`

 * *Files identical despite different names*

