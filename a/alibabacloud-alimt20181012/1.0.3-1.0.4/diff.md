# Comparing `tmp/alibabacloud_alimt20181012-1.0.3.tar.gz` & `tmp/alibabacloud_alimt20181012-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_alimt20181012-1.0.3.tar", last modified: Fri Oct 14 06:48:22 2022, max compression
+gzip compressed data, was "dist/alibabacloud_alimt20181012-1.0.4.tar", last modified: Tue Apr 11 08:51:38 2023, max compression
```

## Comparing `alibabacloud_alimt20181012-1.0.3.tar` & `alibabacloud_alimt20181012-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      190 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1028 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1113 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012/
--rw-r--r--   0 root         (0) root         (0)       21 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79380 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012/client.py
--rw-r--r--   0 root         (0) root         (0)    93064 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      315 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-14 06:48:22.000000 alibabacloud_alimt20181012-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2825 2022-10-14 06:48:21.000000 alibabacloud_alimt20181012-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85868 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/client.py
+-rw-r--r--   0 root         (0) root         (0)   105220 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      315 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-04-11 08:51:38.000000 alibabacloud_alimt20181012-1.0.4/setup.py
```

### Comparing `alibabacloud_alimt20181012-1.0.3/LICENSE` & `alibabacloud_alimt20181012-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.0.3/PKG-INFO` & `alibabacloud_alimt20181012-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_alimt20181012
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012-1.0.3/README-CN.md` & `alibabacloud_alimt20181012-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.0.3/README.md` & `alibabacloud_alimt20181012-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012/client.py` & `alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1136,14 +1136,84 @@
     async def get_title_intelligence_async(
         self,
         request: alimt_20181012_models.GetTitleIntelligenceRequest,
     ) -> alimt_20181012_models.GetTitleIntelligenceResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_title_intelligence_with_options_async(request, runtime)
 
+    def get_translate_image_batch_result_with_options(
+        self,
+        request: alimt_20181012_models.GetTranslateImageBatchResultRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alimt_20181012_models.GetTranslateImageBatchResultResponse:
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
+    async def get_translate_image_batch_result_with_options_async(
+        self,
+        request: alimt_20181012_models.GetTranslateImageBatchResultRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alimt_20181012_models.GetTranslateImageBatchResultResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_translate_image_batch_result(
+        self,
+        request: alimt_20181012_models.GetTranslateImageBatchResultRequest,
+    ) -> alimt_20181012_models.GetTranslateImageBatchResultResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_translate_image_batch_result_with_options(request, runtime)
+
+    async def get_translate_image_batch_result_async(
+        self,
+        request: alimt_20181012_models.GetTranslateImageBatchResultRequest,
+    ) -> alimt_20181012_models.GetTranslateImageBatchResultResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_translate_image_batch_result_with_options_async(request, runtime)
+
     def get_translate_report_with_options(
         self,
         request: alimt_20181012_models.GetTranslateReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> alimt_20181012_models.GetTranslateReportResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -1891,7 +1961,97 @@
 
     async def translate_image_async(
         self,
         request: alimt_20181012_models.TranslateImageRequest,
     ) -> alimt_20181012_models.TranslateImageResponse:
         runtime = util_models.RuntimeOptions()
         return await self.translate_image_with_options_async(request, runtime)
+
+    def translate_image_batch_with_options(
+        self,
+        request: alimt_20181012_models.TranslateImageBatchRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alimt_20181012_models.TranslateImageBatchResponse:
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
+    async def translate_image_batch_with_options_async(
+        self,
+        request: alimt_20181012_models.TranslateImageBatchRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> alimt_20181012_models.TranslateImageBatchResponse:
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
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def translate_image_batch(
+        self,
+        request: alimt_20181012_models.TranslateImageBatchRequest,
+    ) -> alimt_20181012_models.TranslateImageBatchResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.translate_image_batch_with_options(request, runtime)
+
+    async def translate_image_batch_async(
+        self,
+        request: alimt_20181012_models.TranslateImageBatchRequest,
+    ) -> alimt_20181012_models.TranslateImageBatchResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.translate_image_batch_with_options_async(request, runtime)
```

### Comparing `alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012/models.py` & `alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1794,14 +1794,236 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetTitleIntelligenceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetTranslateImageBatchResultRequest(TeaModel):
+    def __init__(
+        self,
+        task_id: str = None,
+    ):
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class GetTranslateImageBatchResultResponseBodyDataResult(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        final_image_url: str = None,
+        in_painting_url: str = None,
+        message: str = None,
+        source_image_url: str = None,
+        success: bool = None,
+        template_json: str = None,
+    ):
+        self.code = code
+        self.final_image_url = final_image_url
+        self.in_painting_url = in_painting_url
+        self.message = message
+        self.source_image_url = source_image_url
+        self.success = success
+        self.template_json = template_json
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        result: List[GetTranslateImageBatchResultResponseBodyDataResult] = None,
+        status: str = None,
+    ):
+        self.result = result
+        self.status = status
+
+    def validate(self):
+        if self.result:
+            for k in self.result:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        code: int = None,
+        data: GetTranslateImageBatchResultResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetTranslateImageBatchResultResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
     def __init__(
         self,
         api_name: str = None,
         begin_time: str = None,
         end_time: str = None,
         group: str = None,
@@ -3029,7 +3251,182 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = TranslateImageResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TranslateImageBatchRequest(TeaModel):
+    def __init__(
+        self,
+        custom_task_id: str = None,
+        ext: str = None,
+        field: str = None,
+        image_urls: str = None,
+        source_language: str = None,
+        target_language: str = None,
+    ):
+        self.custom_task_id = custom_task_id
+        self.ext = ext
+        self.field = field
+        self.image_urls = image_urls
+        self.source_language = source_language
+        self.target_language = target_language
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        task_id: str = None,
+    ):
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_id is not None:
+            result['TaskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TaskId') is not None:
+            self.task_id = m.get('TaskId')
+        return self
+
+
+class TranslateImageBatchResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: int = None,
+        data: TranslateImageBatchResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TranslateImageBatchResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
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
+    def from_map(self, m: dict = None):
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

### Comparing `alibabacloud_alimt20181012-1.0.3/alibabacloud_alimt20181012.egg-info/PKG-INFO` & `alibabacloud_alimt20181012-1.0.4/alibabacloud_alimt20181012.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-alimt20181012
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud Machine Translation (20181012) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_alimt20181012-1.0.3/setup.py` & `alibabacloud_alimt20181012-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,34 +20,34 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_alimt20181012.
 
-Created on 14/10/2022
+Created on 11/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_alimt20181012"
 NAME = "alibabacloud_alimt20181012" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Machine Translation (20181012) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

