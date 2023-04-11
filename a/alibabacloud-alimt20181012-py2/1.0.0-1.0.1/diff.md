# Comparing `tmp/alibabacloud_alimt20181012_py2-1.0.0.tar.gz` & `tmp/alibabacloud_alimt20181012_py2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alimt20181012_py2-1.0.0.tar", last modified: Fri Oct 14 06:47:53 2022, max compression
+gzip compressed data, was "dist/alibabacloud_alimt20181012_py2-1.0.1.tar", last modified: Tue Apr 11 08:51:19 2023, max compression
```

## Comparing `alibabacloud_alimt20181012_py2-1.0.0.tar` & `alibabacloud_alimt20181012_py2-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      588 2022-10-14 06:47:52.000000 alibabacloud_alimt20181012_py2-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2022-10-14 06:47:52.000000 alibabacloud_alimt20181012_py2-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2498 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1039 2022-10-14 06:47:52.000000 alibabacloud_alimt20181012_py2-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2022-10-14 06:47:52.000000 alibabacloud_alimt20181012_py2-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012/
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-14 06:47:52.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36224 2022-10-14 06:47:52.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012/client.py
--rw-r--r--   0 root         (0) root         (0)    93539 2022-10-14 06:47:52.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2498 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      347 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-14 06:47:53.000000 alibabacloud_alimt20181012_py2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3134 2022-10-14 06:47:52.000000 alibabacloud_alimt20181012_py2-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:19.000000 alibabacloud_alimt20181012_py2-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-04-11 08:51:19.000000 alibabacloud_alimt20181012_py2-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:19.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38808 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012/client.py
+-rw-r--r--   0 root         (0) root         (0)   105838 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:19.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      347 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 08:51:19.000000 alibabacloud_alimt20181012_py2-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-04-11 08:51:18.000000 alibabacloud_alimt20181012_py2-1.0.1/setup.py
```

### Comparing `alibabacloud_alimt20181012_py2-1.0.0/LICENSE` & `alibabacloud_alimt20181012_py2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012_py2-1.0.0/PKG-INFO` & `alibabacloud_alimt20181012_py2-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alimt20181012_py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012_py2-1.0.0/README-CN.md` & `alibabacloud_alimt20181012_py2-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012_py2-1.0.0/README.md` & `alibabacloud_alimt20181012_py2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012/client.py` & `alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -527,14 +527,42 @@
             self.call_api(params, req, runtime)
         )
 
     def get_title_intelligence(self, request):
         runtime = util_models.RuntimeOptions()
         return self.get_title_intelligence_with_options(request, runtime)
 
+    def get_translate_image_batch_result_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.task_id):
+            body['TaskId'] = request.task_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetTranslateImageBatchResult',
+            version='2018-10-12',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alimt_20181012_models.GetTranslateImageBatchResultResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def get_translate_image_batch_result(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.get_translate_image_batch_result_with_options(request, runtime)
+
     def get_translate_report_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.api_name):
             query['ApiName'] = request.api_name
         if not UtilClient.is_unset(request.begin_time):
             query['BeginTime'] = request.begin_time
@@ -851,7 +879,45 @@
             alimt_20181012_models.TranslateImageResponse(),
             self.call_api(params, req, runtime)
         )
 
     def translate_image(self, request):
         runtime = util_models.RuntimeOptions()
         return self.translate_image_with_options(request, runtime)
+
+    def translate_image_batch_with_options(self, request, runtime):
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.custom_task_id):
+            body['CustomTaskId'] = request.custom_task_id
+        if not UtilClient.is_unset(request.ext):
+            body['Ext'] = request.ext
+        if not UtilClient.is_unset(request.field):
+            body['Field'] = request.field
+        if not UtilClient.is_unset(request.image_urls):
+            body['ImageUrls'] = request.image_urls
+        if not UtilClient.is_unset(request.source_language):
+            body['SourceLanguage'] = request.source_language
+        if not UtilClient.is_unset(request.target_language):
+            body['TargetLanguage'] = request.target_language
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='TranslateImageBatch',
+            version='2018-10-12',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            alimt_20181012_models.TranslateImageBatchResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    def translate_image_batch(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.translate_image_batch_with_options(request, runtime)
```

### Comparing `alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012/models.py` & `alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1574,14 +1574,210 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetTitleIntelligenceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetTranslateImageBatchResultRequest(TeaModel):
+    def __init__(self, task_id=None):
+        self.task_id = task_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetTranslateImageBatchResultRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class GetTranslateImageBatchResultResponseBodyDataResult(TeaModel):
+    def __init__(self, code=None, final_image_url=None, in_painting_url=None, message=None, source_image_url=None,
+                 success=None, template_json=None):
+        self.code = code  # type: int
+        self.final_image_url = final_image_url  # type: str
+        self.in_painting_url = in_painting_url  # type: str
+        self.message = message  # type: str
+        self.source_image_url = source_image_url  # type: str
+        self.success = success  # type: bool
+        self.template_json = template_json  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(GetTranslateImageBatchResultResponseBodyDataResult, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.final_image_url is not None:
+            result['FinalImageUrl'] = self.final_image_url
+        if self.in_painting_url is not None:
+            result['InPaintingUrl'] = self.in_painting_url
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.source_image_url is not None:
+            result['SourceImageUrl'] = self.source_image_url
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.template_json is not None:
+            result['TemplateJson'] = self.template_json
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('FinalImageUrl') is not None:
+            self.final_image_url = m.get('FinalImageUrl')
+        if m.get('InPaintingUrl') is not None:
+            self.in_painting_url = m.get('InPaintingUrl')
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('SourceImageUrl') is not None:
+            self.source_image_url = m.get('SourceImageUrl')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('TemplateJson') is not None:
+            self.template_json = m.get('TemplateJson')
+        return self
+
+
+class GetTranslateImageBatchResultResponseBodyData(TeaModel):
+    def __init__(self, result=None, status=None):
+        self.result = result  # type: list[GetTranslateImageBatchResultResponseBodyDataResult]
+        self.status = status  # type: str
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(GetTranslateImageBatchResultResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Result'] = []
+        if self.result is not None:
+            for k in self.result:
+                result['Result'].append(k.to_map() if k else None)
+        if self.status is not None:
+            result['Status'] = self.status
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        self.result = []
+        if m.get('Result') is not None:
+            for k in m.get('Result'):
+                temp_model = GetTranslateImageBatchResultResponseBodyDataResult()
+                self.result.append(temp_model.from_map(k))
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        return self
+
+
+class GetTranslateImageBatchResultResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
+        self.code = code  # type: int
+        self.data = data  # type: GetTranslateImageBatchResultResponseBodyData
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(GetTranslateImageBatchResultResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = GetTranslateImageBatchResultResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class GetTranslateImageBatchResultResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: GetTranslateImageBatchResultResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(GetTranslateImageBatchResultResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetTranslateImageBatchResultResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetTranslateReportRequest(TeaModel):
     def __init__(self, api_name=None, begin_time=None, end_time=None, group=None):
         self.api_name = api_name  # type: str
         self.begin_time = begin_time  # type: str
         self.end_time = end_time  # type: str
         self.group = group  # type: str
 
@@ -2660,7 +2856,161 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = TranslateImageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TranslateImageBatchRequest(TeaModel):
+    def __init__(self, custom_task_id=None, ext=None, field=None, image_urls=None, source_language=None,
+                 target_language=None):
+        self.custom_task_id = custom_task_id  # type: str
+        self.ext = ext  # type: str
+        self.field = field  # type: str
+        self.image_urls = image_urls  # type: str
+        self.source_language = source_language  # type: str
+        self.target_language = target_language  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(TranslateImageBatchRequest, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.custom_task_id is not None:
+            result['CustomTaskId'] = self.custom_task_id
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.field is not None:
+            result['Field'] = self.field
+        if self.image_urls is not None:
+            result['ImageUrls'] = self.image_urls
+        if self.source_language is not None:
+            result['SourceLanguage'] = self.source_language
+        if self.target_language is not None:
+            result['TargetLanguage'] = self.target_language
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CustomTaskId') is not None:
+            self.custom_task_id = m.get('CustomTaskId')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('Field') is not None:
+            self.field = m.get('Field')
+        if m.get('ImageUrls') is not None:
+            self.image_urls = m.get('ImageUrls')
+        if m.get('SourceLanguage') is not None:
+            self.source_language = m.get('SourceLanguage')
+        if m.get('TargetLanguage') is not None:
+            self.target_language = m.get('TargetLanguage')
+        return self
+
+
+class TranslateImageBatchResponseBodyData(TeaModel):
+    def __init__(self, task_id=None):
+        self.task_id = task_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(TranslateImageBatchResponseBodyData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class TranslateImageBatchResponseBody(TeaModel):
+    def __init__(self, code=None, data=None, message=None, request_id=None):
+        self.code = code  # type: int
+        self.data = data  # type: TranslateImageBatchResponseBodyData
+        self.message = message  # type: str
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(TranslateImageBatchResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = TranslateImageBatchResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class TranslateImageBatchResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: TranslateImageBatchResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(TranslateImageBatchResponse, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TranslateImageBatchResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_alimt20181012_py2-1.0.0/alibabacloud_alimt20181012_py2.egg-info/PKG-INFO` & `alibabacloud_alimt20181012_py2-1.0.1/alibabacloud_alimt20181012_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alimt20181012-py2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012_py2-1.0.0/setup.py` & `alibabacloud_alimt20181012_py2-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,34 +21,34 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alimt20181012_py2.
 
-Created on 14/10/2022
+Created on 11/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alimt20181012"
 NAME = "alibabacloud_alimt20181012_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Machine Translation (20181012) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
     "alibabacloud_oss_sdk_py2>=0.0.1, <1.0.0",
     "alibabacloud_openplatform20191219_py2>=1.0.0, <2.0.0",
     "alibabacloud_oss_util_py2>=0.0.1, <1.0.0",
     "alibabacloud_tea_fileform_py2>=0.0.1, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.3, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
```

