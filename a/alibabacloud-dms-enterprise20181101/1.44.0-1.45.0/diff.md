# Comparing `tmp/alibabacloud_dms-enterprise20181101-1.44.0.tar.gz` & `tmp/alibabacloud_dms-enterprise20181101-1.45.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.44.0.tar", last modified: Fri Jan 13 02:30:33 2023, max compression
+gzip compressed data, was "dist/alibabacloud_dms-enterprise20181101-1.45.0.tar", last modified: Tue Apr 11 03:36:53 2023, max compression
```

## Comparing `alibabacloud_dms-enterprise20181101-1.44.0.tar` & `alibabacloud_dms-enterprise20181101-1.45.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/
--rw-r--r--   0 root         (0) root         (0)     4512 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2395 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1055 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101/
--rw-r--r--   0 root         (0) root         (0)       22 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   702873 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101/client.py
--rw-r--r--   0 root         (0) root         (0)  1559539 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2395 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      508 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2667 2023-01-13 02:30:33.000000 alibabacloud_dms-enterprise20181101-1.44.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/
+-rw-r--r--   0 root         (0) root         (0)     4668 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   746627 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1685783 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2395 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      508 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-04-11 03:36:53.000000 alibabacloud_dms-enterprise20181101-1.45.0/setup.py
```

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/ChangeLog.md` & `alibabacloud_dms-enterprise20181101-1.45.0/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2023-01-13 Version: 1.44.0
+- Supported GetProxy, ListProxies to return RegionId information.
+- Supported SearchDatabase to return CatalogName information.
+
 2022-12-21 Version: 1.43.0
 - Supported GetProxyAccess API.
 
 2022-12-02 Version: 1.42.0
 - Supported GetStructSyncOrderDetail OrderId param required.
 
 2022-11-23 Version: 1.41.0
```

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/LICENSE` & `alibabacloud_dms-enterprise20181101-1.45.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.45.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dms-enterprise20181101
-Version: 1.44.0
+Version: 1.45.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/README-CN.md` & `alibabacloud_dms-enterprise20181101-1.45.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/README.md` & `alibabacloud_dms-enterprise20181101-1.45.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101/client.py` & `alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1059,14 +1059,118 @@
     async def close_order_async(
         self,
         request: dms_enterprise_20181101_models.CloseOrderRequest,
     ) -> dms_enterprise_20181101_models.CloseOrderResponse:
         runtime = util_models.RuntimeOptions()
         return await self.close_order_with_options_async(request, runtime)
 
+    def create_authority_template_with_options(
+        self,
+        request: dms_enterprise_20181101_models.CreateAuthorityTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateAuthorityTemplateResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: CreateAuthorityTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAuthorityTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateAuthorityTemplate',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateAuthorityTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_authority_template_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.CreateAuthorityTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.CreateAuthorityTemplateResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: CreateAuthorityTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAuthorityTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateAuthorityTemplate',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.CreateAuthorityTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_authority_template(
+        self,
+        request: dms_enterprise_20181101_models.CreateAuthorityTemplateRequest,
+    ) -> dms_enterprise_20181101_models.CreateAuthorityTemplateResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: CreateAuthorityTemplateRequest
+        @return: CreateAuthorityTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.create_authority_template_with_options(request, runtime)
+
+    async def create_authority_template_async(
+        self,
+        request: dms_enterprise_20181101_models.CreateAuthorityTemplateRequest,
+    ) -> dms_enterprise_20181101_models.CreateAuthorityTemplateResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: CreateAuthorityTemplateRequest
+        @return: CreateAuthorityTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.create_authority_template_with_options_async(request, runtime)
+
     def create_data_correct_order_with_options(
         self,
         tmp_req: dms_enterprise_20181101_models.CreateDataCorrectOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.CreateDataCorrectOrderResponse:
         """
         For more information about the Normal Data Modify feature, see [Change regular data](~~58419~~).
@@ -2249,15 +2353,15 @@
 
     def create_sqlreview_order_with_options(
         self,
         tmp_req: dms_enterprise_20181101_models.CreateSQLReviewOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.CreateSQLReviewOrderResponse:
         """
-        For more instructions on this feature, see [SQL audit](~~60374~~) .
+        For more information about the SQL review feature, see [SQL review](~~60374~~).
         
         @param tmp_req: CreateSQLReviewOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSQLReviewOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dms_enterprise_20181101_models.CreateSQLReviewOrderShrinkRequest()
@@ -2296,15 +2400,15 @@
 
     async def create_sqlreview_order_with_options_async(
         self,
         tmp_req: dms_enterprise_20181101_models.CreateSQLReviewOrderRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.CreateSQLReviewOrderResponse:
         """
-        For more instructions on this feature, see [SQL audit](~~60374~~) .
+        For more information about the SQL review feature, see [SQL review](~~60374~~).
         
         @param tmp_req: CreateSQLReviewOrderRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSQLReviewOrderResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dms_enterprise_20181101_models.CreateSQLReviewOrderShrinkRequest()
@@ -2342,28 +2446,28 @@
         )
 
     def create_sqlreview_order(
         self,
         request: dms_enterprise_20181101_models.CreateSQLReviewOrderRequest,
     ) -> dms_enterprise_20181101_models.CreateSQLReviewOrderResponse:
         """
-        For more instructions on this feature, see [SQL audit](~~60374~~) .
+        For more information about the SQL review feature, see [SQL review](~~60374~~).
         
         @param request: CreateSQLReviewOrderRequest
         @return: CreateSQLReviewOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_sqlreview_order_with_options(request, runtime)
 
     async def create_sqlreview_order_async(
         self,
         request: dms_enterprise_20181101_models.CreateSQLReviewOrderRequest,
     ) -> dms_enterprise_20181101_models.CreateSQLReviewOrderResponse:
         """
-        For more instructions on this feature, see [SQL audit](~~60374~~) .
+        For more information about the SQL review feature, see [SQL review](~~60374~~).
         
         @param request: CreateSQLReviewOrderRequest
         @return: CreateSQLReviewOrderResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_sqlreview_order_with_options_async(request, runtime)
 
@@ -4649,16 +4753,16 @@
 
     def execute_struct_sync_with_options(
         self,
         request: dms_enterprise_20181101_models.ExecuteStructSyncRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.ExecuteStructSyncResponse:
         """
-        If the security rules of the instance need to be approved for synchronization, call [SubmitStructSyncOrderApproval](~~206166~~) The interface initiates an approval process and completes the approval.
-        >  You can call [GetStructSyncJobDetail](~~206160~~) You can call this operation to query whether the target instance requires an approval.
+        If the security rules of an instance indicate that a ticket must be approved before you perform schema synchronization, you can call the [SubmitStructSyncOrderApproval](~~206166~~) operation to submit the ticket for approval.
+        >  You can call the [GetStructSyncJobDetail](~~206160~~) operation to query whether you need to submit a ticket for approval.
         
         @param request: ExecuteStructSyncRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ExecuteStructSyncResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4687,16 +4791,16 @@
 
     async def execute_struct_sync_with_options_async(
         self,
         request: dms_enterprise_20181101_models.ExecuteStructSyncRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.ExecuteStructSyncResponse:
         """
-        If the security rules of the instance need to be approved for synchronization, call [SubmitStructSyncOrderApproval](~~206166~~) The interface initiates an approval process and completes the approval.
-        >  You can call [GetStructSyncJobDetail](~~206160~~) You can call this operation to query whether the target instance requires an approval.
+        If the security rules of an instance indicate that a ticket must be approved before you perform schema synchronization, you can call the [SubmitStructSyncOrderApproval](~~206166~~) operation to submit the ticket for approval.
+        >  You can call the [GetStructSyncJobDetail](~~206160~~) operation to query whether you need to submit a ticket for approval.
         
         @param request: ExecuteStructSyncRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ExecuteStructSyncResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4724,30 +4828,30 @@
         )
 
     def execute_struct_sync(
         self,
         request: dms_enterprise_20181101_models.ExecuteStructSyncRequest,
     ) -> dms_enterprise_20181101_models.ExecuteStructSyncResponse:
         """
-        If the security rules of the instance need to be approved for synchronization, call [SubmitStructSyncOrderApproval](~~206166~~) The interface initiates an approval process and completes the approval.
-        >  You can call [GetStructSyncJobDetail](~~206160~~) You can call this operation to query whether the target instance requires an approval.
+        If the security rules of an instance indicate that a ticket must be approved before you perform schema synchronization, you can call the [SubmitStructSyncOrderApproval](~~206166~~) operation to submit the ticket for approval.
+        >  You can call the [GetStructSyncJobDetail](~~206160~~) operation to query whether you need to submit a ticket for approval.
         
         @param request: ExecuteStructSyncRequest
         @return: ExecuteStructSyncResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.execute_struct_sync_with_options(request, runtime)
 
     async def execute_struct_sync_async(
         self,
         request: dms_enterprise_20181101_models.ExecuteStructSyncRequest,
     ) -> dms_enterprise_20181101_models.ExecuteStructSyncResponse:
         """
-        If the security rules of the instance need to be approved for synchronization, call [SubmitStructSyncOrderApproval](~~206166~~) The interface initiates an approval process and completes the approval.
-        >  You can call [GetStructSyncJobDetail](~~206160~~) You can call this operation to query whether the target instance requires an approval.
+        If the security rules of an instance indicate that a ticket must be approved before you perform schema synchronization, you can call the [SubmitStructSyncOrderApproval](~~206166~~) operation to submit the ticket for approval.
+        >  You can call the [GetStructSyncJobDetail](~~206160~~) operation to query whether you need to submit a ticket for approval.
         
         @param request: ExecuteStructSyncRequest
         @return: ExecuteStructSyncResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.execute_struct_sync_with_options_async(request, runtime)
 
@@ -4821,14 +4925,214 @@
     async def get_approval_detail_async(
         self,
         request: dms_enterprise_20181101_models.GetApprovalDetailRequest,
     ) -> dms_enterprise_20181101_models.GetApprovalDetailResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_approval_detail_with_options_async(request, runtime)
 
+    def get_authority_template_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetAuthorityTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetAuthorityTemplateResponse:
+        """
+        You must be a Data Management (DMS) administrator or a database administrator (DBA). For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GetAuthorityTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAuthorityTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAuthorityTemplate',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetAuthorityTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_authority_template_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetAuthorityTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetAuthorityTemplateResponse:
+        """
+        You must be a Data Management (DMS) administrator or a database administrator (DBA). For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GetAuthorityTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAuthorityTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAuthorityTemplate',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetAuthorityTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_authority_template(
+        self,
+        request: dms_enterprise_20181101_models.GetAuthorityTemplateRequest,
+    ) -> dms_enterprise_20181101_models.GetAuthorityTemplateResponse:
+        """
+        You must be a Data Management (DMS) administrator or a database administrator (DBA). For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GetAuthorityTemplateRequest
+        @return: GetAuthorityTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.get_authority_template_with_options(request, runtime)
+
+    async def get_authority_template_async(
+        self,
+        request: dms_enterprise_20181101_models.GetAuthorityTemplateRequest,
+    ) -> dms_enterprise_20181101_models.GetAuthorityTemplateResponse:
+        """
+        You must be a Data Management (DMS) administrator or a database administrator (DBA). For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GetAuthorityTemplateRequest
+        @return: GetAuthorityTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.get_authority_template_with_options_async(request, runtime)
+
+    def get_authority_template_item_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GetAuthorityTemplateItemRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetAuthorityTemplateItemResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GetAuthorityTemplateItemRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAuthorityTemplateItemResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAuthorityTemplateItem',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetAuthorityTemplateItemResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_authority_template_item_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetAuthorityTemplateItemRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetAuthorityTemplateItemResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GetAuthorityTemplateItemRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetAuthorityTemplateItemResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetAuthorityTemplateItem',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetAuthorityTemplateItemResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_authority_template_item(
+        self,
+        request: dms_enterprise_20181101_models.GetAuthorityTemplateItemRequest,
+    ) -> dms_enterprise_20181101_models.GetAuthorityTemplateItemResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GetAuthorityTemplateItemRequest
+        @return: GetAuthorityTemplateItemResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.get_authority_template_item_with_options(request, runtime)
+
+    async def get_authority_template_item_async(
+        self,
+        request: dms_enterprise_20181101_models.GetAuthorityTemplateItemRequest,
+    ) -> dms_enterprise_20181101_models.GetAuthorityTemplateItemResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GetAuthorityTemplateItemRequest
+        @return: GetAuthorityTemplateItemResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.get_authority_template_item_with_options_async(request, runtime)
+
     def get_dbtask_sqljob_log_with_options(
         self,
         request: dms_enterprise_20181101_models.GetDBTaskSQLJobLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetDBTaskSQLJobLogResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -5209,15 +5513,15 @@
 
     def get_data_correct_sqlfile_with_options(
         self,
         request: dms_enterprise_20181101_models.GetDataCorrectSQLFileRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetDataCorrectSQLFileResponse:
         """
-        This interface applies to: [Common data change](~~58419~~) and [Batch Data import](~~144643~~) .
+        This operation applies to [regular data change](~~58419~~) and [batch data import](~~144643~~).
         
         @param request: GetDataCorrectSQLFileRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDataCorrectSQLFileResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5246,15 +5550,15 @@
 
     async def get_data_correct_sqlfile_with_options_async(
         self,
         request: dms_enterprise_20181101_models.GetDataCorrectSQLFileRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetDataCorrectSQLFileResponse:
         """
-        This interface applies to: [Common data change](~~58419~~) and [Batch Data import](~~144643~~) .
+        This operation applies to [regular data change](~~58419~~) and [batch data import](~~144643~~).
         
         @param request: GetDataCorrectSQLFileRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetDataCorrectSQLFileResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5282,28 +5586,28 @@
         )
 
     def get_data_correct_sqlfile(
         self,
         request: dms_enterprise_20181101_models.GetDataCorrectSQLFileRequest,
     ) -> dms_enterprise_20181101_models.GetDataCorrectSQLFileResponse:
         """
-        This interface applies to: [Common data change](~~58419~~) and [Batch Data import](~~144643~~) .
+        This operation applies to [regular data change](~~58419~~) and [batch data import](~~144643~~).
         
         @param request: GetDataCorrectSQLFileRequest
         @return: GetDataCorrectSQLFileResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_data_correct_sqlfile_with_options(request, runtime)
 
     async def get_data_correct_sqlfile_async(
         self,
         request: dms_enterprise_20181101_models.GetDataCorrectSQLFileRequest,
     ) -> dms_enterprise_20181101_models.GetDataCorrectSQLFileResponse:
         """
-        This interface applies to: [Common data change](~~58419~~) and [Batch Data import](~~144643~~) .
+        This operation applies to [regular data change](~~58419~~) and [batch data import](~~144643~~).
         
         @param request: GetDataCorrectSQLFileRequest
         @return: GetDataCorrectSQLFileResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_data_correct_sqlfile_with_options_async(request, runtime)
 
@@ -5685,14 +5989,92 @@
     async def get_data_export_order_detail_async(
         self,
         request: dms_enterprise_20181101_models.GetDataExportOrderDetailRequest,
     ) -> dms_enterprise_20181101_models.GetDataExportOrderDetailResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_data_export_order_detail_with_options_async(request, runtime)
 
+    def get_data_import_sqlwith_options(
+        self,
+        request: dms_enterprise_20181101_models.GetDataImportSQLRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataImportSQLResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.sql_id):
+            query['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataImportSQL',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataImportSQLResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_data_import_sqlwith_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataImportSQLRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GetDataImportSQLResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.sql_id):
+            query['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetDataImportSQL',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GetDataImportSQLResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_data_import_sql(
+        self,
+        request: dms_enterprise_20181101_models.GetDataImportSQLRequest,
+    ) -> dms_enterprise_20181101_models.GetDataImportSQLResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_data_import_sqlwith_options(request, runtime)
+
+    async def get_data_import_sql_async(
+        self,
+        request: dms_enterprise_20181101_models.GetDataImportSQLRequest,
+    ) -> dms_enterprise_20181101_models.GetDataImportSQLResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_data_import_sqlwith_options_async(request, runtime)
+
     def get_database_with_options(
         self,
         request: dms_enterprise_20181101_models.GetDatabaseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetDatabaseResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6132,14 +6514,21 @@
         return await self.get_logic_database_with_options_async(request, runtime)
 
     def get_meta_table_column_with_options(
         self,
         request: dms_enterprise_20181101_models.GetMetaTableColumnRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetMetaTableColumnResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: GetMetaTableColumnRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMetaTableColumnResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.table_guid):
             query['TableGuid'] = request.table_guid
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
         req = open_api_models.OpenApiRequest(
@@ -6162,14 +6551,21 @@
         )
 
     async def get_meta_table_column_with_options_async(
         self,
         request: dms_enterprise_20181101_models.GetMetaTableColumnRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetMetaTableColumnResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: GetMetaTableColumnRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMetaTableColumnResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.table_guid):
             query['TableGuid'] = request.table_guid
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
         req = open_api_models.OpenApiRequest(
@@ -6191,29 +6587,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_meta_table_column(
         self,
         request: dms_enterprise_20181101_models.GetMetaTableColumnRequest,
     ) -> dms_enterprise_20181101_models.GetMetaTableColumnResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: GetMetaTableColumnRequest
+        @return: GetMetaTableColumnResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_meta_table_column_with_options(request, runtime)
 
     async def get_meta_table_column_async(
         self,
         request: dms_enterprise_20181101_models.GetMetaTableColumnRequest,
     ) -> dms_enterprise_20181101_models.GetMetaTableColumnResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: GetMetaTableColumnRequest
+        @return: GetMetaTableColumnResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_meta_table_column_with_options_async(request, runtime)
 
     def get_meta_table_detail_info_with_options(
         self,
         request: dms_enterprise_20181101_models.GetMetaTableDetailInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetMetaTableDetailInfoResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: GetMetaTableDetailInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMetaTableDetailInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.table_guid):
             query['TableGuid'] = request.table_guid
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
         req = open_api_models.OpenApiRequest(
@@ -6236,14 +6651,21 @@
         )
 
     async def get_meta_table_detail_info_with_options_async(
         self,
         request: dms_enterprise_20181101_models.GetMetaTableDetailInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetMetaTableDetailInfoResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: GetMetaTableDetailInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMetaTableDetailInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.table_guid):
             query['TableGuid'] = request.table_guid
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
         req = open_api_models.OpenApiRequest(
@@ -6265,21 +6687,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_meta_table_detail_info(
         self,
         request: dms_enterprise_20181101_models.GetMetaTableDetailInfoRequest,
     ) -> dms_enterprise_20181101_models.GetMetaTableDetailInfoResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: GetMetaTableDetailInfoRequest
+        @return: GetMetaTableDetailInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_meta_table_detail_info_with_options(request, runtime)
 
     async def get_meta_table_detail_info_async(
         self,
         request: dms_enterprise_20181101_models.GetMetaTableDetailInfoRequest,
     ) -> dms_enterprise_20181101_models.GetMetaTableDetailInfoResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: GetMetaTableDetailInfoRequest
+        @return: GetMetaTableDetailInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_meta_table_detail_info_with_options_async(request, runtime)
 
     def get_online_ddlprogress_with_options(
         self,
         request: dms_enterprise_20181101_models.GetOnlineDDLProgressRequest,
         runtime: util_models.RuntimeOptions,
@@ -6693,15 +7127,15 @@
 
     def get_perm_apply_order_detail_with_options(
         self,
         request: dms_enterprise_20181101_models.GetPermApplyOrderDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetPermApplyOrderDetailResponse:
         """
-        This interface is applicable to obtaining: *Database-permission** , **Table-permissions** , **sensitive column-permission** .
+        You can call this operation to query the information about tickets that apply for permissions on databases, tables, and sensitive columns.
         
         @param request: GetPermApplyOrderDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetPermApplyOrderDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6730,15 +7164,15 @@
 
     async def get_perm_apply_order_detail_with_options_async(
         self,
         request: dms_enterprise_20181101_models.GetPermApplyOrderDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetPermApplyOrderDetailResponse:
         """
-        This interface is applicable to obtaining: *Database-permission** , **Table-permissions** , **sensitive column-permission** .
+        You can call this operation to query the information about tickets that apply for permissions on databases, tables, and sensitive columns.
         
         @param request: GetPermApplyOrderDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GetPermApplyOrderDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6766,28 +7200,28 @@
         )
 
     def get_perm_apply_order_detail(
         self,
         request: dms_enterprise_20181101_models.GetPermApplyOrderDetailRequest,
     ) -> dms_enterprise_20181101_models.GetPermApplyOrderDetailResponse:
         """
-        This interface is applicable to obtaining: *Database-permission** , **Table-permissions** , **sensitive column-permission** .
+        You can call this operation to query the information about tickets that apply for permissions on databases, tables, and sensitive columns.
         
         @param request: GetPermApplyOrderDetailRequest
         @return: GetPermApplyOrderDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.get_perm_apply_order_detail_with_options(request, runtime)
 
     async def get_perm_apply_order_detail_async(
         self,
         request: dms_enterprise_20181101_models.GetPermApplyOrderDetailRequest,
     ) -> dms_enterprise_20181101_models.GetPermApplyOrderDetailResponse:
         """
-        This interface is applicable to obtaining: *Database-permission** , **Table-permissions** , **sensitive column-permission** .
+        You can call this operation to query the information about tickets that apply for permissions on databases, tables, and sensitive columns.
         
         @param request: GetPermApplyOrderDetailRequest
         @return: GetPermApplyOrderDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.get_perm_apply_order_detail_with_options_async(request, runtime)
 
@@ -6868,16 +7302,14 @@
     def get_proxy_with_options(
         self,
         request: dms_enterprise_20181101_models.GetProxyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetProxyResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.instance_id):
-            query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.proxy_id):
             query['ProxyId'] = request.proxy_id
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -6900,16 +7332,14 @@
     async def get_proxy_with_options_async(
         self,
         request: dms_enterprise_20181101_models.GetProxyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GetProxyResponse:
         UtilClient.validate_model(request)
         query = {}
-        if not UtilClient.is_unset(request.instance_id):
-            query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.proxy_id):
             query['ProxyId'] = request.proxy_id
         if not UtilClient.is_unset(request.tid):
             query['Tid'] = request.tid
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -8273,14 +8703,126 @@
     async def get_user_upload_file_job_async(
         self,
         request: dms_enterprise_20181101_models.GetUserUploadFileJobRequest,
     ) -> dms_enterprise_20181101_models.GetUserUploadFileJobResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_user_upload_file_job_with_options_async(request, runtime)
 
+    def grant_template_authority_with_options(
+        self,
+        request: dms_enterprise_20181101_models.GrantTemplateAuthorityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GrantTemplateAuthorityResponse:
+        """
+        You must be a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GrantTemplateAuthorityRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GrantTemplateAuthorityResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.expire_date):
+            query['ExpireDate'] = request.expire_date
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GrantTemplateAuthority',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GrantTemplateAuthorityResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def grant_template_authority_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.GrantTemplateAuthorityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.GrantTemplateAuthorityResponse:
+        """
+        You must be a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GrantTemplateAuthorityRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GrantTemplateAuthorityResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.comment):
+            query['Comment'] = request.comment
+        if not UtilClient.is_unset(request.expire_date):
+            query['ExpireDate'] = request.expire_date
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GrantTemplateAuthority',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.GrantTemplateAuthorityResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def grant_template_authority(
+        self,
+        request: dms_enterprise_20181101_models.GrantTemplateAuthorityRequest,
+    ) -> dms_enterprise_20181101_models.GrantTemplateAuthorityResponse:
+        """
+        You must be a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GrantTemplateAuthorityRequest
+        @return: GrantTemplateAuthorityResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.grant_template_authority_with_options(request, runtime)
+
+    async def grant_template_authority_async(
+        self,
+        request: dms_enterprise_20181101_models.GrantTemplateAuthorityRequest,
+    ) -> dms_enterprise_20181101_models.GrantTemplateAuthorityResponse:
+        """
+        You must be a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: GrantTemplateAuthorityRequest
+        @return: GrantTemplateAuthorityResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.grant_template_authority_with_options_async(request, runtime)
+
     def grant_user_permission_with_options(
         self,
         request: dms_enterprise_20181101_models.GrantUserPermissionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.GrantUserPermissionResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -8528,14 +9070,21 @@
         return await self.list_classification_templates_with_options_async(request, runtime)
 
     def list_columns_with_options(
         self,
         request: dms_enterprise_20181101_models.ListColumnsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.ListColumnsResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: ListColumnsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListColumnsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.logic):
             query['Logic'] = request.logic
         if not UtilClient.is_unset(request.table_id):
             query['TableId'] = request.table_id
         if not UtilClient.is_unset(request.tid):
@@ -8560,14 +9109,21 @@
         )
 
     async def list_columns_with_options_async(
         self,
         request: dms_enterprise_20181101_models.ListColumnsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.ListColumnsResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: ListColumnsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListColumnsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.logic):
             query['Logic'] = request.logic
         if not UtilClient.is_unset(request.table_id):
             query['TableId'] = request.table_id
         if not UtilClient.is_unset(request.tid):
@@ -8591,21 +9147,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_columns(
         self,
         request: dms_enterprise_20181101_models.ListColumnsRequest,
     ) -> dms_enterprise_20181101_models.ListColumnsResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: ListColumnsRequest
+        @return: ListColumnsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_columns_with_options(request, runtime)
 
     async def list_columns_async(
         self,
         request: dms_enterprise_20181101_models.ListColumnsRequest,
     ) -> dms_enterprise_20181101_models.ListColumnsResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: ListColumnsRequest
+        @return: ListColumnsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_columns_with_options_async(request, runtime)
 
     def list_dagversions_with_options(
         self,
         request: dms_enterprise_20181101_models.ListDAGVersionsRequest,
         runtime: util_models.RuntimeOptions,
@@ -9141,14 +9709,178 @@
         
         @param request: ListDataCorrectPreCheckSQLRequest
         @return: ListDataCorrectPreCheckSQLResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_data_correct_pre_check_sqlwith_options_async(request, runtime)
 
+    def list_data_import_sqlpre_check_detail_with_options(
+        self,
+        request: dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.page_numer):
+            query['PageNumer'] = request.page_numer
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.sql_type):
+            query['SqlType'] = request.sql_type
+        if not UtilClient.is_unset(request.status_code):
+            query['StatusCode'] = request.status_code
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDataImportSQLPreCheckDetail',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_data_import_sqlpre_check_detail_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.page_numer):
+            query['PageNumer'] = request.page_numer
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.sql_type):
+            query['SqlType'] = request.sql_type
+        if not UtilClient.is_unset(request.status_code):
+            query['StatusCode'] = request.status_code
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDataImportSQLPreCheckDetail',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_data_import_sqlpre_check_detail(
+        self,
+        request: dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailRequest,
+    ) -> dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_data_import_sqlpre_check_detail_with_options(request, runtime)
+
+    async def list_data_import_sqlpre_check_detail_async(
+        self,
+        request: dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailRequest,
+    ) -> dms_enterprise_20181101_models.ListDataImportSQLPreCheckDetailResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_data_import_sqlpre_check_detail_with_options_async(request, runtime)
+
+    def list_data_import_sqltype_with_options(
+        self,
+        request: dms_enterprise_20181101_models.ListDataImportSQLTypeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.ListDataImportSQLTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDataImportSQLType',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.ListDataImportSQLTypeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_data_import_sqltype_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.ListDataImportSQLTypeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.ListDataImportSQLTypeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.order_id):
+            query['OrderId'] = request.order_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListDataImportSQLType',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.ListDataImportSQLTypeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_data_import_sqltype(
+        self,
+        request: dms_enterprise_20181101_models.ListDataImportSQLTypeRequest,
+    ) -> dms_enterprise_20181101_models.ListDataImportSQLTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_data_import_sqltype_with_options(request, runtime)
+
+    async def list_data_import_sqltype_async(
+        self,
+        request: dms_enterprise_20181101_models.ListDataImportSQLTypeRequest,
+    ) -> dms_enterprise_20181101_models.ListDataImportSQLTypeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_data_import_sqltype_with_options_async(request, runtime)
+
     def list_database_user_permssions_with_options(
         self,
         request: dms_enterprise_20181101_models.ListDatabaseUserPermssionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.ListDatabaseUserPermssionsResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -11348,14 +12080,21 @@
         return await self.list_standard_groups_with_options_async(request, runtime)
 
     def list_tables_with_options(
         self,
         request: dms_enterprise_20181101_models.ListTablesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.ListTablesResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: ListTablesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTablesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.database_id):
             query['DatabaseId'] = request.database_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -11386,14 +12125,21 @@
         )
 
     async def list_tables_with_options_async(
         self,
         request: dms_enterprise_20181101_models.ListTablesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.ListTablesResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: ListTablesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTablesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.database_id):
             query['DatabaseId'] = request.database_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -11423,21 +12169,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_tables(
         self,
         request: dms_enterprise_20181101_models.ListTablesRequest,
     ) -> dms_enterprise_20181101_models.ListTablesResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: ListTablesRequest
+        @return: ListTablesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_tables_with_options(request, runtime)
 
     async def list_tables_async(
         self,
         request: dms_enterprise_20181101_models.ListTablesRequest,
     ) -> dms_enterprise_20181101_models.ListTablesResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: ListTablesRequest
+        @return: ListTablesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_tables_with_options_async(request, runtime)
 
     def list_task_flow_with_options(
         self,
         request: dms_enterprise_20181101_models.ListTaskFlowRequest,
         runtime: util_models.RuntimeOptions,
@@ -13869,14 +14627,118 @@
     async def retry_data_correct_pre_check_async(
         self,
         request: dms_enterprise_20181101_models.RetryDataCorrectPreCheckRequest,
     ) -> dms_enterprise_20181101_models.RetryDataCorrectPreCheckResponse:
         runtime = util_models.RuntimeOptions()
         return await self.retry_data_correct_pre_check_with_options_async(request, runtime)
 
+    def revoke_template_authority_with_options(
+        self,
+        request: dms_enterprise_20181101_models.RevokeTemplateAuthorityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.RevokeTemplateAuthorityResponse:
+        """
+        You must be a database administrator (DBA) or a DMS administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: RevokeTemplateAuthorityRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokeTemplateAuthorityResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RevokeTemplateAuthority',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.RevokeTemplateAuthorityResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def revoke_template_authority_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.RevokeTemplateAuthorityRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.RevokeTemplateAuthorityResponse:
+        """
+        You must be a database administrator (DBA) or a DMS administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: RevokeTemplateAuthorityRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokeTemplateAuthorityResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        if not UtilClient.is_unset(request.user_ids):
+            query['UserIds'] = request.user_ids
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='RevokeTemplateAuthority',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.RevokeTemplateAuthorityResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def revoke_template_authority(
+        self,
+        request: dms_enterprise_20181101_models.RevokeTemplateAuthorityRequest,
+    ) -> dms_enterprise_20181101_models.RevokeTemplateAuthorityResponse:
+        """
+        You must be a database administrator (DBA) or a DMS administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: RevokeTemplateAuthorityRequest
+        @return: RevokeTemplateAuthorityResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.revoke_template_authority_with_options(request, runtime)
+
+    async def revoke_template_authority_async(
+        self,
+        request: dms_enterprise_20181101_models.RevokeTemplateAuthorityRequest,
+    ) -> dms_enterprise_20181101_models.RevokeTemplateAuthorityResponse:
+        """
+        You must be a database administrator (DBA) or a DMS administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: RevokeTemplateAuthorityRequest
+        @return: RevokeTemplateAuthorityResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.revoke_template_authority_with_options_async(request, runtime)
+
     def revoke_user_permission_with_options(
         self,
         request: dms_enterprise_20181101_models.RevokeUserPermissionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.RevokeUserPermissionResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -14078,14 +14940,21 @@
         return await self.search_database_with_options_async(request, runtime)
 
     def search_table_with_options(
         self,
         request: dms_enterprise_20181101_models.SearchTableRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.SearchTableResponse:
+        """
+        You can call this operation only for database instances that are managed in Security Collaboration mode.
+        
+        @param request: SearchTableRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SearchTableResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.db_type):
             query['DbType'] = request.db_type
         if not UtilClient.is_unset(request.env_type):
             query['EnvType'] = request.env_type
         if not UtilClient.is_unset(request.page_number):
@@ -14122,14 +14991,21 @@
         )
 
     async def search_table_with_options_async(
         self,
         request: dms_enterprise_20181101_models.SearchTableRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.SearchTableResponse:
+        """
+        You can call this operation only for database instances that are managed in Security Collaboration mode.
+        
+        @param request: SearchTableRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SearchTableResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.db_type):
             query['DbType'] = request.db_type
         if not UtilClient.is_unset(request.env_type):
             query['EnvType'] = request.env_type
         if not UtilClient.is_unset(request.page_number):
@@ -14165,21 +15041,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def search_table(
         self,
         request: dms_enterprise_20181101_models.SearchTableRequest,
     ) -> dms_enterprise_20181101_models.SearchTableResponse:
+        """
+        You can call this operation only for database instances that are managed in Security Collaboration mode.
+        
+        @param request: SearchTableRequest
+        @return: SearchTableResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.search_table_with_options(request, runtime)
 
     async def search_table_async(
         self,
         request: dms_enterprise_20181101_models.SearchTableRequest,
     ) -> dms_enterprise_20181101_models.SearchTableResponse:
+        """
+        You can call this operation only for database instances that are managed in Security Collaboration mode.
+        
+        @param request: SearchTableRequest
+        @return: SearchTableResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.search_table_with_options_async(request, runtime)
 
     def set_owners_with_options(
         self,
         request: dms_enterprise_20181101_models.SetOwnersRequest,
         runtime: util_models.RuntimeOptions,
@@ -14644,14 +15532,21 @@
         return await self.sync_database_meta_with_options_async(request, runtime)
 
     def sync_instance_meta_with_options(
         self,
         request: dms_enterprise_20181101_models.SyncInstanceMetaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.SyncInstanceMetaResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: SyncInstanceMetaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SyncInstanceMetaResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ignore_table):
             query['IgnoreTable'] = request.ignore_table
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.tid):
@@ -14676,14 +15571,21 @@
         )
 
     async def sync_instance_meta_with_options_async(
         self,
         request: dms_enterprise_20181101_models.SyncInstanceMetaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.SyncInstanceMetaResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: SyncInstanceMetaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SyncInstanceMetaResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ignore_table):
             query['IgnoreTable'] = request.ignore_table
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.tid):
@@ -14707,24 +15609,144 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def sync_instance_meta(
         self,
         request: dms_enterprise_20181101_models.SyncInstanceMetaRequest,
     ) -> dms_enterprise_20181101_models.SyncInstanceMetaResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: SyncInstanceMetaRequest
+        @return: SyncInstanceMetaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.sync_instance_meta_with_options(request, runtime)
 
     async def sync_instance_meta_async(
         self,
         request: dms_enterprise_20181101_models.SyncInstanceMetaRequest,
     ) -> dms_enterprise_20181101_models.SyncInstanceMetaResponse:
+        """
+        You can call this operation only for database instances whose control mode is Security Collaboration.
+        
+        @param request: SyncInstanceMetaRequest
+        @return: SyncInstanceMetaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.sync_instance_meta_with_options_async(request, runtime)
 
+    def update_authority_template_with_options(
+        self,
+        request: dms_enterprise_20181101_models.UpdateAuthorityTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.UpdateAuthorityTemplateResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: UpdateAuthorityTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAuthorityTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateAuthorityTemplate',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.UpdateAuthorityTemplateResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def update_authority_template_with_options_async(
+        self,
+        request: dms_enterprise_20181101_models.UpdateAuthorityTemplateRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dms_enterprise_20181101_models.UpdateAuthorityTemplateResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: UpdateAuthorityTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAuthorityTemplateResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.description):
+            query['Description'] = request.description
+        if not UtilClient.is_unset(request.name):
+            query['Name'] = request.name
+        if not UtilClient.is_unset(request.template_id):
+            query['TemplateId'] = request.template_id
+        if not UtilClient.is_unset(request.tid):
+            query['Tid'] = request.tid
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='UpdateAuthorityTemplate',
+            version='2018-11-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dms_enterprise_20181101_models.UpdateAuthorityTemplateResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def update_authority_template(
+        self,
+        request: dms_enterprise_20181101_models.UpdateAuthorityTemplateRequest,
+    ) -> dms_enterprise_20181101_models.UpdateAuthorityTemplateResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: UpdateAuthorityTemplateRequest
+        @return: UpdateAuthorityTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.update_authority_template_with_options(request, runtime)
+
+    async def update_authority_template_async(
+        self,
+        request: dms_enterprise_20181101_models.UpdateAuthorityTemplateRequest,
+    ) -> dms_enterprise_20181101_models.UpdateAuthorityTemplateResponse:
+        """
+        You are a database administrator (DBA) or a Data Management (DMS) administrator. For more information about how to view system roles, see [View system roles](~~324212~~).
+        
+        @param request: UpdateAuthorityTemplateRequest
+        @return: UpdateAuthorityTemplateResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.update_authority_template_with_options_async(request, runtime)
+
     def update_instance_with_options(
         self,
         request: dms_enterprise_20181101_models.UpdateInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dms_enterprise_20181101_models.UpdateInstanceResponse:
         """
         Before you call the UpdateInstance operation, call the [GetInstance](~~141567~~) or [ListInstances](~~141936~~) operation to obtain the complete information about the instance.
```

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101/models.py` & `alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -2037,45 +2037,45 @@
         db_id: int = None,
         is_logic: bool = None,
         new_level: str = None,
         schema_name: str = None,
         table_name: str = None,
         tid: int = None,
     ):
-        # The name of the field. You can call the [ListSensitiveColumns](~~188103~~) operation to query the name of the field.
+        # The name of the field. You can call the [ListSensitiveColumns](~~188103~~) operation to obtain the name of the field.
         # 
-        # >  You can also call the [ListColumns](~~141870~~) operation to query the name of the field.
+        # > You can also call the [ListColumns](~~141870~~) operation to obtain the name of the field.
         self.column_name = column_name
-        # The ID of the database. You can call the [SearchDatabase](~~141876~~) operation to query the ID of the database.
+        # The ID of the database. You can call the [SearchDatabase](~~141876~~) operation to obtain the ID of the database.
         # 
-        # >  You can also call the [ListDatabases](~~141873~~) operation to query the ID of a physical database and the [ListLogicDatabases](~~141874~~) operation to query the ID of a logical database.
+        # > You can also call the [ListDatabases](~~141873~~) operation to obtain the ID of a physical database and the [ListLogicDatabases](~~141874~~) operation to obtain the ID of a logical database.
         self.db_id = db_id
         # Specifies whether the database is a logical database. Valid values:
         # 
         # *   true: The database is a physical database.
         # *   false: The database is a logical database.
         self.is_logic = is_logic
         # The new sensitivity level of the field that you want to specify. Valid values:
         # 
         # *   INNER: low sensitivity level
         # *   SENSITIVE: medium sensitivity level
         # *   CONFIDENTIAL: high sensitivity level
         self.new_level = new_level
-        # The name of the database. You can call the [ListSensitiveColumns](~~188103~~) operation to query the name of the database.
+        # The name of the database. You can call the [ListSensitiveColumns](~~188103~~) operation to obtain the name of the database.
         # 
-        # *   You can also call the [SearchDatabase](~~141876~~) operation to query the name of the database.
-        # *   You can also call the [ListDatabases](~~141873~~) operation to query the name of a physical database and the [ListLogicDatabases](~~141874~~) operation to query the name of a logical database.
+        # *   You can also call the [SearchDatabase](~~141876~~) operation to obtain the name of the database.
+        # *   You can also call the [ListDatabases](~~141873~~) operation to obtain the name of a physical database and the [ListLogicDatabases](~~141874~~) operation to obtain the name of a logical database.
         self.schema_name = schema_name
-        # The name of the table. You can call the [ListSensitiveColumns](~~188103~~) operation to query the name of the table.
+        # The name of the table. You can call the [ListSensitiveColumns](~~188103~~) operation to obtain the name of the table.
         # 
-        # >  You can also call the [ListTables](~~141878~~) operation to query the name of the table.
+        # > You can also call the [ListTables](~~141878~~) operation to obtain the name of the table.
         self.table_name = table_name
         # The ID of the tenant.
         # 
-        # >  To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](~~181330~~) topic.
+        # > To view the ID of the tenant, go to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [View information about the current tenant](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2122,24 +2122,24 @@
     def __init__(
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
-        # The error code.
+        # The error code returned if the request failed.
         self.error_code = error_code
-        # The error message.
+        # The error message returned if the request failed.
         self.error_message = error_message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful. Valid values:
+        # Indicates whether the request was successful. Valid values:
         # 
-        # *   true: The request is successful.
-        # *   false: The request fails.
+        # *   true: The request was successful.
+        # *   false: The request failed.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2355,16 +2355,21 @@
 class CloseOrderRequest(TeaModel):
     def __init__(
         self,
         close_reason: str = None,
         order_id: int = None,
         tid: int = None,
     ):
+        # The reason why the ticket is closed.
         self.close_reason = close_reason
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2395,17 +2400,21 @@
     def __init__(
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2476,14 +2485,217 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CloseOrderResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateAuthorityTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        name: str = None,
+        tid: int = None,
+    ):
+        # The description of the permission template.
+        self.description = description
+        # The name of the permission template.
+        self.name = name
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
+        self.tid = tid
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
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class CreateAuthorityTemplateResponseBodyAuthorityTemplateView(TeaModel):
+    def __init__(
+        self,
+        create_time: str = None,
+        creator_id: int = None,
+        description: str = None,
+        name: str = None,
+        template_id: int = None,
+    ):
+        # The time when the permission template was created. The time is in the yyyy-MM-DD HH:mm:ss format.
+        self.create_time = create_time
+        # The ID of the user who created the permission template.
+        self.creator_id = creator_id
+        # The description of the permission template.
+        self.description = description
+        # The name of the permission template.
+        self.name = name
+        # The ID of the permission template.
+        self.template_id = template_id
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
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.creator_id is not None:
+            result['CreatorId'] = self.creator_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('CreatorId') is not None:
+            self.creator_id = m.get('CreatorId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class CreateAuthorityTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        authority_template_view: CreateAuthorityTemplateResponseBodyAuthorityTemplateView = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        # The details of the permission template.
+        self.authority_template_view = authority_template_view
+        # The error code.
+        self.error_code = error_code
+        # The error message.
+        self.error_message = error_message
+        # The ID of the request.
+        self.request_id = request_id
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
+        self.success = success
+
+    def validate(self):
+        if self.authority_template_view:
+            self.authority_template_view.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.authority_template_view is not None:
+            result['AuthorityTemplateView'] = self.authority_template_view.to_map()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthorityTemplateView') is not None:
+            temp_model = CreateAuthorityTemplateResponseBodyAuthorityTemplateView()
+            self.authority_template_view = temp_model.from_map(m['AuthorityTemplateView'])
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class CreateAuthorityTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateAuthorityTemplateResponseBody = None,
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
+            temp_model = CreateAuthorityTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateDataCorrectOrderRequestParamDbItemList(TeaModel):
     def __init__(
         self,
         db_id: int = None,
         logic: bool = None,
     ):
         # The ID of the database. The database can be a physical database or a logical database.
@@ -4985,19 +5197,32 @@
         db_id: int = None,
         logic: bool = None,
         order_id: int = None,
         plan_time: str = None,
         publish_strategy: str = None,
         tid: int = None,
     ):
+        # The ID of the database for which the schema design is executed.
         self.db_id = db_id
+        # Indicates whether the database is a logical database.
         self.logic = logic
+        # The ID of the ticket.
+        # 
+        # > : You can create a schema design ticket in the DMS console. For more information, see [Design schemas](~~69711~~). You can also create a schema design ticket by calling the [CreateOrder](~~144649~~) operation and obtain the ticket ID.
         self.order_id = order_id
+        # The time to execute the schema design ticket.
         self.plan_time = plan_time
+        # The policy to execute the schema design ticket. Valid values:
+        # 
+        # *   IMMEDIATELY: immediately executes the schema design ticket.
+        # *   REGULARLY: executes the schema design ticket at a scheduled time.
         self.publish_strategy = publish_strategy
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5041,18 +5266,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         task_id: int = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
+        # The ID of the job.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5134,16 +5364,21 @@
 class CreateSQLReviewOrderRequestParam(TeaModel):
     def __init__(
         self,
         attachment_key_list: List[str] = None,
         db_id: int = None,
         project_name: str = None,
     ):
+        # The files to be reviewed. Multiple files can be reviewed at a time.
         self.attachment_key_list = attachment_key_list
+        # The ID of the database. You can call the [SearchDatabases](~~141876~~) operation to query the ID of the database.
+        # 
+        # >  You can call this operation to query only physical databases. This operation is unavailable to query logical databases.
         self.db_id = db_id
+        # The name of the project.
         self.project_name = project_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5174,17 +5409,21 @@
     def __init__(
         self,
         comment: str = None,
         param: CreateSQLReviewOrderRequestParam = None,
         related_user_list: List[int] = None,
         tid: int = None,
     ):
+        # The purpose or objective of the SQL review. This reduces unnecessary communication.
         self.comment = comment
+        # The parameters of the ticket.
         self.param = param
+        # The stakeholders involved in this operation. All the specified stakeholders can view the ticket details and take part in the approval process. Irrelevant users other than DMS administrators and database administrators (DBAs) are not allowed to view the ticket details.
         self.related_user_list = related_user_list
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to obtain the tenant ID.
         self.tid = tid
 
     def validate(self):
         if self.param:
             self.param.validate()
 
     def to_map(self):
@@ -5221,17 +5460,21 @@
     def __init__(
         self,
         comment: str = None,
         param_shrink: str = None,
         related_user_list_shrink: str = None,
         tid: int = None,
     ):
+        # The purpose or objective of the SQL review. This reduces unnecessary communication.
         self.comment = comment
+        # The parameters of the ticket.
         self.param_shrink = param_shrink
+        # The stakeholders involved in this operation. All the specified stakeholders can view the ticket details and take part in the approval process. Irrelevant users other than DMS administrators and database administrators (DBAs) are not allowed to view the ticket details.
         self.related_user_list_shrink = related_user_list_shrink
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to obtain the tenant ID.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5267,18 +5510,23 @@
         self,
         create_order_result: List[int] = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The result of the ticket creation task.
         self.create_order_result = create_order_result
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5722,17 +5970,24 @@
     def __init__(
         self,
         db_id: int = None,
         db_search_name: str = None,
         logic: bool = None,
         version_id: str = None,
     ):
+        # The ID of the database. You can call the [SearchDatabases](~~141876~~) operation to query the ID of the database.
         self.db_id = db_id
+        # The name that is used to search for the database. You can call the [SearchDatabases](~~141876~~) operation to query the name of the database.
         self.db_search_name = db_search_name
+        # Specifies whether the database is a logical database. Valid values:
+        # 
+        # *   **true**: The database is a logical database.
+        # *   **false**: The database is not a logical database.
         self.logic = logic
+        # The version number of the schema. The default value is the latest schema version number. For more information, see [Manage schema versions](~~202275~~).
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5765,15 +6020,17 @@
 
 class CreateStructSyncOrderRequestParamTableInfoList(TeaModel):
     def __init__(
         self,
         source_table_name: str = None,
         target_table_name: str = None,
     ):
+        # The name of the source table.
         self.source_table_name = source_table_name
+        # The name of the destination table.
         self.target_table_name = target_table_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5800,17 +6057,26 @@
     def __init__(
         self,
         db_id: int = None,
         db_search_name: str = None,
         logic: bool = None,
         version_id: str = None,
     ):
+        # The ID of the database. You can call the [SearchDatabases](~~141876~~) operation to query the ID of the database.
         self.db_id = db_id
+        # The name that is used to search for the database. You can call the [SearchDatabases](~~141876~~) operation to query the name of the database.
         self.db_search_name = db_search_name
+        # Specifies whether the database is a logical database. Valid values:
+        # 
+        # *   **true**: The database is a logical database.
+        # *   **false**: The database is not a logical database.
         self.logic = logic
+        # The version number. By default, this parameter is left empty.
+        # 
+        # >  If you specify the schema version number of the destination database, Data Management (DMS) only compares the schemas of the two databases.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5845,17 +6111,24 @@
     def __init__(
         self,
         ignore_error: bool = None,
         source: CreateStructSyncOrderRequestParamSource = None,
         table_info_list: List[CreateStructSyncOrderRequestParamTableInfoList] = None,
         target: CreateStructSyncOrderRequestParamTarget = None,
     ):
+        # Specifies whether to skip an error that occurs in executing an SQL statement. Valid values:
+        # 
+        # *   **true**: continues to execute subsequent SQL statements if an error occurs in executing an SQL statement.
+        # *   **false**: stops executing subsequent SQL statements if an error occurs in executing an SQL statement.
         self.ignore_error = ignore_error
+        # The information about the base database.
         self.source = source
+        # The information about the table of which you want to synchronize the schema.
         self.table_info_list = table_info_list
+        # The information about the database to which you want to synchronize the schema of a table.
         self.target = target
 
     def validate(self):
         if self.source:
             self.source.validate()
         if self.table_info_list:
             for k in self.table_info_list:
@@ -5905,18 +6178,25 @@
         self,
         attachment_key: str = None,
         comment: str = None,
         param: CreateStructSyncOrderRequestParam = None,
         related_user_list: List[int] = None,
         tid: int = None,
     ):
+        # The key of an attachment that is returned after the attachment is uploaded. You can call the [GetUserUploadFileJob](~~206069~~) operation to query the key of the attachment.
         self.attachment_key = attachment_key
+        # The remarks of the ticket.
         self.comment = comment
+        # The parameters of the ticket.
         self.param = param
+        # The IDs of the stakeholders.
         self.related_user_list = related_user_list
+        # The ID of the tenant.
+        # 
+        # >  To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the DMS console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         if self.param:
             self.param.validate()
 
     def to_map(self):
@@ -5958,18 +6238,25 @@
         self,
         attachment_key: str = None,
         comment: str = None,
         param_shrink: str = None,
         related_user_list_shrink: str = None,
         tid: int = None,
     ):
+        # The key of an attachment that is returned after the attachment is uploaded. You can call the [GetUserUploadFileJob](~~206069~~) operation to query the key of the attachment.
         self.attachment_key = attachment_key
+        # The remarks of the ticket.
         self.comment = comment
+        # The parameters of the ticket.
         self.param_shrink = param_shrink
+        # The IDs of the stakeholders.
         self.related_user_list_shrink = related_user_list_shrink
+        # The ID of the tenant.
+        # 
+        # >  To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the DMS console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6009,18 +6296,23 @@
         self,
         create_order_result: List[int] = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The result of creating the ticket.
         self.create_order_result = create_order_result
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6109,29 +6401,29 @@
         node_output: str = None,
         node_type: str = None,
         tid: int = None,
         time_variables: str = None,
     ):
         # The ID of the task flow. You can call the [ListTaskFlow](~~424565~~) or [ListLhTaskFlowAndScenario](~~426672~~) operation to query the task flow ID.
         self.dag_id = dag_id
-        # The position of the node on the Directed Acyclic Graph (DAG).
+        # The position of the node on the directed acyclic graph (DAG).
         self.graph_param = graph_param
-        # The configuration for the node.
+        # The configuration of the node.
         self.node_content = node_content
-        # The name of the node you want to create.
+        # The name of the node that you want to create.
         self.node_name = node_name
         # The output variables for the task.
         self.node_output = node_output
-        # The type of the node you want to create. For more information about the valid values for this parameter, see [NodeType parameter](~~424705~~).
+        # The type of the node that you want to create. For more information about the valid values for this parameter, see [NodeType parameter](~~424705~~).
         self.node_type = node_type
         # The ID of the tenant.
         # 
-        # > To view the ID of the tenant, go to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [View information about the current tenant](~~181330~~).
+        # > To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the [View information about the current tenant](~~181330~~) section of the "Manage DMS tenants" topic.
         self.tid = tid
-        # The time variables configured for the node.
+        # The time variables for the node.
         self.time_variables = time_variables
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6183,19 +6475,19 @@
         self,
         error_code: str = None,
         error_message: str = None,
         node_id: int = None,
         request_id: str = None,
         success: bool = None,
     ):
-        # The error code returned if the request failed.
+        # The error code returned.
         self.error_code = error_code
-        # The error message returned if the request failed.
+        # The error message returned if the request fails.
         self.error_message = error_message
-        # The ID of the task node returned when the task was created.
+        # The ID of the task node returned if the node is created.
         self.node_id = node_id
         # The ID of the request. You can use the ID to query logs and troubleshoot issues.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
         # *   true: The request was successful.
         # *   false: The request failed.
@@ -6601,16 +6893,19 @@
 class CreateUploadOSSFileJobRequestUploadTarget(TeaModel):
     def __init__(
         self,
         bucket_name: str = None,
         endpoint: str = None,
         object_name: str = None,
     ):
+        # The name of the OSS bucket.
         self.bucket_name = bucket_name
+        # The endpoint of the OSS bucket.
         self.endpoint = endpoint
+        # The name of the OSS object.
         self.object_name = object_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6641,17 +6936,30 @@
     def __init__(
         self,
         file_name: str = None,
         file_source: str = None,
         tid: int = None,
         upload_target: CreateUploadOSSFileJobRequestUploadTarget = None,
     ):
+        # The name of the file.
+        # 
+        # > The file name must end with .txt or .sql. For example, the file name can be text.txt.
         self.file_name = file_name
+        # The purpose of the file upload task. Valid values:
+        # 
+        # *   **datacorrect**: The file is uploaded to change data.
+        # *   **order_info_attachment**: The file is uploaded as an attachment in a ticket.
+        # *   **big-file**: The file is uploaded to import multiple data records at a time.
+        # *   **sqlreview**: The file is uploaded for SQL review.
         self.file_source = file_source
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](~~181330~~) topic.
         self.tid = tid
+        # The information about the OSS file to be uploaded.
         self.upload_target = upload_target
 
     def validate(self):
         if self.upload_target:
             self.upload_target.validate()
 
     def to_map(self):
@@ -6688,17 +6996,30 @@
     def __init__(
         self,
         file_name: str = None,
         file_source: str = None,
         tid: int = None,
         upload_target_shrink: str = None,
     ):
+        # The name of the file.
+        # 
+        # > The file name must end with .txt or .sql. For example, the file name can be text.txt.
         self.file_name = file_name
+        # The purpose of the file upload task. Valid values:
+        # 
+        # *   **datacorrect**: The file is uploaded to change data.
+        # *   **order_info_attachment**: The file is uploaded as an attachment in a ticket.
+        # *   **big-file**: The file is uploaded to import multiple data records at a time.
+        # *   **sqlreview**: The file is uploaded for SQL review.
         self.file_source = file_source
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](~~181330~~) topic.
         self.tid = tid
+        # The information about the OSS file to be uploaded.
         self.upload_target_shrink = upload_target_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6734,18 +7055,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         job_key: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The key of the file upload task. You can query the upload progress and task details. For more information, see [GetUserUploadFileJob](~~206069~~).
         self.job_key = job_key
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8519,14 +8845,15 @@
 
 class DisableUserRequest(TeaModel):
     def __init__(
         self,
         tid: int = None,
         uid: str = None,
     ):
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to obtain the tenant ID.
         self.tid = tid
         # The UID of the Alibaba Cloud account.
         self.uid = uid
 
     def validate(self):
         pass
 
@@ -9187,16 +9514,28 @@
 class ExecuteDataExportRequest(TeaModel):
     def __init__(
         self,
         action_detail: Dict[str, Any] = None,
         order_id: int = None,
         tid: int = None,
     ):
+        # The parameters that are required to perform the operation:
+        # 
+        # ```json
+        # {
+        #    "fileType": "CSV", // The format of the exported file.
+        #    "encoding": "" // The encoding format.
+        #  }
+        # ```
         self.action_detail = action_detail
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9226,16 +9565,28 @@
 class ExecuteDataExportShrinkRequest(TeaModel):
     def __init__(
         self,
         action_detail_shrink: str = None,
         order_id: int = None,
         tid: int = None,
     ):
+        # The parameters that are required to perform the operation:
+        # 
+        # ```json
+        # {
+        #    "fileType": "CSV", // The format of the exported file.
+        #    "encoding": "" // The encoding format.
+        #  }
+        # ```
         self.action_detail_shrink = action_detail_shrink
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9266,17 +9617,21 @@
     def __init__(
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9570,15 +9925,19 @@
 
 class ExecuteStructSyncRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9605,17 +9964,21 @@
     def __init__(
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9692,17 +10055,17 @@
 
 class GetApprovalDetailRequest(TeaModel):
     def __init__(
         self,
         tid: int = None,
         workflow_instance_id: int = None,
     ):
-        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to query the tenant ID.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to obtain the tenant ID.
         self.tid = tid
-        # The ID of the approval process. You can call the [GetOrderBaseInfo](~~144642~~) operation to query the ID of the approval process.
+        # The ID of the approval process. You can call the [GetOrderBaseInfo](~~144642~~) operation to obtain the ID of the approval process.
         self.workflow_instance_id = workflow_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9867,15 +10230,17 @@
         self.operate_comment = operate_comment
         # The time when the ticket was submitted.
         self.operate_time = operate_time
         # The ID of the user who submitted the ticket.
         self.operator_id = operator_id
         # The approval status of the ticket. Valid values:
         # 
-        # *   **AUDITING**: The ticket is being processed.
+        # *   **START**: The ticket was submitted.
+        # *   **ERROR**: An error occurred.
+        # *   **AUDITING**: The ticket is being reviewed.
         # *   **REJECT**: The ticket was rejected.
         # *   **CANCEL**: The ticket was revoked.
         # *   **APPROVED**: The ticket was approved.
         self.workflow_ins_code = workflow_ins_code
 
     def validate(self):
         if self.audit_user_id_list:
@@ -9977,37 +10342,37 @@
         self.current_handlers = current_handlers
         # The description of the approval process.
         self.description = description
         # The ID of the ticket.
         self.order_id = order_id
         # The type of the ticket. Valid values:
         # 
-        # - **NDDL**: The ticket is used to change the schema design.
-        # - **DATA_TRACK**: The ticket is used to track data.
-        # - **TABLE_SYNC**: The ticket is used to synchronize databases and tables.
-        # - **PERM_APPLY**: The ticket is used to apply for permissions.
-        # - **DATA_EXPORT**: The ticket is used to export data.
-        # - **DATA_CORRECT**: The ticket is used to change data.
-        # - **OWNER_APPLY**: The ticket is used to apply for the owner role of a resource.
-        # - **SENSITIVITY**: The ticket is used to change column sensitivity levels.
+        # *   **NDDL**: a schema design ticket
+        # *   **DATA_TRACK**: a data tracking ticket
+        # *   **TABLE_SYNC**: a table synchronization ticket
+        # *   **PERM_APPLY**: a permission application ticket
+        # *   **DATA_EXPORT**: a data export ticket
+        # *   **DATA_CORRECT**: a data change ticket
+        # *   **OWNER_APPLY**: an owner role application ticket
+        # *   **SENSITIVITY**: a column sensitivity level change ticket
         self.order_type = order_type
-        # The reason for the approval.
+        # The reasons for the approval.
         self.reason_list = reason_list
-        # The ID of the approval template.
+        # The ID of the workflow template.
         self.template_id = template_id
         # The title of the approval process.
         self.title = title
         # The approval status of the ticket. Valid values:
         # 
-        # - **AUDITING**: The ticket is being processed.
-        # - **REJECT**: The ticket was rejected.
-        # - **CANCEL**: The ticket was revoked.
-        # - **APPROVED**: The ticket was approved.
+        # *   **AUDITING**: The ticket is being reviewed.
+        # *   **REJECT**: The ticket was rejected.
+        # *   **CANCEL**: The ticket was revoked.
+        # *   **APPROVED**: The ticket was approved.
         # 
-        # >  If an approval process contains multiple approval nodes, this parameter is returned for each approval node.
+        # > An approval process contains multiple approval nodes, and this parameter is returned for each approval node.
         self.workflow_ins_code = workflow_ins_code
         # The details of approval nodes.
         self.workflow_nodes = workflow_nodes
 
     def validate(self):
         if self.current_handlers:
             self.current_handlers.validate()
@@ -10083,24 +10448,24 @@
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
         # The approval details of the ticket.
         self.approval_detail = approval_detail
-        # The error code returned if the request fails.
+        # The error code returned if the request failed.
         self.error_code = error_code
-        # The error message returned if the request fails.
+        # The error message returned if the request failed.
         self.error_message = error_message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request was successful. Valid values:
+        # Indicates whether the request is successful. Valid values:
         # 
-        # - **true**: The request was successful.
-        # - **false**: The request failed.
+        # *   **true**: The request is successful.
+        # *   **false**: The request fails.
         self.success = success
 
     def validate(self):
         if self.approval_detail:
             self.approval_detail.validate()
 
     def to_map(self):
@@ -10177,14 +10542,595 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetApprovalDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetAuthorityTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        template_id: int = None,
+        tid: int = None,
+    ):
+        # The ID of the permission template.
+        self.template_id = template_id
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
+        self.tid = tid
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
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetAuthorityTemplateResponseBodyAuthorityTemplateViewAuthorityTemplateItemListAuthorityTemplateItem(TeaModel):
+    def __init__(
+        self,
+        attribute: str = None,
+        db_id: int = None,
+        instance_id: int = None,
+        item_id: int = None,
+        modifier_id: int = None,
+        resource_type: str = None,
+        table_name: str = None,
+        template_id: int = None,
+    ):
+        # Other information. For example, you can add the logon permission on an instance to the permission template.
+        self.attribute = attribute
+        # The ID of the database.
+        self.db_id = db_id
+        # The ID of the instance.
+        self.instance_id = instance_id
+        # The ID of the resource.
+        self.item_id = item_id
+        # The ID of the user who modified the resource.
+        self.modifier_id = modifier_id
+        # The type of the resource. Valid values:
+        # 
+        # *   **INSTANCE**: instance
+        # *   **LOGIC_DB**: logical database
+        # *   **META_DB**: physical database
+        # *   **LOGIC_TABLE**: logical table
+        # *   **SINGLE_TABLE**: physical table
+        self.resource_type = resource_type
+        # The name of the table.
+        self.table_name = table_name
+        # The ID of the permission template.
+        self.template_id = template_id
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
+        if self.attribute is not None:
+            result['Attribute'] = self.attribute
+        if self.db_id is not None:
+            result['DbId'] = self.db_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.item_id is not None:
+            result['ItemId'] = self.item_id
+        if self.modifier_id is not None:
+            result['ModifierId'] = self.modifier_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.table_name is not None:
+            result['TableName'] = self.table_name
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Attribute') is not None:
+            self.attribute = m.get('Attribute')
+        if m.get('DbId') is not None:
+            self.db_id = m.get('DbId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('ItemId') is not None:
+            self.item_id = m.get('ItemId')
+        if m.get('ModifierId') is not None:
+            self.modifier_id = m.get('ModifierId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TableName') is not None:
+            self.table_name = m.get('TableName')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class GetAuthorityTemplateResponseBodyAuthorityTemplateViewAuthorityTemplateItemList(TeaModel):
+    def __init__(
+        self,
+        authority_template_item: List[GetAuthorityTemplateResponseBodyAuthorityTemplateViewAuthorityTemplateItemListAuthorityTemplateItem] = None,
+    ):
+        self.authority_template_item = authority_template_item
+
+    def validate(self):
+        if self.authority_template_item:
+            for k in self.authority_template_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['AuthorityTemplateItem'] = []
+        if self.authority_template_item is not None:
+            for k in self.authority_template_item:
+                result['AuthorityTemplateItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.authority_template_item = []
+        if m.get('AuthorityTemplateItem') is not None:
+            for k in m.get('AuthorityTemplateItem'):
+                temp_model = GetAuthorityTemplateResponseBodyAuthorityTemplateViewAuthorityTemplateItemListAuthorityTemplateItem()
+                self.authority_template_item.append(temp_model.from_map(k))
+        return self
+
+
+class GetAuthorityTemplateResponseBodyAuthorityTemplateView(TeaModel):
+    def __init__(
+        self,
+        authority_template_item_list: GetAuthorityTemplateResponseBodyAuthorityTemplateViewAuthorityTemplateItemList = None,
+        create_time: str = None,
+        creator_id: int = None,
+        description: str = None,
+        name: str = None,
+        template_id: int = None,
+    ):
+        # The resource information in the permission template.
+        self.authority_template_item_list = authority_template_item_list
+        # The time when the permission template was created. The time is in the yyyy-MM-DD HH:mm:ss format.
+        self.create_time = create_time
+        # The ID of the user who created the permission template.
+        self.creator_id = creator_id
+        # The description of the permission template.
+        self.description = description
+        # The name of the permission template.
+        self.name = name
+        # The ID of the permission template.
+        self.template_id = template_id
+
+    def validate(self):
+        if self.authority_template_item_list:
+            self.authority_template_item_list.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.authority_template_item_list is not None:
+            result['AuthorityTemplateItemList'] = self.authority_template_item_list.to_map()
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.creator_id is not None:
+            result['CreatorId'] = self.creator_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthorityTemplateItemList') is not None:
+            temp_model = GetAuthorityTemplateResponseBodyAuthorityTemplateViewAuthorityTemplateItemList()
+            self.authority_template_item_list = temp_model.from_map(m['AuthorityTemplateItemList'])
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('CreatorId') is not None:
+            self.creator_id = m.get('CreatorId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class GetAuthorityTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        authority_template_view: GetAuthorityTemplateResponseBodyAuthorityTemplateView = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        # The details of the permission template.
+        self.authority_template_view = authority_template_view
+        # The error code returned if the request failed.
+        self.error_code = error_code
+        # The error message returned if the request failed.
+        self.error_message = error_message
+        # The ID of the request.
+        self.request_id = request_id
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
+        self.success = success
+
+    def validate(self):
+        if self.authority_template_view:
+            self.authority_template_view.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.authority_template_view is not None:
+            result['AuthorityTemplateView'] = self.authority_template_view.to_map()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthorityTemplateView') is not None:
+            temp_model = GetAuthorityTemplateResponseBodyAuthorityTemplateView()
+            self.authority_template_view = temp_model.from_map(m['AuthorityTemplateView'])
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetAuthorityTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetAuthorityTemplateResponseBody = None,
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
+            temp_model = GetAuthorityTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class GetAuthorityTemplateItemRequest(TeaModel):
+    def __init__(
+        self,
+        template_id: int = None,
+        tid: int = None,
+    ):
+        # The ID of the permission template.
+        self.template_id = template_id
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
+        self.tid = tid
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
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetAuthorityTemplateItemResponseBodyAuthorityTemplateItemListAuthorityTemplateItem(TeaModel):
+    def __init__(
+        self,
+        attribute: str = None,
+        db_id: int = None,
+        instance_id: int = None,
+        item_id: int = None,
+        modifier_id: int = None,
+        resource_type: str = None,
+        table_name: str = None,
+        template_id: int = None,
+    ):
+        # The additional information. For example, permissions to log on to an instance are added to the permission template.
+        self.attribute = attribute
+        # The ID of the database.
+        self.db_id = db_id
+        # The ID of the instance.
+        self.instance_id = instance_id
+        # The ID of the resource.
+        self.item_id = item_id
+        # The ID of the user who modifies the resource.
+        self.modifier_id = modifier_id
+        # The type of the resource. Valid values:
+        # 
+        # *   **INSTANCE**: instance
+        # *   **LOGIC_DB**: logical database
+        # *   **META_DB**: physical database
+        # *   **LOGIC_TABLE**: logical table
+        # *   **LOGIC_TABLE**: physical table
+        self.resource_type = resource_type
+        # The name of the table.
+        self.table_name = table_name
+        # The ID of the permission template.
+        self.template_id = template_id
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
+        if self.attribute is not None:
+            result['Attribute'] = self.attribute
+        if self.db_id is not None:
+            result['DbId'] = self.db_id
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.item_id is not None:
+            result['ItemId'] = self.item_id
+        if self.modifier_id is not None:
+            result['ModifierId'] = self.modifier_id
+        if self.resource_type is not None:
+            result['ResourceType'] = self.resource_type
+        if self.table_name is not None:
+            result['TableName'] = self.table_name
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Attribute') is not None:
+            self.attribute = m.get('Attribute')
+        if m.get('DbId') is not None:
+            self.db_id = m.get('DbId')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('ItemId') is not None:
+            self.item_id = m.get('ItemId')
+        if m.get('ModifierId') is not None:
+            self.modifier_id = m.get('ModifierId')
+        if m.get('ResourceType') is not None:
+            self.resource_type = m.get('ResourceType')
+        if m.get('TableName') is not None:
+            self.table_name = m.get('TableName')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class GetAuthorityTemplateItemResponseBodyAuthorityTemplateItemList(TeaModel):
+    def __init__(
+        self,
+        authority_template_item: List[GetAuthorityTemplateItemResponseBodyAuthorityTemplateItemListAuthorityTemplateItem] = None,
+    ):
+        self.authority_template_item = authority_template_item
+
+    def validate(self):
+        if self.authority_template_item:
+            for k in self.authority_template_item:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['AuthorityTemplateItem'] = []
+        if self.authority_template_item is not None:
+            for k in self.authority_template_item:
+                result['AuthorityTemplateItem'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.authority_template_item = []
+        if m.get('AuthorityTemplateItem') is not None:
+            for k in m.get('AuthorityTemplateItem'):
+                temp_model = GetAuthorityTemplateItemResponseBodyAuthorityTemplateItemListAuthorityTemplateItem()
+                self.authority_template_item.append(temp_model.from_map(k))
+        return self
+
+
+class GetAuthorityTemplateItemResponseBody(TeaModel):
+    def __init__(
+        self,
+        authority_template_item_list: GetAuthorityTemplateItemResponseBodyAuthorityTemplateItemList = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        # The permission templates.
+        self.authority_template_item_list = authority_template_item_list
+        # The error code.
+        self.error_code = error_code
+        # The error message.
+        self.error_message = error_message
+        # The ID of the request.
+        self.request_id = request_id
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
+        self.success = success
+
+    def validate(self):
+        if self.authority_template_item_list:
+            self.authority_template_item_list.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.authority_template_item_list is not None:
+            result['AuthorityTemplateItemList'] = self.authority_template_item_list.to_map()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthorityTemplateItemList') is not None:
+            temp_model = GetAuthorityTemplateItemResponseBodyAuthorityTemplateItemList()
+            self.authority_template_item_list = temp_model.from_map(m['AuthorityTemplateItemList'])
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetAuthorityTemplateItemResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetAuthorityTemplateItemResponseBody = None,
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
+            temp_model = GetAuthorityTemplateItemResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetDBTaskSQLJobLogRequest(TeaModel):
     def __init__(
         self,
         job_id: int = None,
         tid: int = None,
     ):
         # The ID of the SQL task. You can call the [ListDBTaskSQLJob](~~207049~~) operation to query the ID of the SQL task.
@@ -10321,15 +11267,21 @@
 
 class GetDBTopologyRequest(TeaModel):
     def __init__(
         self,
         logic_db_id: int = None,
         tid: int = None,
     ):
+        # The ID of the logical database.
+        # 
+        # > You can call the [ListLogicDatabases](~~141874~~) operation to query the ID of the logical database.
         self.logic_db_id = logic_db_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10362,23 +11314,60 @@
         instance_id: int = None,
         instance_resource_id: str = None,
         instance_source: str = None,
         region_id: str = None,
         schema_name: str = None,
         search_name: str = None,
     ):
+        # The name of the catalog to which the database belongs.
+        # 
+        # > If the database is a PostgreSQL database, the value of this parameter is the name of the database.
         self.catalog_name = catalog_name
+        # The ID of the logical database.
         self.db_id = db_id
+        # The type of the database. For more information about the valid values of this parameter, see [DbType parameter](~~198106~~).
         self.db_type = db_type
+        # The type of the environment to which the logical database belongs. Valid values:
+        # 
+        # *   **product**: production environment
+        # *   **dev**: development environment
+        # *   **pre**: pre-release environment
+        # *   **test**: test environment
+        # *   **sit**: SIT environment
+        # *   **uat**: UAT environment
+        # *   **pet**: stress testing environment
+        # *   **stag**: staging environment
+        # 
+        # > For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # The ID of the instance in which the logical database resides.
         self.instance_id = instance_id
+        # The ID of the resource related to the instance. The resource corresponds with the database instance type returned in the InstanceSource parameter.
+        # 
+        # *   If the value of the InstanceSource parameter is RDS, the ID of an ApsaraDB RDS instance is returned.
+        # *   If the value of the InstanceSource parameter is ECS_OWN, the ID of a self-managed database that is hosted on an Elastic Compute Service (ECS) instance is returned.
+        # *   If the value of the InstanceSource parameter is PUBLIC_OWN, an empty string is returned.
+        # *   If the value of the InstanceSource parameter is VPC_ID, the ID of a self-managed database instance in a virtual private cloud (VPC) that is connected over Express Connect circuits is returned.
+        # *   If the value of the InstanceSource parameter is GATEWAY, the ID of a database instance connected by using a database gateway is returned.
         self.instance_resource_id = instance_resource_id
+        # The type of the database instance. Valid values:
+        # 
+        # *   **RDS**: an ApsaraDB RDS instance.
+        # *   **ECS_OWN**: a self-managed database that is hosted on an ECS instance.
+        # *   **PUBLIC_OWN**: a self-managed database instance that is connected over the Internet.
+        # *   **VPC_ID**: a self-managed database instance in a VPC that is connected over Express Connect circuits.
+        # *   **GATEWAY**: a database instance connected by using a database gateway.
         self.instance_source = instance_source
+        # The ID of the region in which the instance resides.
         self.region_id = region_id
+        # The name of the logical database.
+        # 
+        # > If the database is a PostgreSQL database, the value of this parameter is the name of the database schema.
         self.schema_name = schema_name
+        # The name that is used to search for the database.
         self.search_name = search_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10440,20 +11429,38 @@
         dbtopology_info_list: List[GetDBTopologyResponseBodyDBTopologyDBTopologyInfoList] = None,
         db_type: str = None,
         env_type: str = None,
         logic_db_id: int = None,
         logic_db_name: str = None,
         search_name: str = None,
     ):
+        # The alias of the logical database.
         self.alias = alias
+        # The topologies of the physical database shards.
         self.dbtopology_info_list = dbtopology_info_list
+        # The type of the database. For more information about the valid values of this parameter, see [DbType parameter](~~198106~~).
         self.db_type = db_type
+        # The type of the environment to which the logical database belongs. Valid values:
+        # 
+        # *   **product**: production environment
+        # *   **dev**: development environment
+        # *   **pre**: pre-release environment
+        # *   **test**: test environment
+        # *   **sit**: system integration testing (SIT) environment
+        # *   **uat**: user acceptance testing (UAT) environment
+        # *   **pet**: stress testing environment
+        # *   **stag**: staging environment
+        # 
+        # > For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # The ID of the logical database.
         self.logic_db_id = logic_db_id
+        # The name of the logical database.
         self.logic_db_name = logic_db_name
+        # The name that is used to search for the logical database.
         self.search_name = search_name
 
     def validate(self):
         if self.dbtopology_info_list:
             for k in self.dbtopology_info_list:
                 if k:
                     k.validate()
@@ -10509,18 +11516,23 @@
         self,
         dbtopology: GetDBTopologyResponseBodyDBTopology = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The topology of the logical database.
         self.dbtopology = dbtopology
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.dbtopology:
             self.dbtopology.validate()
 
     def to_map(self):
@@ -11473,15 +12485,19 @@
 
 class GetDataCorrectSQLFileRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11509,18 +12525,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         file_url: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The download URL of the SQL script.
         self.file_url = file_url
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11601,15 +12622,19 @@
 
 class GetDataCorrectTaskDetailRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket. You can call the [CreateDataCorrectOrder](~~208388~~), [CreateDataImportOrder](~~208387~~), or [CreateFreeLockCorrectOrder](~~208386~~) operation to obtain the ticket ID.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](~~181330~~) topic.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11636,17 +12661,30 @@
     def __init__(
         self,
         actual_affect_rows: int = None,
         create_time: str = None,
         dbtask_group_id: int = None,
         job_status: str = None,
     ):
+        # The number of rows affected by the SQL statement.
         self.actual_affect_rows = actual_affect_rows
+        # The time when the task was created.
         self.create_time = create_time
+        # The ID of the SQL task group.
         self.dbtask_group_id = dbtask_group_id
+        # The state of the SQL task. Valid values:
+        # 
+        # *   **INIT**: The SQL task was initialized.
+        # *   **PENDING**: The SQL task waited to be run.
+        # *   **BE_SCHEDULED**: The SQL task waited to be scheduled.
+        # *   **FAIL**: The SQL task failed.
+        # *   **SUCCESS**: The SQL task was successful.
+        # *   **PAUSE**: The SQL task was paused.
+        # *   **DELETE**: The SQL task was deleted.
+        # *   **RUNNING**: The SQL task was being run.
         self.job_status = job_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11682,18 +12720,23 @@
         self,
         data_correct_task_detail: GetDataCorrectTaskDetailResponseBodyDataCorrectTaskDetail = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The details of the data change task.
         self.data_correct_task_detail = data_correct_task_detail
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         if self.data_correct_task_detail:
             self.data_correct_task_detail.validate()
 
     def to_map(self):
@@ -12002,17 +13045,23 @@
     def __init__(
         self,
         order_id: int = None,
         page_number: int = None,
         page_size: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket. You can query the ticket ID from the response parameters of the [CreateDataCronClearOrder](~~208385~~) operation.
         self.order_id = order_id
+        # The number of the page to return.
         self.page_number = page_number
+        # The number of entries to return on each page.
         self.page_size = page_size
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](~~181330~~) topic.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12047,17 +13096,30 @@
     def __init__(
         self,
         actual_affect_rows: int = None,
         create_time: str = None,
         dbtask_group_id: int = None,
         job_status: str = None,
     ):
+        # The number of rows affected by the SQL task.
         self.actual_affect_rows = actual_affect_rows
+        # The time when the SQL task was created.
         self.create_time = create_time
+        # The ID of the SQL task group.
         self.dbtask_group_id = dbtask_group_id
+        # The state of the SQL task. Valid values:
+        # 
+        # *   **INIT**: The SQL task was initialized.
+        # *   **PENDING**: The SQL task waited to be run.
+        # *   **BE_SCHEDULED**: The SQL task waited to be scheduled.
+        # *   **FAIL**: The SQL task failed.
+        # *   **SUCCESS**: The SQL task was successful.
+        # *   **PAUSE**: The SQL task was paused.
+        # *   **DELETE**: The SQL task was deleted.
+        # *   **RUNNING**: The SQL task was being run.
         self.job_status = job_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12094,19 +13156,25 @@
         data_cron_clear_task_detail_list: List[GetDataCronClearTaskDetailListResponseBodyDataCronClearTaskDetailList] = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
+        # The historical data cleansing tasks
         self.data_cron_clear_task_detail_list = data_cron_clear_task_detail_list
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful.
         self.success = success
+        # The total number of SQL tasks.
         self.total_count = total_count
 
     def validate(self):
         if self.data_cron_clear_task_detail_list:
             for k in self.data_cron_clear_task_detail_list:
                 if k:
                     k.validate()
@@ -12384,15 +13452,19 @@
 
 class GetDataExportOrderDetailRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12417,15 +13489,28 @@
 
 class GetDataExportOrderDetailResponseBodyDataExportOrderDetailKeyInfo(TeaModel):
     def __init__(
         self,
         job_status: str = None,
         pre_check_id: int = None,
     ):
+        # The status of the data export ticket. Valid values:
+        # 
+        # *   PRE_CHECKING: The ticket is being prechecked.
+        # *   PRE_CHECK_SUCCESS: The ticket passes the precheck.
+        # *   PRE_CHECK_FAIL: The ticket fails to pass the precheck.
+        # *   WAITING_APPLY_AUDIT: The ticket is to be submitted for approval.
+        # *   APPLY_AUDIT_SUCESS: The ticket is submitted for approval.
+        # *   ENABLE_EXPORT: The ticket is approved. Data can be exported.
+        # *   WAITING_EXPORT: Data is to be scheduled for export.
+        # *   DOING_EXPORT: Data is being exported.
+        # *   EXPORT_FAIL: Data fails to be exported.
+        # *   EXPORT_SUCCESS: Data is exported.
         self.job_status = job_status
+        # The ID of the precheck.
         self.pre_check_id = pre_check_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12457,22 +13542,31 @@
         db_id: int = None,
         env_type: str = None,
         exe_sql: str = None,
         ignore_affect_rows: bool = None,
         ignore_affect_rows_reason: str = None,
         logic: bool = None,
     ):
+        # The number of rows that are affected by the system check.
         self.actual_affect_rows = actual_affect_rows
+        # The category of the reason for the data export.
         self.classify = classify
+        # The database from which data is exported.
         self.database = database
+        # The ID of the database from which you want to export data.
         self.db_id = db_id
+        # The type of the environment to which the database belongs.
         self.env_type = env_type
+        # The SQL statement that is executed to export data.
         self.exe_sql = exe_sql
+        # Indicates whether the affected rows are skipped.
         self.ignore_affect_rows = ignore_affect_rows
+        # The reason why the affected rows are skipped.
         self.ignore_affect_rows_reason = ignore_affect_rows_reason
+        # Indicates whether the database is a logical database.
         self.logic = logic
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12525,15 +13619,17 @@
 
 class GetDataExportOrderDetailResponseBodyDataExportOrderDetail(TeaModel):
     def __init__(
         self,
         key_info: GetDataExportOrderDetailResponseBodyDataExportOrderDetailKeyInfo = None,
         order_detail: GetDataExportOrderDetailResponseBodyDataExportOrderDetailOrderDetail = None,
     ):
+        # The status information of the data export ticket.
         self.key_info = key_info
+        # The details of the ticket.
         self.order_detail = order_detail
 
     def validate(self):
         if self.key_info:
             self.key_info.validate()
         if self.order_detail:
             self.order_detail.validate()
@@ -12566,18 +13662,23 @@
         self,
         data_export_order_detail: GetDataExportOrderDetailResponseBodyDataExportOrderDetail = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The details of the data export ticket.
         self.data_export_order_detail = data_export_order_detail
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.data_export_order_detail:
             self.data_export_order_detail.validate()
 
     def to_map(self):
@@ -12654,14 +13755,177 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetDataExportOrderDetailResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetDataImportSQLRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        sql_id: int = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.sql_id = sql_id
+        self.tid = tid
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
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class GetDataImportSQLResponseBodySQLDetail(TeaModel):
+    def __init__(
+        self,
+        exec_sql: str = None,
+    ):
+        self.exec_sql = exec_sql
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
+        if self.exec_sql is not None:
+            result['ExecSql'] = self.exec_sql
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ExecSql') is not None:
+            self.exec_sql = m.get('ExecSql')
+        return self
+
+
+class GetDataImportSQLResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        sqldetail: GetDataImportSQLResponseBodySQLDetail = None,
+        success: bool = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.sqldetail = sqldetail
+        self.success = success
+
+    def validate(self):
+        if self.sqldetail:
+            self.sqldetail.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.sqldetail is not None:
+            result['SQLDetail'] = self.sqldetail.to_map()
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SQLDetail') is not None:
+            temp_model = GetDataImportSQLResponseBodySQLDetail()
+            self.sqldetail = temp_model.from_map(m['SQLDetail'])
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GetDataImportSQLResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetDataImportSQLResponseBody = None,
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
+            temp_model = GetDataImportSQLResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetDatabaseRequest(TeaModel):
     def __init__(
         self,
         host: str = None,
         port: int = None,
         schema_name: str = None,
         sid: str = None,
@@ -13893,19 +15157,19 @@
 
 class GetLogicDatabaseRequest(TeaModel):
     def __init__(
         self,
         db_id: str = None,
         tid: int = None,
     ):
-        # The ID of the logical database. You can call the [ListLogicDatabases](https://www.alibabacloud.com/help/en/data-management-service/latest/listlogicdatabases) or [SearchDatabase](https://www.alibabacloud.com/help/en/data-management-service/latest/searchdatabase) operation to obtain the ID of the logical database.
+        # The ID of the logical database. You can call the [ListLogicDatabases](~~141874~~) or [SearchDatabase](~~141876~~) operation to obtain the ID of the logical database.
         self.db_id = db_id
-        # The ID of the tenant. 
+        # The ID of the tenant.
         # 
-        # >  To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](https://www.alibabacloud.com/help/en/data-management-service/latest/manage-dms-tenants) topic.
+        # > To view the ID of the tenant, go to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [View information about the current tenant](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14023,27 +15287,28 @@
         schema_name: str = None,
         search_name: str = None,
     ):
         # The alias of the logical database.
         self.alias = alias
         # The ID of the logical database.
         self.database_id = database_id
+        # The IDs of database shards of the logical database.
         self.database_ids = database_ids
-        # The type of the database. For more information about the valid values of the DbType parameter, see [DbType parameter](https://www.alibabacloud.com/help/en/data-management-service/latest/dbtype-parameter).
+        # The database engine. For more information about the valid values of the DbType parameter, see [DbType parameter](~~198106~~).
         self.db_type = db_type
         # The type of the environment to which the database belongs. Valid values:
         # 
-        # - product: production environment
-        # - dev: development environment
-        # - pre: staging environment
-        # - test: test environment
-        # - sit: SIT environment
-        # - uat: user acceptance testing (UAT) environment
-        # - pet: stress testing environment
-        # - stag: STAG environment
+        # *   product: production environment
+        # *   dev: development environment
+        # *   pre: pre-release environment
+        # *   test: test environment
+        # *   sit: system integration testing (SIT) environment
+        # *   uat: user acceptance testing (UAT) environment
+        # *   pet: stress testing environment
+        # *   stag: staging environment
         self.env_type = env_type
         # Indicates whether the database is a logical database. The return value is true.
         self.logic = logic
         # The IDs of the owners of the logical database.
         self.owner_id_list = owner_id_list
         # The names of the owners of the logical database.
         self.owner_name_list = owner_name_list
@@ -14121,26 +15386,26 @@
         self,
         error_code: str = None,
         error_message: str = None,
         logic_database: GetLogicDatabaseResponseBodyLogicDatabase = None,
         request_id: str = None,
         success: bool = None,
     ):
-        # The error code.
+        # The status code.
         self.error_code = error_code
         # The error message.
         self.error_message = error_message
-        # The details about the logical database.
+        # The details of the logical database.
         self.logic_database = logic_database
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful. Valid values:
+        # Indicates whether the request was successful. Valid values:
         # 
-        # - true: The request is successful.
-        # - false: The request fails.
+        # *   true: The request was successful.
+        # *   false: The request failed.
         self.success = success
 
     def validate(self):
         if self.logic_database:
             self.logic_database.validate()
 
     def to_map(self):
@@ -14228,15 +15493,15 @@
         tid: int = None,
     ):
         # The globally unique identifier (GUID) of the table in Data Management (DMS).
         # 
         # *   If the database to which the table belongs is a logical database, you can call the [ListLogicTables](~~141875~~) operation to obtain the value of this parameter.
         # *   If the database to which the table belongs is a physical database, you can call the [ListTables](~~141878~~) operation to obtain the value of this parameter.
         self.table_guid = table_guid
-        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to query the tenant ID.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to obtain the tenant ID.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14271,54 +15536,54 @@
         data_scale: int = None,
         description: str = None,
         nullable: bool = None,
         position: int = None,
         primary_key: str = None,
         security_level: str = None,
     ):
-        # Indicates whether the field is an auto-increment field. Valid values:
+        # Indicates whether the column is an auto-increment column. Valid values:
         # 
-        # *   **true**: The field is an auto-increment field.
-        # *   **false**: The field is not an auto-increment field.
+        # *   **true**: The column is an auto-increment column.
+        # *   **false**: The column is not an auto-increment column.
         self.auto_increment = auto_increment
-        # The ID of the field.
+        # The ID of the column.
         self.column_id = column_id
-        # The name of the field.
+        # The name of the column.
         self.column_name = column_name
-        # The data type of the field.
+        # The data type of the column.
         # 
-        # >  The returned data type is not unique. For example, the returned data type can be **bigint** or **int**.
+        # > The return value of a column is not unique, such as **bigint** or **int**.
         self.column_type = column_type
         # The length of the field.
         self.data_length = data_length
         # The precision of the field.
         self.data_precision = data_precision
-        # The number of decimal places that the field shows.
+        # The number of decimal places for the field.
         self.data_scale = data_scale
-        # The description of the field.
+        # The description of the column.
         self.description = description
         # Indicates whether the field can be empty. Valid values:
         # 
         # *   **true**: The field can be empty.
         # *   **false**: The field cannot be empty.
         self.nullable = nullable
         # The position of the field in the table.
         self.position = position
         # Indicates whether the field is the primary key. Valid values:
         # 
         # *   **true**: The field is the primary key.
         # *   **false**: The field is not the primary key.
         self.primary_key = primary_key
-        # The sensitivity level of the field. Valid values:
+        # The sensitivity level of the column. Valid values:
         # 
-        # *   **INNER**: The field is not sensitive.
-        # *   **SENSITIVE**: The field is sensitive.
-        # *   **CONFIDENTIAL**: The field is confidential.
+        # *   **INNER**: The column is not sensitive.
+        # *   **SENSITIVE**: The column is sensitive.
+        # *   **CONFIDENTIAL**: The column is confidential.
         # 
-        # >  For more information, see [Sensitivity levels of fields](~~66091~~).
+        # > For more information, see [Sensitivity levels of columns](~~66091~~).
         self.security_level = security_level
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14494,15 +15759,25 @@
 
 class GetMetaTableDetailInfoRequest(TeaModel):
     def __init__(
         self,
         table_guid: str = None,
         tid: int = None,
     ):
+        # The GUID of the table in Data Management (DMS).
+        # 
+        # > 
+        # 
+        # *   You can call the [ListLogicTables](~~141875~~) operation with ReturnGuid set to true to query the GUIDs of logical tables in a specific logical database.
+        # 
+        # *   You can call the [ListTables](~~141878~~) operation with ReturnGuid set to true to query the GUIDs of tables in a specific physical database.
         self.table_guid = table_guid
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the [View information about the current tenant](~~181330~~) section of the Manage DMS tenants topic.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14535,23 +15810,39 @@
         data_length: int = None,
         data_precision: int = None,
         data_scale: int = None,
         description: str = None,
         nullable: bool = None,
         position: str = None,
     ):
+        # Indicates whether the column is an auto-increment column. Valid values:
+        # 
+        # *   true: The column is an auto-increment column.
+        # *   false: The column is not an auto-increment column.
         self.auto_increment = auto_increment
+        # The ID of the column.
         self.column_id = column_id
+        # The name of the column.
         self.column_name = column_name
+        # The data type of the column. Examples: Bigint, Int, and Varchar.
         self.column_type = column_type
+        # The length of the field.
         self.data_length = data_length
+        # The precision of the field.
         self.data_precision = data_precision
+        # The scale of the column.
         self.data_scale = data_scale
+        # The description of the column.
         self.description = description
+        # Indicates whether the column is nullable. Valid values:
+        # 
+        # *   true: The column is nullable.
+        # *   false: The column is not nullable.
         self.nullable = nullable
+        # The position of the field in the table.
         self.position = position
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14611,18 +15902,26 @@
         self,
         index_columns: List[str] = None,
         index_id: str = None,
         index_name: str = None,
         index_type: str = None,
         unique: bool = None,
     ):
+        # The index column.
         self.index_columns = index_columns
+        # The ID of the index.
         self.index_id = index_id
+        # The name of the index.
         self.index_name = index_name
+        # The type of the index. Examples: Primary, Unique, and Normal.
         self.index_type = index_type
+        # Indicates whether the index is unique. Valid values:
+        # 
+        # *   true: The index is unique.
+        # *   false: The index is not unique.
         self.unique = unique
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14659,15 +15958,17 @@
 
 class GetMetaTableDetailInfoResponseBodyDetailInfo(TeaModel):
     def __init__(
         self,
         column_list: List[GetMetaTableDetailInfoResponseBodyDetailInfoColumnList] = None,
         index_list: List[GetMetaTableDetailInfoResponseBodyDetailInfoIndexList] = None,
     ):
+        # The columns in the table.
         self.column_list = column_list
+        # The list of indexes.
         self.index_list = index_list
 
     def validate(self):
         if self.column_list:
             for k in self.column_list:
                 if k:
                     k.validate()
@@ -14712,18 +16013,23 @@
         self,
         detail_info: GetMetaTableDetailInfoResponseBodyDetailInfo = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The details of the table.
         self.detail_info = detail_info
+        # The error code returned.
         self.error_code = error_code
+        # The error message returned.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         if self.detail_info:
             self.detail_info.validate()
 
     def to_map(self):
@@ -14806,15 +16112,19 @@
 
 class GetOnlineDDLProgressRequest(TeaModel):
     def __init__(
         self,
         job_detail_id: int = None,
         tid: int = None,
     ):
+        # The ID of the OnlineDDL SQL task details. You can call the [ListDBTaskSQLJobDetail](~~207073~~) operation to obtain the task detail ID.
         self.job_detail_id = job_detail_id
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, go to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](~~181330~~) topic.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14850,26 +16160,59 @@
         cutover_window_end_time: str = None,
         cutover_window_start_time: str = None,
         delay_seconds: int = None,
         job_status: str = None,
         progress_ratio: str = None,
         status_desc: str = None,
     ):
+        # The cleanup policy of the original table after the cut-over. Valid values:
+        # 
+        # *   **DROP**: Invalid original tables are deleted.
+        # *   **MOVE**: Invalid original tables are moved to the test database. You can delete the tables manually.
+        # *   **NOTHING**: Invalid original tables are retained in the original database. You can delete the tables manually.
         self.clean_strategy = clean_strategy
+        # The policy of full replication. Valid values:
+        # 
+        # *   **AUTO**: DMS dynamically adjusts the chunk size based on the performance of the database. Tables are locked for less than 1.5 seconds during a single replication operation.
+        # *   **RUNNING**: DMS uses the specified value of the CopyChunkSize parameter. The valid value of the CopyChunkSize parameter ranges from 1 to 60000. If you set this parameter to RUNNING, you must specify the CopyChunkSize parameter.
         self.copy_chunk_mode = copy_chunk_mode
+        # The size of each chunk that is used to replicate data. This parameter is used to specify the size of each chunk. A larger chunk size increases the replication efficiency and decreases the business performance.
+        # 
+        # > During full replication, the original table is divided into N small chunks and each chunk is replicated to the temporary table one by one. By default, DMS dynamically adjusts the size of each chunk.
         self.copy_chunk_size = copy_chunk_size
+        # The actual amount of data replicated from the original table in the lock-free change operation.
         self.copy_count = copy_count
+        # The estimated total number of rows of the data. The value is obtained from the statistical data in the information_schema database. In most cases, the estimated total number of rows is smaller than the actual number of rows in a table.
         self.copy_total = copy_total
+        # The number of retries when the cut-over fails.
         self.cutover_fail_retry_times = cutover_fail_retry_times
+        # The maximum period of time that a table can be locked during cut-over. Unit: seconds.
         self.cutover_lock_time_seconds = cutover_lock_time_seconds
+        # The end of the time window of the cut-over operation. This value is at least 30 minutes later than the CutoverWindowStartTime parameter. Default value: 23:59:59
         self.cutover_window_end_time = cutover_window_end_time
+        # The beginning of the time window of the cut-over operation. Default value: 00:00:00. This parameter controls the time window of the cut-over. Cut-over can be performed only when the cut-over conditions are met and the time is within the specified time window. If the time is not within the time window, the cut-over operation is not performed until the time reaches the beginning of the time window.
         self.cutover_window_start_time = cutover_window_start_time
+        # The replay latency of DMS. Unit: seconds. The replay latency is the period of time that is taken to replay the binary logs of the table to the temporary table. The latency does not indicate the data migration latency between a primary database and a secondary database.
         self.delay_seconds = delay_seconds
+        # The state of the task. Valid values:
+        # 
+        # *   **INIT**: The task is being initialized.
+        # *   **SUCCESS**: The task is complete.
+        # *   **RUNNING**: The task is being executed.
+        # *   **WAITING_CUTOVER**: The task is waiting for cut-over.
+        # *   **RESTARTING**: The task is restarting.
+        # *   **PAUSE**: The task is suspended.
+        # *   **UNSUPPORTED**: The task is not supported.
+        # *   **CANCELED**: The task is canceled.
+        # *   **FAIL**: The task failed.
+        # *   **INTERRUPT**: The task is interrupted.
         self.job_status = job_status
+        # The estimated execution progress. The actual progress is subject to the task status.
         self.progress_ratio = progress_ratio
+        # The description of the task status.
         self.status_desc = status_desc
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14941,18 +16284,26 @@
         self,
         error_code: str = None,
         error_message: str = None,
         online_ddltask_detail: GetOnlineDDLProgressResponseBodyOnlineDDLTaskDetail = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The details of the task.
         self.online_ddltask_detail = online_ddltask_detail
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         if self.online_ddltask_detail:
             self.online_ddltask_detail.validate()
 
     def to_map(self):
@@ -15046,39 +16397,47 @@
         # The end of the time range to query. Specify the time in the yyyy-MM-DD HH:mm:ss format.
         self.end_time = end_time
         # The functional module for which you want to query operation logs. If you do not specify this parameter, operation logs for all functional modules are returned. Valid values:
         # 
         # *   **PERMISSION**: permissions
         # *   **OWNER**: data owner
         # *   **SQL_CONSOLE**: data query
-        # *   **SQL\_CONSOLE\_EXPORT**: query result export
+        # *   **SQL_CONSOLE_EXPORT**: query result export
         # *   **DATA_CHANGE**: data change
         # *   **DATA_EXPORT**: data export
         # *   **SQL_REVIEW**: SQL review
         # *   **DT_SYNC**: database and table synchronization
         # *   **DT_DETAIL**: database and table details
         # *   **DB_TASK**: task management
         # *   **INSTANCE_MANAGE**: instance management
         # *   **USER_MANAGE**: user management
-        # *   **SECURITY_RULE**: security rule
+        # *   **SECURITY_RULE**: security rules
         # *   **CONFIG_MANAGE**: configuration management
         # *   **RESOURCE_AUTH**: resource authorization
-        # *   **ACCESS\_WHITE\_IP**: access IP address allowlist
+        # *   **ACCESS_WHITE_IP**: access IP address whitelist
+        # *   **NDDL**: schema design
+        # *   **DSQL_CONSOLE**: cross-database data query
+        # *   **DSQL_CONSOLE_EXPORT**: cross-database query result export
+        # *   **DATA_TRACT**: data tracking
+        # *   **DATA_QUALITY**: data quality
+        # *   **DATALINK_MANAGE** :DBLink management
+        # *   **DATASEC_MANAGE**: sensitive data management
+        # *   **SELL**: sales
         self.module = module
         # The number of the page to return. Pages start from page 1.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values:
         # 
         # *   30
         # *   50
         # *   100
         self.page_size = page_size
         # The beginning of the time range to query. Specify the time in the yyyy-MM-DD HH:mm:ss format.
         self.start_time = start_time
-        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to obtain the tenant ID.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15127,30 +16486,33 @@
         op_user_id: int = None,
         order_id: int = None,
         user_id: str = None,
         user_nick: str = None,
     ):
         # The endpoint of the database instance.
         # 
-        # > * This parameter is valid only for database instances of the LocalInstance type.
-        # > * This parameter is valid only for operations on the functional modules related to tasks.
+        # > 
+        # 
+        # *   This parameter is valid only for database instances of the LocalInstance type.
+        # 
+        # *   This parameter is valid only for operations on the functional modules related to tasks.
         self.database = database
         # The functional module for which the operation log is queried.
         self.module = module
         # The details of the operation.
         self.op_content = op_content
         # The time when the operation was performed.
         self.op_time = op_time
         # The ID of the user who performed the operation.
         self.op_user_id = op_user_id
         # The ID of the ticket or task.
         # 
         # >  This parameter is valid only for operations on the functional modules related to tasks and the task management module in system management.
         self.order_id = order_id
-        # The UID of the Alibaba Cloud account.
+        # The ID of the Alibaba Cloud account.
         self.user_id = user_id
         # The display name of the user.
         self.user_nick = user_nick
 
     def validate(self):
         pass
 
@@ -15240,26 +16602,26 @@
         error_code: str = None,
         error_message: str = None,
         op_log_details: GetOpLogResponseBodyOpLogDetails = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The error code returned if the request fails.
+        # The error code.
         self.error_code = error_code
-        # The error message returned if the request fails.
+        # The error message returned if the request failed.
         self.error_message = error_message
         # The details of the operation log.
         self.op_log_details = op_log_details
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request is successful. Valid values:
+        # Indicates whether the request was successful. Valid values:
         # 
-        # - **true**: The request is successful.
-        # - **false**: The request fails.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
         # The total number of operation logs that are returned.
         self.total_count = total_count
 
     def validate(self):
         if self.op_log_details:
             self.op_log_details.validate()
@@ -15491,15 +16853,19 @@
 
 class GetOrderBaseInfoRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15589,26 +16955,47 @@
         related_user_list: GetOrderBaseInfoResponseBodyOrderBaseInfoRelatedUserList = None,
         related_user_nick_list: GetOrderBaseInfoResponseBodyOrderBaseInfoRelatedUserNickList = None,
         status_code: str = None,
         status_desc: str = None,
         workflow_instance_id: int = None,
         workflow_status_desc: str = None,
     ):
+        # The remarks of the ticket.
         self.comment = comment
+        # The applicant.
         self.committer = committer
+        # The ID of the applicant. Note: The ID is different from the Alibaba Cloud account ID of the applicant.
         self.committer_id = committer_id
+        # The time when the ticket was created.
         self.create_time = create_time
+        # The time when the ticket was last modified.
         self.last_modify_time = last_modify_time
+        # The ID of the ticket.
         self.order_id = order_id
+        # The type of the ticket. For more information about the value of this parameter, see the request parameters of the [CreateOrder](~~465865~~) operation.
         self.plugin_type = plugin_type
+        # The IDs of the operators that are related to the ticket.
         self.related_user_list = related_user_list
+        # The nicknames of the operators that are related to the ticket.
         self.related_user_nick_list = related_user_nick_list
+        # The status code of the ticket. Valid values:
+        # 
+        # *   **new**: The ticket is created.
+        # *   **toaudit**: The ticket is being reviewed.
+        # *   **Approved**: The ticket is approved.
+        # *   **reject**: The ticket is rejected.
+        # *   **processing**: The ticket is being executed.
+        # *   **success**: The ticket is executed.
+        # *   **closed**: The ticket is closed.
         self.status_code = status_code
+        # The description of the status.
         self.status_desc = status_desc
+        # The ID of the approval process.
         self.workflow_instance_id = workflow_instance_id
+        # The description of the approval process.
         self.workflow_status_desc = workflow_status_desc
 
     def validate(self):
         if self.related_user_list:
             self.related_user_list.validate()
         if self.related_user_nick_list:
             self.related_user_nick_list.validate()
@@ -15685,18 +17072,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         order_base_info: GetOrderBaseInfoResponseBodyOrderBaseInfo = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The basic information about the ticket.
         self.order_base_info = order_base_info
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.order_base_info:
             self.order_base_info.validate()
 
     def to_map(self):
@@ -15779,15 +17171,19 @@
 
 class GetOwnerApplyOrderDetailRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15816,19 +17212,27 @@
         db_type: str = None,
         env_type: str = None,
         owner_ids: List[int] = None,
         owner_nick_names: List[str] = None,
         search_name: str = None,
         table_name: str = None,
     ):
+        # The type of the database engine.
         self.db_type = db_type
+        # The type of the environment to which the instance belongs. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # The IDs of the original owners.
         self.owner_ids = owner_ids
+        # The nicknames of the owners.
         self.owner_nick_names = owner_nick_names
+        # The search name of the resource.
         self.search_name = search_name
+        # The name of the table.
+        # 
+        # > : This parameter is returned when you submit a Database-OWNER ticket.
         self.table_name = table_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15870,16 +17274,22 @@
 class GetOwnerApplyOrderDetailResponseBodyOwnerApplyOrderDetailResources(TeaModel):
     def __init__(
         self,
         logic: bool = None,
         resource_detail: GetOwnerApplyOrderDetailResponseBodyOwnerApplyOrderDetailResourcesResourceDetail = None,
         target_id: str = None,
     ):
+        # Indicates whether the database is a logical database. Valid values:
+        # 
+        # *   **true**: The instance is a logical database.
+        # *   **false**: The instance is not a logical database.
         self.logic = logic
+        # The details of the resource.
         self.resource_detail = resource_detail
+        # The ID of the resource.
         self.target_id = target_id
 
     def validate(self):
         if self.resource_detail:
             self.resource_detail.validate()
 
     def to_map(self):
@@ -15910,15 +17320,21 @@
 
 class GetOwnerApplyOrderDetailResponseBodyOwnerApplyOrderDetail(TeaModel):
     def __init__(
         self,
         apply_type: str = None,
         resources: List[GetOwnerApplyOrderDetailResponseBodyOwnerApplyOrderDetailResources] = None,
     ):
+        # The type of the submitted ticket. Valid values:
+        # 
+        # *   **INSTANCE**: the ticket that applies for the permissions to be an instance owner
+        # *   **DB**: the ticket that applies for the permissions to be a database owner
+        # *   **TABLE**: the ticket that applies for the permissions to be a table owner
         self.apply_type = apply_type
+        # The details of the requested resource.
         self.resources = resources
 
     def validate(self):
         if self.resources:
             for k in self.resources:
                 if k:
                     k.validate()
@@ -15954,18 +17370,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         owner_apply_order_detail: GetOwnerApplyOrderDetailResponseBodyOwnerApplyOrderDetail = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The details of the ticket.
         self.owner_apply_order_detail = owner_apply_order_detail
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.owner_apply_order_detail:
             self.owner_apply_order_detail.validate()
 
     def to_map(self):
@@ -16048,15 +17469,19 @@
 
 class GetPermApplyOrderDetailRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16081,15 +17506,17 @@
 
 class GetPermApplyOrderDetailResponseBodyPermApplyOrderDetailResourcesColumnInfo(TeaModel):
     def __init__(
         self,
         column_name: str = None,
         table_name: str = None,
     ):
+        # The name of the column.
         self.column_name = column_name
+        # The name of the table.
         self.table_name = table_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16119,20 +17546,30 @@
         db_type: str = None,
         env_type: str = None,
         logic: bool = None,
         owner_ids: List[int] = None,
         owner_nick_names: List[str] = None,
         search_name: str = None,
     ):
+        # The ID of the database.
         self.db_id = db_id
+        # The type of the database engine.
         self.db_type = db_type
+        # The type of the environment to which the instance belongs. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # Indicates whether the database is a logical database. Valid values:
+        # 
+        # *   **true**: The database is a logical database.
+        # *   **false**: The database is not a logical database.
         self.logic = logic
+        # The IDs of the owners of the database.
         self.owner_ids = owner_ids
+        # The nicknames of the owners of the database.
         self.owner_nick_names = owner_nick_names
+        # The name that is used to search for the database.
         self.search_name = search_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16185,23 +17622,33 @@
         host: str = None,
         instance_id: str = None,
         owner_ids: List[int] = None,
         owner_nick_name: List[str] = None,
         port: int = None,
         search_name: str = None,
     ):
+        # The type of the database engine.
         self.db_type = db_type
+        # The ID of the database administrator (DBA) of the instance.
         self.dba_id = dba_id
+        # The nickname of the DBA of the instance.
         self.dba_nick_name = dba_nick_name
+        # The type of the environment to which the instance belongs. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # The endpoint of the instance.
         self.host = host
+        # The ID of the instance.
         self.instance_id = instance_id
+        # The IDs of the owners of the instance.
         self.owner_ids = owner_ids
+        # The nicknames of the owners of the instance.
         self.owner_nick_name = owner_nick_name
+        # The port that is used to connect to the instance.
         self.port = port
+        # The name that is used to search for the instance.
         self.search_name = search_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16257,14 +17704,15 @@
 
 
 class GetPermApplyOrderDetailResponseBodyPermApplyOrderDetailResourcesTableInfo(TeaModel):
     def __init__(
         self,
         table_name: str = None,
     ):
+        # The name of the table.
         self.table_name = table_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16287,17 +17735,21 @@
     def __init__(
         self,
         column_info: GetPermApplyOrderDetailResponseBodyPermApplyOrderDetailResourcesColumnInfo = None,
         database_info: GetPermApplyOrderDetailResponseBodyPermApplyOrderDetailResourcesDatabaseInfo = None,
         instance_info: GetPermApplyOrderDetailResponseBodyPermApplyOrderDetailResourcesInstanceInfo = None,
         table_info: GetPermApplyOrderDetailResponseBodyPermApplyOrderDetailResourcesTableInfo = None,
     ):
+        # The information about the column.
         self.column_info = column_info
+        # The information about the database.
         self.database_info = database_info
+        # The information about the instance.
         self.instance_info = instance_info
+        # The information about the table.
         self.table_info = table_info
 
     def validate(self):
         if self.column_info:
             self.column_info.validate()
         if self.database_info:
             self.database_info.validate()
@@ -16343,17 +17795,34 @@
     def __init__(
         self,
         apply_type: str = None,
         perm_type: int = None,
         resources: List[GetPermApplyOrderDetailResponseBodyPermApplyOrderDetailResources] = None,
         seconds: int = None,
     ):
+        # The type of objects on which you apply for permissions. Valid values:
+        # 
+        # *   **DB**: database
+        # *   **TAB**: table
+        # *   **COL**: column
+        # *   **INSTANT**: instance
         self.apply_type = apply_type
+        # The type of permissions that you apply for. Valid values:
+        # 
+        # *   **1**: the permissions to query information
+        # *   **2**: the permissions to export information
+        # *   **3**: the permissions to query and export information
+        # *   **4**: the permissions to modify information
+        # *   **5**: the permissions to query and modify information
+        # *   **6**: the permissions to export and modify information
+        # *   **7**: the permissions to query, export, and modify information
         self.perm_type = perm_type
+        # The list of resources.
         self.resources = resources
+        # The validity duration of the permissions. Unit: seconds.
         self.seconds = seconds
 
     def validate(self):
         if self.resources:
             for k in self.resources:
                 if k:
                     k.validate()
@@ -16397,18 +17866,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         perm_apply_order_detail: GetPermApplyOrderDetailResponseBodyPermApplyOrderDetail = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The details of the permission application ticket.
         self.perm_apply_order_detail = perm_apply_order_detail
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.perm_apply_order_detail:
             self.perm_apply_order_detail.validate()
 
     def to_map(self):
@@ -16491,15 +17965,17 @@
 
 class GetPhysicalDatabaseRequest(TeaModel):
     def __init__(
         self,
         db_id: int = None,
         tid: int = None,
     ):
+        # The ID of the physical database. You can call the [SearchDatabase](~~141876~~) operation to obtain the ID.
         self.db_id = db_id
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to query the ID of the tenant.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16592,29 +18068,56 @@
         owner_name_list: GetPhysicalDatabaseResponseBodyDatabaseOwnerNameList = None,
         port: int = None,
         schema_name: str = None,
         search_name: str = None,
         sid: str = None,
         state: str = None,
     ):
+        # The name of the catalog to which the database belongs.
+        # 
+        # > : If the database is a PostgreSQL database, the name of the database is displayed.
         self.catalog_name = catalog_name
+        # The ID of the physical database.
         self.database_id = database_id
+        # The type of the database engine.
         self.db_type = db_type
+        # The user ID of the DBA in the destination database.
         self.dba_id = dba_id
+        # The nickname of the database administrator (DBA) in the destination database.
         self.dba_name = dba_name
+        # The encoding format of the database.
         self.encoding = encoding
+        # The type of the environment to which the database belongs. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # The endpoint that is used to connect to the database.
         self.host = host
+        # The instance ID of the destination database.
         self.instance_id = instance_id
+        # The user IDs of the database owners.
         self.owner_id_list = owner_id_list
+        # The nicknames of the database owners.
         self.owner_name_list = owner_name_list
+        # The port that is used to connect to the database.
         self.port = port
+        # The name of the database.
+        # 
+        # > : If the database is a PostgreSQL database, the name of the mode is displayed.
         self.schema_name = schema_name
+        # The name that is used for searching the database.
         self.search_name = search_name
+        # The system ID (SID) of the database.
+        # 
+        # > : The value of the parameter is returned only for Oracle databases.
         self.sid = sid
+        # The state of the database. Valid values:
+        # 
+        # *   **NORMAL**: The database is normal.
+        # *   **DISABLE**: The database is disabled.
+        # *   **OFFLINE**: The database is unpublished.
+        # *   **NOT_EXIST**: The database does not exist.
         self.state = state
 
     def validate(self):
         if self.owner_id_list:
             self.owner_id_list.validate()
         if self.owner_name_list:
             self.owner_name_list.validate()
@@ -16703,18 +18206,23 @@
         self,
         database: GetPhysicalDatabaseResponseBodyDatabase = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The information about the physical database.
         self.database = database
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.database:
             self.database.validate()
 
     def to_map(self):
@@ -16794,46 +18302,39 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GetProxyRequest(TeaModel):
     def __init__(
         self,
-        instance_id: int = None,
         proxy_id: int = None,
         tid: int = None,
     ):
-        # The ID of the database instance. You can call the [ListInstances](https://www.alibabacloud.com/help/en/data-management-service/latest/listinstances) or [GetInstance](https://www.alibabacloud.com/help/en/data-management-service/latest/getinstance) operation to query the database instance ID.
-        self.instance_id = instance_id
-        # The ID of the secure access proxy. You can call the [ListProxies](https://www.alibabacloud.com/help/en/data-management-service/latest/listproxies) operation to query the ID of the secure access proxy.
+        # The ID of the secure access proxy. You can call the [ListProxies](~~295371~~) operation to query the ID of the secure access proxy.
         self.proxy_id = proxy_id
-        # The ID of the tenant. You can call the [GetUserActiveTenant](https://www.alibabacloud.com/help/en/data-management-service/latest/getuseractivetenant) operation to query the tenant ID.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to obtain the tenant ID.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        if self.instance_id is not None:
-            result['InstanceId'] = self.instance_id
         if self.proxy_id is not None:
             result['ProxyId'] = self.proxy_id
         if self.tid is not None:
             result['Tid'] = self.tid
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        if m.get('InstanceId') is not None:
-            self.instance_id = m.get('InstanceId')
         if m.get('ProxyId') is not None:
             self.proxy_id = m.get('ProxyId')
         if m.get('Tid') is not None:
             self.tid = m.get('Tid')
         return self
 
 
@@ -16857,47 +18358,53 @@
         request_id: str = None,
         success: bool = None,
     ):
         # The ID of the user who enabled the secure access proxy feature.
         self.creator_id = creator_id
         # The nickname of the user who enabled the secure access proxy feature.
         self.creator_name = creator_name
-        # The error code returned.
+        # The error code returned if the request failed.
         self.error_code = error_code
-        # The error message returned.
+        # The error message returned if the request failed.
         self.error_message = error_message
-        # The port that was used by HTTPS clients to connect to the database instance.
+        # The port number used by the HTTPS protocol.
         self.https_port = https_port
-        # The ID of the database instance.
+        # The ID of the instance.
         self.instance_id = instance_id
-        # Indicates whether the internal endpoint is enabled. Default value: **true**.
+        # Indicates whether the internal endpoint was enabled. Default value: **true**.
         self.private_enable = private_enable
         # The internal endpoint.
         self.private_host = private_host
+        # The port number used by the protocol.
         self.protocol_port = protocol_port
+        # The protocol type of the database. Example: MYSQL.
         self.protocol_type = protocol_type
         # The ID of the secure access proxy.
         self.proxy_id = proxy_id
-        # Indicates whether the public endpoint is enabled. Valid values:
+        # Indicates whether the public endpoint was enabled. Valid values:
         # 
-        # - **true**: The public endpoint is enabled.
-        # - **false**: The public endpoint is disabled.
+        # *   **true**: The public endpoint was enabled.
+        # *   **false**: The public endpoint was disabled.
         self.public_enable = public_enable
-        # The public endpoint. A public endpoint is returned no matter whether the public endpoint is enabled or disabled.  
+        # The public endpoint. A public endpoint is returned no matter whether the public endpoint is enabled or disabled.
+        # 
+        # > 
         # 
-        # > - If the value of the PublicEnable parameter is **true**, a valid public endpoint that can be resolved by using Alibaba Cloud DNS (DNS) is returned.
-        # > - If the value of the PublicEnable parameter is **false**, an invalid public endpoint that cannot be resolved by using DNS is returned.
+        # *   If the value of the PublicEnable parameter is **true**, a valid public endpoint that can be resolved by using Alibaba Cloud DNS is returned.
+        # 
+        # *   If the value of the PublicEnable parameter is **false**, an invalid public endpoint that cannot be resolved by using Alibaba Cloud DNS is returned.
         self.public_host = public_host
+        # The ID of the region in which the instance resides.
         self.region_id = region_id
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
-        # - **true**: The request was successful.
-        # - **false**: The request failed.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17022,15 +18529,17 @@
 
 class GetProxyAccessRequest(TeaModel):
     def __init__(
         self,
         proxy_access_id: int = None,
         tid: int = None,
     ):
+        # The ID that Data Management (DMS) generates after the user is authorized to enable the secure access proxy feature for an instance. The ID is unique in DMS. You can call the [ListProxyAccesses](~~295386~~) operation to query the ID.
         self.proxy_access_id = proxy_access_id
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17063,23 +18572,38 @@
         origin_info: str = None,
         proxy_access_id: int = None,
         proxy_id: int = None,
         user_id: int = None,
         user_name: str = None,
         user_uid: str = None,
     ):
+        # The username of the database account that is authorized to enable the secure access proxy feature for an instance.
         self.access_id = access_id
+        # The time when the user is authorized to enable the secure access proxy feature for an instance.
         self.gmt_create = gmt_create
+        # The username of the independent database account.
         self.indep_account = indep_account
+        # The ID of the instance for which the secure access proxy feature is enabled.
         self.instance_id = instance_id
+        # The method that is used to authorize the user to enable the secure access proxy feature for an instance. Valid values:
+        # 
+        # *   **Authorization by the Alibaba Cloud Account ()**: The information in the parentheses () indicates the ID of the Alibaba Cloud account.
+        # *   **Authorization by submitting the ticket ()**:The information in the parentheses () indicates the number of the ticket that the user submits to apply for permissions.
         self.origin_info = origin_info
+        # The ID that DMS generates after the user is authorized to enable the secure access proxy feature for an instance. The ID is unique in DMS. You can call the [ListProxyAccesses](~~295386~~) operation to query the ID.
         self.proxy_access_id = proxy_access_id
+        # The ID of the secure access proxy.
+        # 
+        # >  You can call the [ListProxies](~~295371~~) operation to query the ID of the secure access proxy.
         self.proxy_id = proxy_id
+        # The ID of the user.
         self.user_id = user_id
+        # The nickname of the user.
         self.user_name = user_name
+        # The ID of the Alibaba Cloud account.
         self.user_uid = user_uid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17139,19 +18663,26 @@
         self,
         error_code: str = None,
         error_message: str = None,
         proxy_access: GetProxyAccessResponseBodyProxyAccess = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The authorization information about the secure access proxy feature.
         self.proxy_access = proxy_access
-        # Id of the request
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         if self.proxy_access:
             self.proxy_access.validate()
 
     def to_map(self):
@@ -18042,17 +19573,23 @@
     def __init__(
         self,
         order_id: int = None,
         page_number: int = None,
         page_size: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The number of the page to return.
         self.page_number = page_number
+        # The number of entries to return on each page.
         self.page_size = page_size
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18085,15 +19622,17 @@
 
 class GetStructSyncExecSqlDetailResponseBodyStructSyncExecSqlDetail(TeaModel):
     def __init__(
         self,
         exec_sql: str = None,
         total_sql_count: int = None,
     ):
+        # The SQL statements that are executed.
         self.exec_sql = exec_sql
+        # The total number of SQL statements.
         self.total_sql_count = total_sql_count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18121,19 +19660,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         struct_sync_exec_sql_detail: GetStructSyncExecSqlDetailResponseBodyStructSyncExecSqlDetail = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
-        # Id of the request
+        # The ID of the request.
         self.request_id = request_id
+        # The details of the SQL statements.
         self.struct_sync_exec_sql_detail = struct_sync_exec_sql_detail
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.struct_sync_exec_sql_detail:
             self.struct_sync_exec_sql_detail.validate()
 
     def to_map(self):
@@ -18219,18 +19762,31 @@
         self,
         compare_type: str = None,
         order_id: int = None,
         page_number: int = None,
         page_size: int = None,
         tid: int = None,
     ):
+        # The type of the comparison. Valid values:
+        # 
+        # *   **CREATE_TABLE**: compares the created tables.
+        # *   **ALTER_TABLE**: compares the modified tables.
+        # *   **EQUAL_TABLE**: compares the identical tables.
+        # *   **PASS_TABLE**: compares the tables that are skipped during schema synchronization.
+        # *   **NOT_COMPARE**: does not compare tables.
         self.compare_type = compare_type
+        # The ID of the ticket.
         self.order_id = order_id
+        # The number of the page to return.
         self.page_number = page_number
+        # The number of entries to return on each page.
         self.page_size = page_size
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18268,16 +19824,19 @@
 class GetStructSyncJobAnalyzeResultResponseBodyStructSyncJobAnalyzeResultResultList(TeaModel):
     def __init__(
         self,
         script: str = None,
         source_table_name: str = None,
         target_table_name: str = None,
     ):
+        # The SQL script.
         self.script = script
+        # The name of the source table.
         self.source_table_name = source_table_name
+        # The name of the destination table.
         self.target_table_name = target_table_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18306,15 +19865,23 @@
 
 class GetStructSyncJobAnalyzeResultResponseBodyStructSyncJobAnalyzeResultSummaryList(TeaModel):
     def __init__(
         self,
         compare_type: str = None,
         count: int = None,
     ):
+        # The type of the comparison. Valid values:
+        # 
+        # *   **CREATE_TABLE**: compares the created tables.
+        # *   **ALTER_TABLE**: compares the modified tables.
+        # *   **EQUAL_TABLE**: compares the identical tables.
+        # *   **PASS_TABLE**: compares the tables that are skipped during schema synchronization.
+        # *   **NOT_COMPARE**: does not compare tables.
         self.compare_type = compare_type
+        # The number of tables.
         self.count = count
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18339,15 +19906,17 @@
 
 class GetStructSyncJobAnalyzeResultResponseBodyStructSyncJobAnalyzeResult(TeaModel):
     def __init__(
         self,
         result_list: List[GetStructSyncJobAnalyzeResultResponseBodyStructSyncJobAnalyzeResultResultList] = None,
         summary_list: List[GetStructSyncJobAnalyzeResultResponseBodyStructSyncJobAnalyzeResultSummaryList] = None,
     ):
+        # The details of the analysis results.
         self.result_list = result_list
+        # The statistics on the analysis results.
         self.summary_list = summary_list
 
     def validate(self):
         if self.result_list:
             for k in self.result_list:
                 if k:
                     k.validate()
@@ -18392,18 +19961,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         struct_sync_job_analyze_result: GetStructSyncJobAnalyzeResultResponseBodyStructSyncJobAnalyzeResult = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # The analysis result of the schema synchronization task.
         self.struct_sync_job_analyze_result = struct_sync_job_analyze_result
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.struct_sync_job_analyze_result:
             self.struct_sync_job_analyze_result.validate()
 
     def to_map(self):
@@ -18716,15 +20290,19 @@
 
 class GetStructSyncOrderDetailRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18752,18 +20330,26 @@
         self,
         db_id: int = None,
         db_type: str = None,
         env_type: str = None,
         logic: bool = None,
         search_name: str = None,
     ):
+        # The ID of the source database.
         self.db_id = db_id
+        # The type of the database engine.
         self.db_type = db_type
+        # The type of the environment to which the database instance belongs. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # Indicates whether the database is a logical database. Valid values:
+        # 
+        # *   **true**: The database is a logical database.
+        # *   **false**: The database is not a logical database
         self.logic = logic
+        # The name that is used to search for the database.
         self.search_name = search_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18799,14 +20385,15 @@
 
 
 class GetStructSyncOrderDetailResponseBodyStructSyncOrderDetailSourceVersionInfo(TeaModel):
     def __init__(
         self,
         version_id: str = None,
     ):
+        # The version number.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18827,15 +20414,17 @@
 
 class GetStructSyncOrderDetailResponseBodyStructSyncOrderDetailTableInfoList(TeaModel):
     def __init__(
         self,
         source_table_name: str = None,
         target_table_name: str = None,
     ):
+        # The name of the table whose schema you want to synchronize.
         self.source_table_name = source_table_name
+        # The name of the table to which you want to synchronize the schema of a table.
         self.target_table_name = target_table_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18863,18 +20452,26 @@
         self,
         db_id: int = None,
         db_type: str = None,
         env_type: str = None,
         logic: bool = None,
         search_name: str = None,
     ):
+        # The ID of the destination database.
         self.db_id = db_id
+        # The type of the database engine.
         self.db_type = db_type
+        # The type of the environment to which the database instance belongs. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # Indicates whether the database is a logical database. Valid values:
+        # 
+        # *   **true**: The database is a logical database.
+        # *   **false**: The database is not a logical database
         self.logic = logic
+        # The name that is used to search for the database.
         self.search_name = search_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18910,14 +20507,15 @@
 
 
 class GetStructSyncOrderDetailResponseBodyStructSyncOrderDetailTargetVersionInfo(TeaModel):
     def __init__(
         self,
         version_id: str = None,
     ):
+        # The version number.
         self.version_id = version_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -18944,21 +20542,42 @@
         source_type: str = None,
         source_version_info: GetStructSyncOrderDetailResponseBodyStructSyncOrderDetailSourceVersionInfo = None,
         table_info_list: List[GetStructSyncOrderDetailResponseBodyStructSyncOrderDetailTableInfoList] = None,
         target_database_info: GetStructSyncOrderDetailResponseBodyStructSyncOrderDetailTargetDatabaseInfo = None,
         target_type: str = None,
         target_version_info: GetStructSyncOrderDetailResponseBodyStructSyncOrderDetailTargetVersionInfo = None,
     ):
+        # Indicates whether to skip errors. Valid values:
+        # 
+        # *   **true**: skips the error and continues to execute SQL statements.
+        # *   **false**: stops executing SQL statements.
         self.ignore_error = ignore_error
+        # The information about the source database.
         self.source_database_info = source_database_info
+        # The schema version of the source database. Valid values:
+        # 
+        # *   **DATASOURCE**: the default latest version of the system
+        # *   **VERSION**: a previous schema version that you manually specify
         self.source_type = source_type
+        # The version information about the source instance.
+        # 
+        # > This parameter is displayed only when the value of the **SourceType** parameter is **VERSION**.
         self.source_version_info = source_version_info
+        # The information about the table whose schema you want to synchronize.
         self.table_info_list = table_info_list
+        # The information about the destination database.
         self.target_database_info = target_database_info
+        # The schema version of the destination database. Valid values:
+        # 
+        # *   **DATASOURCE**: the default latest version of the system
+        # *   **VERSION**: a previous schema version that you manually specify
         self.target_type = target_type
+        # The version information about the destination instance.
+        # 
+        # > This parameter is displayed only when the value of the **SourceType** parameter is **VERSION**.
         self.target_version_info = target_version_info
 
     def validate(self):
         if self.source_database_info:
             self.source_database_info.validate()
         if self.source_version_info:
             self.source_version_info.validate()
@@ -19030,18 +20649,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         struct_sync_order_detail: GetStructSyncOrderDetailResponseBodyStructSyncOrderDetail = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # The details of the schema synchronization ticket.
         self.struct_sync_order_detail = struct_sync_order_detail
+        # Indicates whether the request was successful.
         self.success = success
 
     def validate(self):
         if self.struct_sync_order_detail:
             self.struct_sync_order_detail.validate()
 
     def to_map(self):
@@ -19124,15 +20748,25 @@
 
 class GetTableDBTopologyRequest(TeaModel):
     def __init__(
         self,
         table_guid: str = None,
         tid: int = None,
     ):
+        # The GUID of the table in DMS.
+        # 
+        # > 
+        # 
+        # *   If the database to which the table belongs is a logical database, you can call the [ListLogicTables](~~141875~~) operation to obtain the GUID. The value of the ReturnGuid parameter must be set to true.
+        # 
+        # *   If the database to which the table belongs is a physical database, you can call the [ListTables](~~141878~~) operation to obtain the GUID. The value of the ReturnGuid parameter must be set to true.
         self.table_guid = table_guid
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19158,16 +20792,19 @@
 class GetTableDBTopologyResponseBodyDBTopologyDataSourceListDatabaseListTableList(TeaModel):
     def __init__(
         self,
         table_id: str = None,
         table_name: str = None,
         table_type: str = None,
     ):
+        # The ID of the table.
         self.table_id = table_id
+        # The name of the physical table.
         self.table_name = table_name
+        # The type of the table. This is a reserved parameter.
         self.table_type = table_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19199,18 +20836,34 @@
         self,
         db_id: str = None,
         db_name: str = None,
         db_type: str = None,
         env_type: str = None,
         table_list: List[GetTableDBTopologyResponseBodyDBTopologyDataSourceListDatabaseListTableList] = None,
     ):
+        # The ID of the database.
         self.db_id = db_id
+        # The name of the database.
         self.db_name = db_name
+        # The type of the database. For more information about the valid values of this parameter, see [DbType parameter](~~198106~~).
         self.db_type = db_type
+        # The type of the environment to which the database belongs. Valid values:
+        # 
+        # *   **product**: production environment
+        # *   **dev**: development environment
+        # *   **pre**: pre-release environment
+        # *   **test**: test environment
+        # *   **sit**: system integration testing (SIT) environment
+        # *   **uat**: user acceptance testing (UAT) environment
+        # *   **pet**: stress testing environment
+        # *   **stag**: staging environment
+        # 
+        # > For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # The physical tables.
         self.table_list = table_list
 
     def validate(self):
         if self.table_list:
             for k in self.table_list:
                 if k:
                     k.validate()
@@ -19258,18 +20911,23 @@
         self,
         database_list: List[GetTableDBTopologyResponseBodyDBTopologyDataSourceListDatabaseList] = None,
         db_type: str = None,
         host: str = None,
         port: int = None,
         sid: str = None,
     ):
+        # The physical databases.
         self.database_list = database_list
+        # The type of the database. For more information about the valid values of this parameter, see [DbType parameter](~~198106~~).
         self.db_type = db_type
+        # The endpoint of the data source.
         self.host = host
+        # The port that is used to connect to the data source.
         self.port = port
+        # The system ID (SID) of the data source.
         self.sid = sid
 
     def validate(self):
         if self.database_list:
             for k in self.database_list:
                 if k:
                     k.validate()
@@ -19315,16 +20973,25 @@
 class GetTableDBTopologyResponseBodyDBTopology(TeaModel):
     def __init__(
         self,
         data_source_list: List[GetTableDBTopologyResponseBodyDBTopologyDataSourceList] = None,
         table_guid: str = None,
         table_name: str = None,
     ):
+        # The data sources.
         self.data_source_list = data_source_list
+        # The GUID of the table in DMS.
         self.table_guid = table_guid
+        # The name of the table.
+        # 
+        # > 
+        # 
+        # *   If a logical table is queried, the name of the logical table is returned.
+        # 
+        # *   If a physical table is queried, the name of the physical table is returned.
         self.table_name = table_name
 
     def validate(self):
         if self.data_source_list:
             for k in self.data_source_list:
                 if k:
                     k.validate()
@@ -19364,18 +21031,23 @@
         self,
         dbtopology: GetTableDBTopologyResponseBodyDBTopology = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The topology of the data table.
         self.dbtopology = dbtopology
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.dbtopology:
             self.dbtopology.validate()
 
     def to_map(self):
@@ -19458,15 +21130,25 @@
 
 class GetTableTopologyRequest(TeaModel):
     def __init__(
         self,
         table_guid: str = None,
         tid: int = None,
     ):
+        # The GUID of the table in Data Management (DMS).
+        # 
+        # > 
+        # 
+        # *   You can call the [ListLogicTables](~~141875~~) operation with ReturnGuid set to true to query the GUIDs of logical tables in a specific logical database.
+        # 
+        # *   You can call the [ListTables](~~141878~~) operation with ReturnGuid set to true to query the GUIDs of tables in a specific physical database.
         self.table_guid = table_guid
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the DMS console. For more information, see the "View information about the current tenant" section of the [Tenant information](~~181330~~) topic.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19500,24 +21182,53 @@
         instance_resource_id: str = None,
         instance_source: str = None,
         region_id: str = None,
         table_count: int = None,
         table_name_expr: str = None,
         table_name_list: str = None,
     ):
+        # The ID of the physical database.
         self.db_id = db_id
+        # The name of the database.
         self.db_name = db_name
+        # The name that is used to search for the database.
         self.db_search_name = db_search_name
+        # The database engine.
         self.db_type = db_type
+        # The ID of the instance to which the physical database belongs.
         self.instance_id = instance_id
+        # The ID of the resource related to the instance. The resource corresponds with the database instance type returned in the InstanceSource parameter.
+        # 
+        # *   **RDS**:The ID of the ApsaraDB RDS instance.
+        # *   **ECS_OWN**: The ID of the Elastic Compute Service (ECS) instance.
+        # *   **PUBLIC_OWN**: This parameter is left empty for self-managed database instances that are connected over the Internet.
+        # *   **VPC_ID**:The ID of the virtual private cloud (VPC).
+        # *   **GATEWAY**: The ID of the database gateway.
         self.instance_resource_id = instance_resource_id
+        # The type of the database instance. Valid values:
+        # 
+        # *   **RDS**: an ApsaraDB RDS instance.
+        # *   **ECS_OWN**: a self-managed database that is deployed on an ECS instance
+        # *   **PUBLIC_OWN**: a self-managed database instance that is connected over the Internet.
+        # *   **VPC_ID**: a self-managed database instance in a VPC that is connected over Express Connect circuits.
+        # *   **GATEWAY**: a database instance connected by using a database gateway.
         self.instance_source = instance_source
+        # The region ID of the instance.
         self.region_id = region_id
+        # The number of tables.
         self.table_count = table_count
+        # The expression of the names of logical tables.
+        # 
+        # **\
+        # 
+        # **Description**This parameter is not returned for physical tables.
         self.table_name_expr = table_name_expr
+        # The names of tables.
+        # 
+        # > The table names are separated by commas (,).
         self.table_name_list = table_name_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19580,17 +21291,24 @@
     def __init__(
         self,
         logic: bool = None,
         table_guid: str = None,
         table_name: str = None,
         table_topology_info_list: List[GetTableTopologyResponseBodyTableTopologyTableTopologyInfoList] = None,
     ):
+        # Indicates whether the table is a logical table. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
         self.logic = logic
+        # The GUID of the table in DMS.
         self.table_guid = table_guid
+        # The name of the table.
         self.table_name = table_name
+        # Information of the topology of the table.
         self.table_topology_info_list = table_topology_info_list
 
     def validate(self):
         if self.table_topology_info_list:
             for k in self.table_topology_info_list:
                 if k:
                     k.validate()
@@ -19634,18 +21352,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         table_topology: GetTableTopologyResponseBodyTableTopology = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
+        # The topology information.
         self.table_topology = table_topology
 
     def validate(self):
         if self.table_topology:
             self.table_topology.validate()
 
     def to_map(self):
@@ -20820,17 +22543,17 @@
 class GetUserRequest(TeaModel):
     def __init__(
         self,
         tid: int = None,
         uid: str = None,
         user_id: str = None,
     ):
-        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to query the ID of the tenant.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to obtain the tenant ID.
         self.tid = tid
-        # The UID of the user. You can view your UID by moving the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console.
+        # The UID of the Alibaba Cloud account. You can view your UID by moving the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console.
         self.uid = uid
         # The ID of the user. You can call the [ListUsers](~~141938~~) operation to query the ID of the user.
         self.user_id = user_id
 
     def validate(self):
         pass
 
@@ -20937,82 +22660,82 @@
     ):
         # The number of queries that are performed on the current day.
         self.cur_execute_count = cur_execute_count
         # The number of rows that are queried on the current day.
         self.cur_result_count = cur_result_count
         # The DingTalk chatbot URL that is used to receive notifications.
         # 
-        # > * The system returns this parameter if the user has set a DingTalk chatbot URL in the console. To set a DingTalk chatbot URL in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
-        # > * The system does not return this parameter if the user has not set a DingTalk chatbot URL.
+        # > 
+        # 
+        # *   The system returns this parameter if the user has set a DingTalk chatbot URL in the console. To set a DingTalk chatbot URL in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
+        # 
+        # *   The system does not return this parameter if the user has not set a DingTalk chatbot URL.
         self.ding_robot = ding_robot
         # The email address that is used to receive notifications.
         # 
-        # > * The system returns this parameter if the user has set an email address in the console. To set an email address in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
-        # > * The system does not return this parameter if the user has not set an email address.
+        # > 
+        # 
+        # *   The system returns this parameter if the user has set an email address in the console. To set an email address in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
+        # 
+        # *   The system does not return this parameter if the user has not set an email address.
         self.email = email
-        # The last time when the user logged on to the console.
+        # The last point in time when the user logged on to the console.
         self.last_login_time = last_login_time
         # The maximum number of queries that can be performed on the current day.
         self.max_execute_count = max_execute_count
         # The maximum number of rows that can be queried on the current day.
         self.max_result_count = max_result_count
-        # The mobile phone number that is used to receive notifications.
+        # The mobile number of the user.
+        # 
+        # > 
+        # 
+        # *   The system returns this parameter if the user has set a mobile phone number in the console. To set a mobile phone number in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
         # 
-        # > * The system returns this parameter if the user has set a mobile phone number in the console. To set a mobile phone number in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
-        # > * The system does not return this parameter if the user has not set a mobile phone number.
+        # *   The system does not return this parameter if the user has not set a mobile phone number.
         self.mobile = mobile
         # The nickname of the user.
         self.nick_name = nick_name
         # The notification method. The system returns one or more values. Valid values:
         # 
-        # *   **SMS**: text message.
+        # *   **SMS**: text message
         # *   **EMAIL**: email.
-        # *   **DingTalk**: DingTalk.
+        # *   **DINGDING**: DingTalk.
         # *   **DINGROBOT**: DingTalk chatbot.
         # *   **WEBHOOK**: webhook.
         self.notification_mode = notification_mode
         # The UID of the Alibaba Cloud account of the user.
         # 
-        # >  An Alibaba Cloud account can contain one or more RAM users.
+        # > An Alibaba Cloud account can contain one or more RAM users.
         self.parent_uid = parent_uid
-        # The ID of the role that is assigned to the user. Valid values:
-        # 
-        # *   **1**: a regular user role.
-        # *   **2**: a database administrator (DBA) role.
-        # *   **3**: a DMS administrator role.
-        # *   **4**: a security administrator role.
-        # *   **6**: a schema read-only user role.
+        # The list of role IDs.
         self.role_id_list = role_id_list
-        # The name of the role that is assigned to the user. Valid values:
-        # 
-        # *   **USER**: a regular user.
-        # *   **DBA** : a DBA.
-        # *   **ADMIN**: a DMS administrator.
-        # *   **SECURITY_ADMIN**: a security administrator.
-        # *   **STRUCT_READ_ONLY**: a schema read-only user.
+        # The list of role names.
         self.role_name_list = role_name_list
         # The signature method that is used to secure connections when a webhook URL is used. Valid values:
         # 
         # *   **NONE**: no signature.
-        # *   **HMAC\_SHA1**: HMAC_SHA1.
+        # *   **HMAC_SHA1**: HMAC_SHA1.
         self.signature_method = signature_method
         # The status of the user. Valid values:
         # 
         # *   **NORMAL**: The user is normal.
         # *   **DISABLE**: The user is disabled.
         # *   **DELETE**: The user is deleted.
         self.state = state
         # The UID of the user.
         self.uid = uid
         # The ID of the user.
         self.user_id = user_id
         # The webhook URL that is used to receive notifications.
         # 
-        # > * If the user has set a webhook URL, DMS sends notifications to the specified URL.
-        # > * The system does not return this parameter if the user has not set a webhook URL.
+        # > 
+        # 
+        # *   If the user has set a webhook URL, DMS sends notifications to the specified URL.
+        # 
+        # *   The system does not return this parameter if the user has not set a webhook URL.
         self.webhook = webhook
 
     def validate(self):
         if self.role_id_list:
             self.role_id_list.validate()
         if self.role_name_list:
             self.role_name_list.validate()
@@ -21109,24 +22832,24 @@
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         user: GetUserResponseBodyUser = None,
     ):
-        # The error code returned.
+        # The error code.
         self.error_code = error_code
-        # The error message returned.
+        # The error message returned if the request failed.
         self.error_message = error_message
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
         # *   **true**: The request was successful.
-        # *   **false**: The request failed.
+        # *   **false**: The request fails.
         self.success = success
         # The information about the user.
         self.user = user
 
     def validate(self):
         if self.user:
             self.user.validate()
@@ -21683,14 +23406,173 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetUserUploadFileJobResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GrantTemplateAuthorityRequest(TeaModel):
+    def __init__(
+        self,
+        comment: str = None,
+        expire_date: str = None,
+        template_id: int = None,
+        tid: int = None,
+        user_ids: str = None,
+    ):
+        # The reason why you want to grant permissions on resources to the users by using the permission template.
+        self.comment = comment
+        # The time when the permission expires. Specify the time in the yyyy-MM-DD HH:mm:ss format.
+        self.expire_date = expire_date
+        # The ID of the permission template.
+        self.template_id = template_id
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
+        self.tid = tid
+        # The IDs of users to which you want to grant permissions on resources by using the permission template.
+        self.user_ids = user_ids
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
+        if self.comment is not None:
+            result['Comment'] = self.comment
+        if self.expire_date is not None:
+            result['ExpireDate'] = self.expire_date
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        if self.user_ids is not None:
+            result['UserIds'] = self.user_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Comment') is not None:
+            self.comment = m.get('Comment')
+        if m.get('ExpireDate') is not None:
+            self.expire_date = m.get('ExpireDate')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        if m.get('UserIds') is not None:
+            self.user_ids = m.get('UserIds')
+        return self
+
+
+class GrantTemplateAuthorityResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        result: bool = None,
+        success: bool = None,
+    ):
+        # The error code.
+        self.error_code = error_code
+        # The error message returned if the request failed.
+        self.error_message = error_message
+        # The ID of the request.
+        self.request_id = request_id
+        # Indicates whether the permissions on resources were granted to the users by using the permission template.
+        self.result = result
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   true: The request was successful.
+        # *   false: The request failed.
+        self.success = success
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
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            self.result = m.get('Result')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class GrantTemplateAuthorityResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GrantTemplateAuthorityResponseBody = None,
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
+            temp_model = GrantTemplateAuthorityResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GrantUserPermissionRequest(TeaModel):
     def __init__(
         self,
         db_id: str = None,
         ds_type: str = None,
         expire_date: str = None,
         instance_id: int = None,
@@ -22281,59 +24163,59 @@
         default_value: str = None,
         description: str = None,
         function_type: str = None,
         nullable: bool = None,
         security_level: str = None,
         sensitive: bool = None,
     ):
-        # Indicates whether the field is an auto-increment field. Valid values:
+        # Indicates whether the column is an auto-increment column. Valid values:
         # 
-        # *   true: The field is an auto-increment field.
-        # *   false: The field is not an auto-increment field.
+        # *   true: The column is an auto-increment column.
+        # *   false: The column is not an auto-increment column.
         self.auto_increment = auto_increment
-        # The ID of the field.
+        # The ID of the column.
         self.column_id = column_id
-        # The name of the field.
+        # The name of the column.
         self.column_name = column_name
-        # The data type of the field.
+        # The data type of the column.
         self.column_type = column_type
         # The length of the field.
         self.data_length = data_length
         # The number of valid digits for the field.
         self.data_precision = data_precision
         # The number of decimal places for the field.
         self.data_scale = data_scale
-        # The default value of the field.
+        # The default value of the column.
         self.default_value = default_value
-        # The description of the field.
+        # The description of the column.
         self.description = description
         # The type of the masking algorithm that is used for the field. Valid values:
         # 
         # *   null: No masking algorithm is used.
         # *   DEFAULT: A full masking algorithm is used.
         # *   FIX_POS: The fixed position is masked.
         # *   FIX_CHAR: The fixed characters are replaced.
         self.function_type = function_type
-        # Indicates whether the field can be empty. Valid values:
+        # Indicates whether the column can be empty. Valid values:
         # 
-        # *   **true**: The field can be empty.
-        # *   **false**: The field cannot be empty.
+        # *   **true**: The column can be empty.
+        # *   **false**: The column cannot be empty.
         self.nullable = nullable
-        # The security level of the field. Valid values:
+        # The security level of the column. Valid values:
         # 
-        # *   INNER: The field is an internal field but not sensitive.
-        # *   SENSITIVE: The field is a sensitive field.
-        # *   CONFIDENTIAL: The field is a confidential field.
+        # *   INNER: The column is an internal column but not sensitive.
+        # *   SENSITIVE: The column is a sensitive column.
+        # *   CONFIDENTIAL: The column is a confidential column.
         # 
-        # >  For more information, see [Adjust the sensitivity level of one or more fields](~~66091~~).
+        # > For more information, see [Sensitivity levels of fields](~~66091~~).
         self.security_level = security_level
-        # Indicates whether the field is a sensitive field. Valid values:
+        # Indicates whether the column is a sensitive column. Valid values:
         # 
-        # *   **true**: The field is a sensitive field.
-        # *   **false**: The field is not a sensitive field.
+        # *   **true**: The column is a sensitive column.
+        # *   **false**: The column is not a sensitive column.
         self.sensitive = sensitive
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22440,26 +24322,26 @@
         self,
         column_list: ListColumnsResponseBodyColumnList = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
-        # The information about the columns returned.
+        # The details about columns.
         self.column_list = column_list
         # The error code returned.
         self.error_code = error_code
         # The error message returned.
         self.error_message = error_message
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
-        # - **true**: The request was successful.
-        # - **false**: The request failed.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         if self.column_list:
             self.column_list.validate()
 
     def to_map(self):
@@ -22803,17 +24685,23 @@
     def __init__(
         self,
         dbtask_group_id: int = None,
         page_number: int = None,
         page_size: int = None,
         tid: int = None,
     ):
+        # The ID of the SQL task group. You can call the [GetStructSyncJobDetail](~~206160~~) operation to obtain this parameter.
         self.dbtask_group_id = dbtask_group_id
+        # The number of the page to return.
         self.page_number = page_number
+        # The number of entries to return on each page.
         self.page_size = page_size
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22855,24 +24743,50 @@
         job_id: int = None,
         job_type: str = None,
         last_exec_time: str = None,
         logic: bool = None,
         status: str = None,
         transactional: bool = None,
     ):
+        # The description of the SQL task.
         self.comment = comment
+        # The time when the SQL task was created.
         self.create_time = create_time
+        # The ID of the database.
         self.db_id = db_id
+        # The name that is used to search for the database.
         self.db_search_name = db_search_name
+        # The ID of the SQL task group.
         self.db_task_group_id = db_task_group_id
+        # The ID of the SQL task.
         self.job_id = job_id
+        # The type of the SQL task.
         self.job_type = job_type
+        # The time when the SQL task was last executed.
         self.last_exec_time = last_exec_time
+        # Indicates whether the database is a logical database. Valid values:
+        # 
+        # *   **true**: The database is a logical database.
+        # *   **false**: The database is a logical database.
         self.logic = logic
+        # The state of the SQL task. Valid values:
+        # 
+        # *   **INIT**: The SQL task was initialized.
+        # *   **PENDING**: The SQL task waited to be run.
+        # *   **BE_SCHEDULED**: The SQL task waited to be scheduled.
+        # *   **FAIL**: The SQL task failed.
+        # *   **SUCCESS**: The SQL task was successful.
+        # *   **PAUSE**: The SQL task was paused.
+        # *   **DELETE**: The SQL task was deleted.
+        # *   **RUNNING**: The SQL task was being run.
         self.status = status
+        # Indicates whether the SQL task is executed as a transaction. Valid values:
+        # 
+        # *   **true**: The SQL task is executed as a transaction.
+        # *   **false**: The SQL task is not executed as a transaction.
         self.transactional = transactional
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22937,19 +24851,25 @@
         dbtask_sqljob_list: List[ListDBTaskSQLJobResponseBodyDBTaskSQLJobList] = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
+        # The list of the SQL tasks.
         self.dbtask_sqljob_list = dbtask_sqljob_list
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
+        # The total number of the SQL tasks.
         self.total_count = total_count
 
     def validate(self):
         if self.dbtask_sqljob_list:
             for k in self.dbtask_sqljob_list:
                 if k:
                     k.validate()
@@ -23343,15 +25263,21 @@
 
 class ListDDLPublishRecordsRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
+        # 
+        # > You can create a schema design ticket in the Data Management (DMS) console. For more information, see [Design schemas](~~69711~~). You can also call the [CreateOrder](~~144649~~) operation to create a schema design ticket and obtain the ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, log on to the DMS console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23380,19 +25306,29 @@
         dbtask_group_id: int = None,
         execute_count: int = None,
         scripts: str = None,
         status_desc: str = None,
         table_name: str = None,
         task_job_status: str = None,
     ):
+        # The ID of the SQL task group.
         self.dbtask_group_id = dbtask_group_id
+        # The number of SQL statements that are executed.
         self.execute_count = execute_count
+        # The script for data changes.
         self.scripts = scripts
+        # The description of the state.
         self.status_desc = status_desc
+        # The name of the table after the change.
         self.table_name = table_name
+        # The state of the publishing task. Valid values:
+        # 
+        # *   **NONE**: The state of the task is unknown.
+        # *   **SUCCESS**: The task is successful.
+        # *   **FAIL**: The task fails.
         self.task_job_status = task_job_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23438,20 +25374,33 @@
         logic: bool = None,
         plan_time: str = None,
         publish_job_list: List[ListDDLPublishRecordsResponseBodyDDLPublishRecordListPublishTaskInfoListPublishJobList] = None,
         publish_strategy: str = None,
         status_desc: str = None,
         task_job_status: str = None,
     ):
+        # The ID of the database.
         self.db_id = db_id
+        # Indicates whether the database is a logical database. Valid values:
+        # 
+        # *   **true**: The database is a logical database.
+        # *   **false**: the database is not a logical database.
         self.logic = logic
+        # The time to publish the ticket.
         self.plan_time = plan_time
+        # The list of the publishing tasks.
         self.publish_job_list = publish_job_list
+        # The publishing policy. Valid values:
+        # 
+        # *   **IMMEDIATELY**: immediately publishes the ticket.
+        # *   **REGULARLY**: publishes the ticket at a scheduled time.
         self.publish_strategy = publish_strategy
+        # The description of the state.
         self.status_desc = status_desc
+        # The state of the task.
         self.task_job_status = task_job_status
 
     def validate(self):
         if self.publish_job_list:
             for k in self.publish_job_list:
                 if k:
                     k.validate()
@@ -23512,23 +25461,55 @@
         finality_reason: str = None,
         publish_status: str = None,
         publish_task_info_list: List[ListDDLPublishRecordsResponseBodyDDLPublishRecordListPublishTaskInfoList] = None,
         risk_level: str = None,
         status_desc: str = None,
         workflow_instance_id: int = None,
     ):
+        # The time when the approval expires.
         self.audit_expire_time = audit_expire_time
+        # The approval state of the ticket. Valid values:
+        # 
+        # *   **EXEMPT_PASS**: The ticket passes without approval.
+        # *   **TO_AUDIT**: The ticket is pending for approval.
+        # *   **CANCEL**: The ticket is canceled.
+        # *   **SUCCESS**: The ticket is approved.
+        # *   **FAIL**: The ticket fails to pass the approval.
         self.audit_status = audit_status
+        # The ID of the user who creates the ticket. You can obtain the user ID by calling the [GetUser](~~147098~~) operation and querying the value of the UserId parameter. The value is not the unique ID (UID) of the Alibaba Cloud account.
         self.creator_id = creator_id
+        # Indicates whether the approval is terminated. Valid values:
+        # 
+        # *   **true**: The approval is terminated.
+        # *   **false**: The approval is not terminated.
+        # 
+        # > Multiple reasons can terminate the approval. For example, you withdraw the application or your ticket is not approved before the specified time.
         self.finality = finality
+        # The reason for the termination.
         self.finality_reason = finality_reason
+        # The publishing state of the ticket. Valid values:
+        # 
+        # *   **START**: The ticket is created.
+        # *   **ANALYZE**: The ticket is under analysis.
+        # *   **AUDIT**: The ticket is under approval.
+        # *   **DISPATCH**: A task is generated for the ticket.
+        # *   **SUCCESS**: The task is successful.
         self.publish_status = publish_status
+        # The list of publishing tasks.
         self.publish_task_info_list = publish_task_info_list
+        # The risk level of the operation. Valid values:
+        # 
+        # *   **NONE_RISK**: The operation does not have risks.
+        # *   **LOW_RISK**: The operation is at low risk.
+        # *   **MIDDLE_RISK**: The operation is at medium risk.
+        # *   **HIGH_RISK**: The operation is at high risk.
         self.risk_level = risk_level
+        # The description of the publishing state.
         self.status_desc = status_desc
+        # The ID of the approval process.
         self.workflow_instance_id = workflow_instance_id
 
     def validate(self):
         if self.publish_task_info_list:
             for k in self.publish_task_info_list:
                 if k:
                     k.validate()
@@ -23596,18 +25577,23 @@
         self,
         ddlpublish_record_list: List[ListDDLPublishRecordsResponseBodyDDLPublishRecordList] = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The details of the publishing records.
         self.ddlpublish_record_list = ddlpublish_record_list
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.ddlpublish_record_list:
             for k in self.ddlpublish_record_list:
                 if k:
                     k.validate()
@@ -24139,31 +26125,383 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListDataCorrectPreCheckSQLResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListDataImportSQLPreCheckDetailRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        page_numer: int = None,
+        page_size: int = None,
+        sql_type: str = None,
+        status_code: str = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.page_numer = page_numer
+        self.page_size = page_size
+        self.sql_type = sql_type
+        self.status_code = status_code
+        self.tid = tid
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
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.page_numer is not None:
+            result['PageNumer'] = self.page_numer
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.sql_type is not None:
+            result['SqlType'] = self.sql_type
+        if self.status_code is not None:
+            result['StatusCode'] = self.status_code
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('PageNumer') is not None:
+            self.page_numer = m.get('PageNumer')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('SqlType') is not None:
+            self.sql_type = m.get('SqlType')
+        if m.get('StatusCode') is not None:
+            self.status_code = m.get('StatusCode')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class ListDataImportSQLPreCheckDetailResponseBodyPreCheckSQLDetailList(TeaModel):
+    def __init__(
+        self,
+        skip: bool = None,
+        sql_id: int = None,
+        sql_type: str = None,
+        status_code: str = None,
+    ):
+        self.skip = skip
+        self.sql_id = sql_id
+        self.sql_type = sql_type
+        self.status_code = status_code
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
+        if self.skip is not None:
+            result['Skip'] = self.skip
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_type is not None:
+            result['SqlType'] = self.sql_type
+        if self.status_code is not None:
+            result['StatusCode'] = self.status_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Skip') is not None:
+            self.skip = m.get('Skip')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlType') is not None:
+            self.sql_type = m.get('SqlType')
+        if m.get('StatusCode') is not None:
+            self.status_code = m.get('StatusCode')
+        return self
+
+
+class ListDataImportSQLPreCheckDetailResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        pre_check_sqldetail_list: List[ListDataImportSQLPreCheckDetailResponseBodyPreCheckSQLDetailList] = None,
+        request_id: str = None,
+        success: bool = None,
+        total_count: int = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.pre_check_sqldetail_list = pre_check_sqldetail_list
+        self.request_id = request_id
+        self.success = success
+        self.total_count = total_count
+
+    def validate(self):
+        if self.pre_check_sqldetail_list:
+            for k in self.pre_check_sqldetail_list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        result['PreCheckSQLDetailList'] = []
+        if self.pre_check_sqldetail_list is not None:
+            for k in self.pre_check_sqldetail_list:
+                result['PreCheckSQLDetailList'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        self.pre_check_sqldetail_list = []
+        if m.get('PreCheckSQLDetailList') is not None:
+            for k in m.get('PreCheckSQLDetailList'):
+                temp_model = ListDataImportSQLPreCheckDetailResponseBodyPreCheckSQLDetailList()
+                self.pre_check_sqldetail_list.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListDataImportSQLPreCheckDetailResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListDataImportSQLPreCheckDetailResponseBody = None,
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
+            temp_model = ListDataImportSQLPreCheckDetailResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class ListDataImportSQLTypeRequest(TeaModel):
+    def __init__(
+        self,
+        order_id: int = None,
+        tid: int = None,
+    ):
+        self.order_id = order_id
+        self.tid = tid
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
+        if self.order_id is not None:
+            result['OrderId'] = self.order_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OrderId') is not None:
+            self.order_id = m.get('OrderId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class ListDataImportSQLTypeResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        sql_type_result: List[str] = None,
+        success: bool = None,
+    ):
+        self.error_code = error_code
+        self.error_message = error_message
+        self.request_id = request_id
+        self.sql_type_result = sql_type_result
+        self.success = success
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
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.sql_type_result is not None:
+            result['SqlTypeResult'] = self.sql_type_result
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SqlTypeResult') is not None:
+            self.sql_type_result = m.get('SqlTypeResult')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class ListDataImportSQLTypeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListDataImportSQLTypeResponseBody = None,
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
+            temp_model = ListDataImportSQLTypeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListDatabaseUserPermssionsRequest(TeaModel):
     def __init__(
         self,
         db_id: str = None,
         logic: bool = None,
         page_number: int = None,
         page_size: int = None,
         perm_type: str = None,
         tid: int = None,
         user_name: str = None,
     ):
+        # The ID of the database.
         self.db_id = db_id
+        # Specifies whether the database is a logical database.
         self.logic = logic
+        # The number of the page to return.
         self.page_number = page_number
+        # The number of entries to return on each page.
         self.page_size = page_size
+        # The type of the permission. Valid values:
+        # 
+        # *   DATABASE: permissions on databases
+        # *   TABLE: permissions on tables
+        # *   COLUMN: permissions on fields
         self.perm_type = perm_type
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
+        # The nickname of the user.
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24212,19 +26550,29 @@
         create_date: str = None,
         expire_date: str = None,
         extra_data: str = None,
         origin_from: str = None,
         perm_type: str = None,
         user_access_id: str = None,
     ):
+        # The time when the permission was created.
         self.create_date = create_date
+        # The time when the permissions expire.
         self.expire_date = expire_date
+        # The extra information. This parameter is reserved.
         self.extra_data = extra_data
+        # The description of the entity that authorizes the permission.
         self.origin_from = origin_from
+        # The type of the permission. Valid values:
+        # 
+        # *   QUERY: the query permissions
+        # *   EXPORT: the export permissions
+        # *   CORRECT: the change permissions
         self.perm_type = perm_type
+        # The ID of the authorization record.
         self.user_access_id = user_access_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24313,28 +26661,43 @@
         schema_name: str = None,
         search_name: str = None,
         table_id: str = None,
         table_name: str = None,
         user_id: str = None,
         user_nick_name: str = None,
     ):
+        # The alias of the database instance.
         self.alias = alias
+        # The name of a column.
         self.column_name = column_name
+        # The ID of the database.
         self.db_id = db_id
+        # The type of the database engine.
         self.db_type = db_type
+        # The type of resources on which the user has permissions.
         self.ds_type = ds_type
+        # The type of the environment to which the database belongs.
         self.env_type = env_type
+        # The ID of the instance.
         self.instance_id = instance_id
+        # Indicates whether the database is a logical database.
         self.logic = logic
+        # The details of user permissions.
         self.perm_details = perm_details
+        # The name of the database.
         self.schema_name = schema_name
+        # The name that is used to search for the database.
         self.search_name = search_name
+        # The ID of the table.
         self.table_id = table_id
+        # The name of the table.
         self.table_name = table_name
+        # The ID of the user.
         self.user_id = user_id
+        # The nickname of the user.
         self.user_nick_name = user_nick_name
 
     def validate(self):
         if self.perm_details:
             self.perm_details.validate()
 
     def to_map(self):
@@ -24452,19 +26815,25 @@
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
         user_permissions: ListDatabaseUserPermssionsResponseBodyUserPermissions = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
+        # The total number of entries returned.
         self.total_count = total_count
+        # The details of user permissions.
         self.user_permissions = user_permissions
 
     def validate(self):
         if self.user_permissions:
             self.user_permissions.validate()
 
     def to_map(self):
@@ -24553,17 +26922,23 @@
     def __init__(
         self,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
         tid: int = None,
     ):
+        # The ID of the instance. The valid value is returned if you call the ListInstances operation. The instance ID is not the ID of the RDS instance.
         self.instance_id = instance_id
+        # The number of the page to return.
         self.page_number = page_number
+        # The number of entries to return per page.
         self.page_size = page_size
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -24664,29 +27039,50 @@
         owner_name_list: ListDatabasesResponseBodyDatabaseListDatabaseOwnerNameList = None,
         port: int = None,
         schema_name: str = None,
         search_name: str = None,
         sid: str = None,
         state: str = None,
     ):
+        # The name of the catalog to which the database belongs.
         self.catalog_name = catalog_name
+        # The ID of the database.
         self.database_id = database_id
+        # The type of the database engine.
         self.db_type = db_type
+        # The ID of the DBA.
         self.dba_id = dba_id
+        # The nickname of the Database administrator (DBA) to which the database belongs.
         self.dba_name = dba_name
+        # The encoding format of the database.
         self.encoding = encoding
+        # The type of the environment to which the database belongs.
         self.env_type = env_type
+        # The endpoint of the instance to which the database belongs.
         self.host = host
+        # The ID of the instance to which the database belongs.
         self.instance_id = instance_id
+        # The IDs of the owners of the database.
         self.owner_id_list = owner_id_list
+        # The nicknames of the database owners.
         self.owner_name_list = owner_name_list
+        # The connection port of the instance to which the database belongs.
         self.port = port
+        # The name of the database.
         self.schema_name = schema_name
+        # The name that is used for searching the database.
         self.search_name = search_name
+        # The system ID (SID) of the instance to which the database belongs.
         self.sid = sid
+        # The state of the database. Valid values:
+        # 
+        # *   NORMAL: The database is normal.
+        # *   DISABLE: The database is disabled.
+        # *   OFFLINE: The database is unpublished.
+        # *   NOT_EXIST: The database does not exist.
         self.state = state
 
     def validate(self):
         if self.owner_id_list:
             self.owner_id_list.validate()
         if self.owner_name_list:
             self.owner_name_list.validate()
@@ -24811,19 +27207,25 @@
         database_list: ListDatabasesResponseBodyDatabaseList = None,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
+        # The details of the databases.
         self.database_list = database_list
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
+        # The number of databases that belong to an instance.
         self.total_count = total_count
 
     def validate(self):
         if self.database_list:
             self.database_list.validate()
 
     def to_map(self):
@@ -25705,16 +28107,21 @@
 class ListIndexesRequest(TeaModel):
     def __init__(
         self,
         logic: bool = None,
         table_id: str = None,
         tid: int = None,
     ):
+        # Specifies whether the table is a logical table.
         self.logic = logic
+        # The ID of the table.
         self.table_id = table_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25746,18 +28153,29 @@
         self,
         index_comment: str = None,
         index_id: str = None,
         index_name: str = None,
         index_type: str = None,
         table_id: str = None,
     ):
+        # The description of the index.
         self.index_comment = index_comment
+        # The ID of the index.
         self.index_id = index_id
+        # The name of the index.
         self.index_name = index_name
+        # The type of the index. Valid values:
+        # 
+        # *   Primary
+        # *   Unique
+        # *   Normal
+        # *   FullText
+        # *   Spatial
         self.index_type = index_type
+        # The ID of the table.
         self.table_id = table_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -25832,18 +28250,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         index_list: ListIndexesResponseBodyIndexList = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The details of indexes.
         self.index_list = index_list
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         if self.index_list:
             self.index_list.validate()
 
     def to_map(self):
@@ -28380,19 +30803,27 @@
         database_id: str = None,
         page_number: int = None,
         page_size: int = None,
         return_guid: bool = None,
         search_name: str = None,
         tid: int = None,
     ):
+        # The ID of the logical database.
         self.database_id = database_id
+        # The number of the page to return.
         self.page_number = page_number
+        # The number of entries to return on each page.
         self.page_size = page_size
+        # Specifies whether to return the GUID of the table.
         self.return_guid = return_guid
+        # The keyword that is used to search for the logical tables. Prefix match is supported.
         self.search_name = search_name
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28495,23 +30926,33 @@
         schema_name: str = None,
         table_count: str = None,
         table_expr: str = None,
         table_guid: str = None,
         table_id: str = None,
         table_name: str = None,
     ):
+        # The ID of the logical database.
         self.database_id = database_id
+        # Indicates whether the table is a logical table. The value is fixed to true.
         self.logic = logic
+        # The IDs of the owners of the logical tables.
         self.owner_id_list = owner_id_list
+        # The nicknames of the owners of the logical tables.
         self.owner_name_list = owner_name_list
+        # The logical database to which the logical table belongs.
         self.schema_name = schema_name
+        # The number of logical tables.
         self.table_count = table_count
+        # The expression of the logical table.
         self.table_expr = table_expr
+        # The GUID of the logical table.
         self.table_guid = table_guid
+        # The ID of the logical table.
         self.table_id = table_id
+        # The name of the logical table.
         self.table_name = table_name
 
     def validate(self):
         if self.owner_id_list:
             self.owner_id_list.validate()
         if self.owner_name_list:
             self.owner_name_list.validate()
@@ -28612,19 +31053,25 @@
         error_code: str = None,
         error_message: str = None,
         logic_table_list: ListLogicTablesResponseBodyLogicTableList = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The details of the logical tables.
         self.logic_table_list = logic_table_list
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
+        # The total number of logical tables that meet the query conditions.
         self.total_count = total_count
 
     def validate(self):
         if self.logic_table_list:
             self.logic_table_list.validate()
 
     def to_map(self):
@@ -29054,15 +31501,15 @@
 
 
 class ListProxiesRequest(TeaModel):
     def __init__(
         self,
         tid: int = None,
     ):
-        # The ID of the tenant. You can call the [GetUserActiveTenant](https://www.alibabacloud.com/help/en/data-management-service/latest/getuseractivetenant) operation to query the tenant ID.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to query the tenant ID.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29097,36 +31544,42 @@
         public_host: str = None,
         region_id: str = None,
     ):
         # The ID of the user who enabled the secure access proxy feature.
         self.creator_id = creator_id
         # The nickname of the user who enabled the secure access proxy feature.
         self.creator_name = creator_name
-        # The port that was used by HTTPS clients to connect to the database instance.
+        # The number of the port that was used by HTTPS clients to connect to the database instance.
         self.https_port = https_port
-        # The ID of the database instance.
+        # The ID of the instance.
         self.instance_id = instance_id
         # Indicates whether the internal endpoint is enabled. Default value: **true**.
         self.private_enable = private_enable
         # The internal endpoint.
         self.private_host = private_host
+        # The number of the port that is used to connect the database instance.
         self.protocol_port = protocol_port
+        # The type of the database. Example: MYSQL.
         self.protocol_type = protocol_type
         # The ID of the secure access proxy.
         self.proxy_id = proxy_id
         # Indicates whether the public endpoint is enabled. Valid values:
         # 
-        # - **true**: The public endpoint is enabled.
-        # - **false**: The public endpoint is disabled.
+        # *   **true**: The public endpoint is enabled.
+        # *   **false**: The public endpoint is disabled.
         self.public_enable = public_enable
-        # The public endpoint. A public endpoint is returned no matter whether the public endpoint is enabled or disabled.  
+        # The public endpoint. A public endpoint is returned no matter whether the public endpoint is enabled or disabled.
         # 
-        # > - If the value of the PublicEnable parameter is **true**, a valid public endpoint that can be resolved by using Alibaba Cloud DNS (DNS) is returned.
-        # > - If the value of the PublicEnable parameter is **false**, an invalid public endpoint that cannot be resolved by using DNS is returned.
+        # > 
+        # 
+        # *   If the value of the PublicEnable parameter is **true**, a valid public endpoint that can be resolved by using Alibaba Cloud DNS (DNS) is returned.
+        # 
+        # *   If the value of the PublicEnable parameter is **false**, an invalid public endpoint that cannot be resolved by using DNS is returned.
         self.public_host = public_host
+        # The ID of the region.
         self.region_id = region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29194,26 +31647,26 @@
         self,
         error_code: str = None,
         error_message: str = None,
         proxy_list: List[ListProxiesResponseBodyProxyList] = None,
         request_id: str = None,
         success: bool = None,
     ):
-        # The error code returned.
+        # The error code.
         self.error_code = error_code
-        # The error message returned.
+        # The error message.
         self.error_message = error_message
-        # An array that consists of secure access proxies.
+        # The proxies that are generated by the secure access proxy feature.
         self.proxy_list = proxy_list
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
-        # - **true**: The request was successful.
-        # - **false**: The request failed.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
 
     def validate(self):
         if self.proxy_list:
             for k in self.proxy_list:
                 if k:
                     k.validate()
@@ -32343,15 +34796,15 @@
         # Specifies whether to return the GUID of a table. Valid values:
         # 
         # *   **true**: returns the GUID of a table.
         # *   **false**: does not return the GUID of a table.
         self.return_guid = return_guid
         # The name used to search for tables. Fuzzy search is supported.
         self.search_name = search_name
-        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to obtain the tenant ID.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32467,25 +34920,25 @@
         self.description = description
         # The encoding format of the table.
         self.encoding = encoding
         # The engine of the table.
         self.engine = engine
         # The number of rows in the table. This is a statistical value and does not indicate the actual number of rows.
         self.num_rows = num_rows
-        # The IDs of the owners of the table.
+        # The ID list of the table owners.
         self.owner_id_list = owner_id_list
-        # The nicknames of the owners of the table.
+        # The nickname list of the table owners.
         self.owner_name_list = owner_name_list
         # The storage space that is occupied by the table. This is a statistical value and does not indicate the accurate storage space. Unit: MB.
         self.store_capacity = store_capacity
         # The GUID of the table in DMS.
         self.table_guid = table_guid
         # The ID of the table.
         self.table_id = table_id
-        # The name of the table.
+        # The table name.
         self.table_name = table_name
         # The database in which the table resides.
         self.table_schema_name = table_schema_name
         # The type of the table. Default value: NORMAL.
         self.table_type = table_type
 
     def validate(self):
@@ -32602,24 +35055,24 @@
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         table_list: ListTablesResponseBodyTableList = None,
         total_count: int = None,
     ):
-        # The error code that is returned if the request fails.
+        # The error code returned.
         self.error_code = error_code
-        # The error message returned if the request fails.
+        # The error message returned.
         self.error_message = error_message
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
-        # - **true**: The request was successful.
-        # - **false**: The request failed.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
         # The details of the tables.
         self.table_list = table_list
         # The total number of tables that meet the query conditions.
         self.total_count = total_count
 
     def validate(self):
@@ -35442,29 +37895,31 @@
         tid: int = None,
         user_state: str = None,
     ):
         # The number of the page to return.
         self.page_number = page_number
         # The number of entries to return on each page.
         # 
-        # >  Valid values: 10, 20, 50, and 100. Default value: 10.
+        # **\
+        # 
+        # Valid values: 10, 20, 50, and 100.**** Default value: 10.
         self.page_size = page_size
         # The role that is assigned to the user. Valid values:
         # 
-        # *   **USER**: a regular user role.
-        # *   **DBA**: a database administrator (DBA) role.
-        # *   **ADMIN**: a Data Management (DMS) administrator role.
-        # *   **SECURITY_ADMIN**: a security administrator role.
-        # *   **STRUCT\_READ\_ONLY**: a schema read-only user role.
+        # *   **USER**: a regular user.
+        # *   **DBA** : a database administrator (DBA).
+        # *   **ADMIN**: a Data Management (DMS) administrator.
+        # *   **SECURITY_ADMIN**: a security administrator.
+        # *   **STRUCT_READ_ONLY**: a schema read-only user.
         # 
         # >  To check your role, move the pointer over the profile picture in the upper-right corner of the DMS console.
         self.role = role
         # The search keyword. Fuzzy match is supported.
         self.search_key = search_key
-        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to query the ID of the tenant.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to obtain the tenant ID.
         self.tid = tid
         # The status of the user. Valid values:
         # 
         # *   **NORMAL**: The user is normal.
         # *   **DISABLE**: The user is disabled.
         # *   **DELETE**: The user is deleted.
         self.user_state = user_state
@@ -35581,86 +38036,86 @@
         role_name_list: ListUsersResponseBodyUserListUserRoleNameList = None,
         signature_method: str = None,
         state: str = None,
         uid: str = None,
         user_id: str = None,
         webhook: str = None,
     ):
-        # The number of queries that are performed on the current day.
+        # The number of queries that were performed on the current day.
         self.cur_execute_count = cur_execute_count
-        # The number of rows that are queried on the current day.
+        # The number of rows that were queried on the current day.
         self.cur_result_count = cur_result_count
         # The DingTalk chatbot URL that is used to receive notifications.
         # 
-        # > * The system returns this parameter if the user has set a DingTalk chatbot URL in the console. To set a DingTalk chatbot URL in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
-        # > * The system does not return this parameter if the user has not set a DingTalk chatbot URL.
+        # > 
+        # 
+        # *   The system returns this parameter if you have set a DingTalk chatbot URL in the console. To set a DingTalk chatbot URL in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
+        # 
+        # *   The system does not return this parameter if you have not set a DingTalk chatbot URL.
         self.ding_robot = ding_robot
         # The email address that is used to receive notifications.
         # 
-        # > * The system returns this parameter if the user has set an email address in the console. To set an email address in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
-        # > * The system does not return this parameter if the user has not set an email address.
+        # > 
+        # 
+        # *   The system returns this parameter if you have set an email address in the console. To set an email address in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
+        # 
+        # *   The system does not return this parameter if you have not set an email address.
         self.email = email
-        # The last time when the user logged on to the console.
+        # The time when the user last logged on to the console.
         self.last_login_time = last_login_time
         # The maximum number of queries that can be performed on the current day.
         self.max_execute_count = max_execute_count
         # The maximum number of rows that can be queried on the current day.
         self.max_result_count = max_result_count
-        # The mobile phone number that is used to receive notifications.
+        # The mobile phone number of the user.
+        # 
+        # > 
         # 
-        # > * The system returns this parameter if the user has set a mobile phone number in the console. To set a mobile phone number in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
-        # > * The system does not return this parameter if the user has not set a mobile phone number.
+        # *   The system returns this parameter if you have set a mobile phone number in the console. To set a mobile phone number in the console, move the pointer over the profile picture in the upper-right corner and click the Edit icon next to **Notice**.
+        # 
+        # *   The system does not return this parameter if you have not set a mobile phone number.
         self.mobile = mobile
         # The nickname of the user.
         self.nick_name = nick_name
         # The notification method. The system returns one or more values. Valid values:
         # 
-        # *   **SMS**: text message.
+        # *   **SMS**: text message
         # *   **EMAIL**: email.
-        # *   **DingTalk**: DingTalk.
+        # *   **DINGDING**: DingTalk.
         # *   **DINGROBOT**: DingTalk chatbot.
         # *   **WEBHOOK**: webhook.
         self.notification_mode = notification_mode
-        # The UID of the Alibaba Cloud account of the user.
+        # The ID of the Alibaba Cloud account of the user.
         self.parent_uid = parent_uid
-        # The ID of the role that is assigned to the user. Valid values:
-        # 
-        # *   **1**: a regular user role.
-        # *   **2**: a DBA role.
-        # *   **3**: a DMS administrator role.
-        # *   **4**: a security administrator role.
-        # *   **6**: a schema read-only user role.
+        # The IDs of the roles.
         self.role_id_list = role_id_list
-        # The name of the role that is assigned to the user. Valid values:
-        # 
-        # *   **USER**: a regular user.
-        # *   **DBA**: a DBA.
-        # *   **ADMIN**: a DMS administrator.
-        # *   **SECURITY_ADMIN**: a security administrator.
-        # *   **STRUCT\_READ\_ONLY**: a schema read-only user.
+        # The names of roles.
         self.role_name_list = role_name_list
         # The signature method that is used to secure connections when a webhook URL is used. Valid values:
         # 
         # *   **NONE**: no signature.
-        # *   **HMAC_SHA1**: HMAC-SHA1.
+        # *   **HMAC_SHA1**: HMAC_SHA1.
         self.signature_method = signature_method
         # The status of the user. Valid values:
         # 
         # *   **NORMAL**: The user is normal.
         # *   **DISABLE**: The user is disabled.
         # *   **DELETE**: The user is deleted.
         self.state = state
-        # The UID of the user.
+        # The ID of the Alibaba Cloud account.
         self.uid = uid
         # The ID of the user.
         self.user_id = user_id
         # The webhook URL that is used to receive notifications.
         # 
-        # > * If the user has set a webhook URL, DMS sends notifications to the specified URL.
-        # > * The system does not return this parameter if the user has not set a webhook URL.
+        # > 
+        # 
+        # *   If you have set a webhook URL, DMS sends notifications to the specified URL.
+        # 
+        # *   The system does not return this parameter if you have not set a webhook URL.
         self.webhook = webhook
 
     def validate(self):
         if self.role_id_list:
             self.role_id_list.validate()
         if self.role_name_list:
             self.role_name_list.validate()
@@ -35793,24 +38248,24 @@
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         total_count: int = None,
         user_list: ListUsersResponseBodyUserList = None,
     ):
-        # The error code returned.
+        # The error code returned if the request failed.
         self.error_code = error_code
-        # The error message returned.
+        # The error message returned if the request failed.
         self.error_message = error_message
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
-        # - **true**: The request was successful.
-        # - **false**: The request failed.
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
         self.success = success
         # The total number of entries returned.
         self.total_count = total_count
         # The details of users.
         self.user_list = user_list
 
     def validate(self):
@@ -35901,15 +38356,19 @@
 
 class ListWorkFlowNodesRequest(TeaModel):
     def __init__(
         self,
         search_name: str = None,
         tid: int = None,
     ):
+        # The name that is used to search for approval nodes.
         self.search_name = search_name
+        # The ID of the tenant.
+        # 
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -35935,16 +38394,19 @@
 class ListWorkFlowNodesResponseBodyWorkflowNodesWorkflowNodeAuditUsersAuditUser(TeaModel):
     def __init__(
         self,
         nick_name: str = None,
         real_name: str = None,
         user_id: int = None,
     ):
+        # The nickname of the approver.
         self.nick_name = nick_name
+        # The real name of the approver.
         self.real_name = real_name
+        # The ID of the approver. The ID is different from the ID of the Alibaba Cloud account of the approver.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -36013,20 +38475,30 @@
         comment: str = None,
         create_user_id: int = None,
         create_user_nick_name: str = None,
         node_id: int = None,
         node_name: str = None,
         node_type: str = None,
     ):
+        # The details about approvers.
         self.audit_users = audit_users
+        # The description of the approval template.
         self.comment = comment
+        # The ID of the creator. This ID is different from the ID of the Alibaba Cloud account of the creator.
         self.create_user_id = create_user_id
+        # The name of the user who creates the approval node.
         self.create_user_nick_name = create_user_nick_name
+        # The ID of the approval node.
         self.node_id = node_id
+        # The name of the approval node.
         self.node_name = node_name
+        # The type of the approval node. Valid values:
+        # 
+        # *   SYS: The approval node is predefined by the system.
+        # *   USER_LIST: The approval node is created by a user.
         self.node_type = node_type
 
     def validate(self):
         if self.audit_users:
             self.audit_users.validate()
 
     def to_map(self):
@@ -36111,18 +38583,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         workflow_nodes: ListWorkFlowNodesResponseBodyWorkflowNodes = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
+        # The details of approval nodes.
         self.workflow_nodes = workflow_nodes
 
     def validate(self):
         if self.workflow_nodes:
             self.workflow_nodes.validate()
 
     def to_map(self):
@@ -38949,14 +41426,159 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = RetryDataCorrectPreCheckResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class RevokeTemplateAuthorityRequest(TeaModel):
+    def __init__(
+        self,
+        template_id: int = None,
+        tid: int = None,
+        user_ids: str = None,
+    ):
+        # The ID of the permission template.
+        self.template_id = template_id
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
+        self.tid = tid
+        # The IDs of users from whom you want to revoke permissions by using a permission template.
+        self.user_ids = user_ids
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
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        if self.user_ids is not None:
+            result['UserIds'] = self.user_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        if m.get('UserIds') is not None:
+            self.user_ids = m.get('UserIds')
+        return self
+
+
+class RevokeTemplateAuthorityResponseBody(TeaModel):
+    def __init__(
+        self,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        result: bool = None,
+        success: bool = None,
+    ):
+        # The error code returned if the request failed.
+        self.error_code = error_code
+        # The error message returned if the request failed.
+        self.error_message = error_message
+        # The ID of the request.
+        self.request_id = request_id
+        # Indicates whether the permissions were revoked from the users.
+        self.result = result
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
+        self.success = success
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
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result is not None:
+            result['Result'] = self.result
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Result') is not None:
+            self.result = m.get('Result')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class RevokeTemplateAuthorityResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: RevokeTemplateAuthorityResponseBody = None,
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
+            temp_model = RevokeTemplateAuthorityResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class RevokeUserPermissionRequest(TeaModel):
     def __init__(
         self,
         db_id: str = None,
         ds_type: str = None,
         instance_id: int = None,
         logic: bool = None,
@@ -39169,15 +41791,15 @@
         search_key: str = None,
         search_range: str = None,
         search_target: str = None,
         tid: int = None,
     ):
         # The type of the database. For more information about the valid values of this parameter, see [DbType parameter](~~198106~~).
         self.db_type = db_type
-        # The type of the environment to which the database belongs. For more information, see [Change the environment type of an instance](~~163309~~).
+        # The environment type of the database. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
         # The number of the page to return.
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
         # The keyword that is used to search for databases.
         self.search_key = search_key
@@ -39190,15 +41812,15 @@
         self.search_range = search_range
         # The category of the database. Valid values:
         # 
         # *   **DB**: single database or logical database.
         # *   **SINGLE_DB**: single database.
         # *   **LOGIC_DB**: logical database.
         self.search_target = search_target
-        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to obtain the tenant ID.
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) operation to query the tenant ID.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -39317,45 +41939,48 @@
         port: int = None,
         schema_name: str = None,
         search_name: str = None,
         sid: str = None,
     ):
         # The alias of the database.
         self.alias = alias
+        # The name of the catalog to which the database belongs.
+        # 
+        # > If the type of the database engine is PostgreSQL, the name of the database is displayed.
         self.catalog_name = catalog_name
         # The ID of the database.
         self.database_id = database_id
         # The name of the data link for cross-database queries.
         self.datalink_name = datalink_name
-        # The type of the database.
+        # The type of the database engine.
         self.db_type = db_type
         # The ID of the user who assumes the database administrator (DBA) role.
         self.dba_id = dba_id
         # The encoding method of the database.
         self.encoding = encoding
-        # The type of the environment to which the database belongs. For more information, see [Change the environment type of an instance](~~163309~~).
+        # The environment type of the database. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
         # The endpoint of the instance in which the database resides.
         self.host = host
         # Indicates whether the database is a logical database. Valid values:
         # 
         # *   **true**: The database is a logical database.
         # *   **false**: The database is not a logical database.
         self.logic = logic
-        # The IDs of the owners of the database.
+        # The IDs of the owners of the databases.
         self.owner_id_list = owner_id_list
         # The nicknames of the database owners.
         self.owner_name_list = owner_name_list
-        # The port number of the instance in which the database resides.
+        # The port of the instance in which the database resides.
         self.port = port
         # The name of the database.
         self.schema_name = schema_name
         # The name that is used to search for the database.
         self.search_name = search_name
-        # The system ID (Sid) of the instance in which the database resides.
+        # The system ID (SID) of the instance in which the database resides.
         self.sid = sid
 
     def validate(self):
         if self.owner_id_list:
             self.owner_id_list.validate()
         if self.owner_name_list:
             self.owner_name_list.validate()
@@ -39480,26 +42105,26 @@
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         search_database_list: SearchDatabaseResponseBodySearchDatabaseList = None,
         success: bool = None,
         total_count: int = None,
     ):
-        # The error code returned.
+        # The error code.
         self.error_code = error_code
-        # The error message returned.
+        # The error message.
         self.error_message = error_message
         # The ID of the request.
         self.request_id = request_id
         # The information about the databases.
         self.search_database_list = search_database_list
-        # Indicates whether the request was successful. Valid values:
+        # Indicates whether the request is successful. Valid values:
         # 
-        # - **true**: The request was successful.
-        # - **false**: The request failed.
+        # *   **true**: The request is successful.
+        # *   **false**: The request fails.
         self.success = success
         # The total number of entries returned.
         self.total_count = total_count
 
     def validate(self):
         if self.search_database_list:
             self.search_database_list.validate()
@@ -39595,22 +42220,51 @@
         page_size: int = None,
         return_guid: bool = None,
         search_key: str = None,
         search_range: str = None,
         search_target: str = None,
         tid: int = None,
     ):
+        # The type of database. Valid values:
+        # 
+        # *   **MySQL**\
+        # *   **SQLServer**\
+        # *   **PostgreSQL**\
+        # *   **Oracle**\
+        # *   **DRDS**\
+        # *   **OceanBase**\
+        # *   **Mongo**\
+        # *   **Redis**\
         self.db_type = db_type
+        # The type of the environment to which databases belong. For more information, see [Change the environment type of an instance](~~163309~~).
         self.env_type = env_type
+        # The number of the page to return.
         self.page_number = page_number
+        # The number of entries to return on each page.
         self.page_size = page_size
+        # Specifies whether to return the GUID of each table.
         self.return_guid = return_guid
+        # The keyword that is used to query tables.
         self.search_key = search_key
+        # The scope of tables that you want to query. Valid values:
+        # 
+        # *   **HAS_PERMSSION**: the tables on which the current account has permissions.
+        # *   **OWNER**: the tables owned by the current account.
+        # *   **MY_FOCUS**: the tables that the current account follows.
+        # *   **UNKNOWN**: all tables.
         self.search_range = search_range
+        # The type of table that you want to query. Valid values:
+        # 
+        # *   **TABLE**: physical and logical tables
+        # *   **SINGLE_TABLE**: physical tables
+        # *   **LOGIC_TABLE**: logical tables
         self.search_target = search_target
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the [View information about the current tenant](~~181330~~) section of the "Manage DMS tenants" topic.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -39730,28 +42384,55 @@
         owner_id_list: SearchTableResponseBodySearchTableListSearchTableOwnerIdList = None,
         owner_name_list: SearchTableResponseBodySearchTableListSearchTableOwnerNameList = None,
         table_guid: str = None,
         table_id: str = None,
         table_name: str = None,
         table_schema_name: str = None,
     ):
+        # The name that is used to search for the database to which the table belongs.
         self.dbsearch_name = dbsearch_name
+        # The ID of the database to which the table belongs.
         self.database_id = database_id
+        # The name of the database.
         self.db_name = db_name
+        # The type of the database. Valid values:
+        # 
+        # *   **MySQL**\
+        # *   **SQLServer**\
+        # *   **PostgreSQL**\
+        # *   **Oracle**\
+        # *   **DRDS**\
+        # *   **OceanBase**\
+        # *   **Mongo**\
+        # *   **Redis**\
         self.db_type = db_type
+        # The description of the table.
         self.description = description
+        # The encoding format of the table.
         self.encoding = encoding
+        # The engine of the table.
         self.engine = engine
+        # The type of the environment to which the database belongs.
         self.env_type = env_type
+        # Indicates whether the table is a logical table. Valid values:
+        # 
+        # *   **true**: The table is a logical table.
+        # *   **false**: The table is not a logical table.
         self.logic = logic
+        # The IDs of the table owners.
         self.owner_id_list = owner_id_list
+        # The nicknames of the table owners.
         self.owner_name_list = owner_name_list
+        # The GUID of the table.
         self.table_guid = table_guid
+        # The ID of the table.
         self.table_id = table_id
+        # The name of the table.
         self.table_name = table_name
+        # The name of the database to which the table belongs.
         self.table_schema_name = table_schema_name
 
     def validate(self):
         if self.owner_id_list:
             self.owner_id_list.validate()
         if self.owner_name_list:
             self.owner_name_list.validate()
@@ -39872,19 +42553,25 @@
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         search_table_list: SearchTableResponseBodySearchTableList = None,
         success: bool = None,
         total_count: int = None,
     ):
+        # The error code returned if the request failed.
         self.error_code = error_code
+        # The error message returned if the request failed.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # The details of the tables.
         self.search_table_list = search_table_list
+        # Indicates whether the request was successful.
         self.success = success
+        # The total number of entries that are returned.
         self.total_count = total_count
 
     def validate(self):
         if self.search_table_list:
             self.search_table_list.validate()
 
     def to_map(self):
@@ -40272,15 +42959,19 @@
 
 class SubmitOrderApprovalRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40307,17 +42998,21 @@
     def __init__(
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40394,15 +43089,19 @@
 
 class SubmitStructSyncOrderApprovalRequest(TeaModel):
     def __init__(
         self,
         order_id: int = None,
         tid: int = None,
     ):
+        # The ID of the ticket.
         self.order_id = order_id
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40430,18 +43129,23 @@
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
         workflow_instance_id: int = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
+        # The ID of the approval process.
         self.workflow_instance_id = workflow_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40663,16 +43367,21 @@
 class SyncDatabaseMetaRequest(TeaModel):
     def __init__(
         self,
         db_id: str = None,
         logic: bool = None,
         tid: int = None,
     ):
+        # The ID of the database.
         self.db_id = db_id
+        # Specifies whether the database is a logical database.
         self.logic = logic
+        # The ID of the tenant.
+        # 
+        # > To view the tenant ID, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40703,17 +43412,21 @@
     def __init__(
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # The error code.
         self.error_code = error_code
+        # The error message.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40791,16 +43504,24 @@
 class SyncInstanceMetaRequest(TeaModel):
     def __init__(
         self,
         ignore_table: bool = None,
         instance_id: str = None,
         tid: int = None,
     ):
+        # Specifies whether to skip synchronization for the metadata of table dictionaries. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
         self.ignore_table = ignore_table
+        # The ID of the instance.
         self.instance_id = instance_id
+        # The ID of the tenant.
+        # 
+        # > To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the [View information about the current tenant](~~181330~~) section of the Manage DMS tenants topic.
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40831,17 +43552,24 @@
     def __init__(
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
+        # Details about the topology of the data table.
         self.error_code = error_code
+        # The error code returned.
         self.error_message = error_message
+        # The ID of the request.
         self.request_id = request_id
+        # Indicates whether the request is successful. Valid values:
+        # 
+        # *   **true**\
+        # *   **false**\
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40912,14 +43640,221 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = SyncInstanceMetaResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class UpdateAuthorityTemplateRequest(TeaModel):
+    def __init__(
+        self,
+        description: str = None,
+        name: str = None,
+        template_id: int = None,
+        tid: int = None,
+    ):
+        # The description of the permission template.
+        # 
+        # >  You must specify the Name or Description parameter. Otherwise, the API call fails.
+        self.description = description
+        # The name of the permission template.
+        # 
+        # >  You must specify the Name or Description parameter. Otherwise, the API call fails.
+        self.name = name
+        # The ID of the permission template.
+        self.template_id = template_id
+        # The ID of the tenant. You can call the [GetUserActiveTenant](~~198073~~) or [ListUserTenants](~~198074~~) operation to query the tenant ID.
+        self.tid = tid
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
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        if self.tid is not None:
+            result['Tid'] = self.tid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        if m.get('Tid') is not None:
+            self.tid = m.get('Tid')
+        return self
+
+
+class UpdateAuthorityTemplateResponseBodyAuthorityTemplateView(TeaModel):
+    def __init__(
+        self,
+        creator_id: int = None,
+        description: str = None,
+        name: str = None,
+        template_id: int = None,
+    ):
+        # The ID of the user who created the permission template.
+        self.creator_id = creator_id
+        # The description of the permission template.
+        self.description = description
+        # The name of the permission template.
+        self.name = name
+        # The ID of the permission template.
+        self.template_id = template_id
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
+        if self.creator_id is not None:
+            result['CreatorId'] = self.creator_id
+        if self.description is not None:
+            result['Description'] = self.description
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.template_id is not None:
+            result['TemplateId'] = self.template_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CreatorId') is not None:
+            self.creator_id = m.get('CreatorId')
+        if m.get('Description') is not None:
+            self.description = m.get('Description')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('TemplateId') is not None:
+            self.template_id = m.get('TemplateId')
+        return self
+
+
+class UpdateAuthorityTemplateResponseBody(TeaModel):
+    def __init__(
+        self,
+        authority_template_view: UpdateAuthorityTemplateResponseBodyAuthorityTemplateView = None,
+        error_code: str = None,
+        error_message: str = None,
+        request_id: str = None,
+        success: bool = None,
+    ):
+        # The details of the permission template.
+        self.authority_template_view = authority_template_view
+        # The error code.
+        self.error_code = error_code
+        # The error message returned if the request failed.
+        self.error_message = error_message
+        # The ID of the request.
+        self.request_id = request_id
+        # Indicates whether the request was successful. Valid values:
+        # 
+        # *   **true**: The request was successful.
+        # *   **false**: The request failed.
+        self.success = success
+
+    def validate(self):
+        if self.authority_template_view:
+            self.authority_template_view.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.authority_template_view is not None:
+            result['AuthorityTemplateView'] = self.authority_template_view.to_map()
+        if self.error_code is not None:
+            result['ErrorCode'] = self.error_code
+        if self.error_message is not None:
+            result['ErrorMessage'] = self.error_message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthorityTemplateView') is not None:
+            temp_model = UpdateAuthorityTemplateResponseBodyAuthorityTemplateView()
+            self.authority_template_view = temp_model.from_map(m['AuthorityTemplateView'])
+        if m.get('ErrorCode') is not None:
+            self.error_code = m.get('ErrorCode')
+        if m.get('ErrorMessage') is not None:
+            self.error_message = m.get('ErrorMessage')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class UpdateAuthorityTemplateResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: UpdateAuthorityTemplateResponseBody = None,
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
+            temp_model = UpdateAuthorityTemplateResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateInstanceRequest(TeaModel):
     def __init__(
         self,
         data_link_name: str = None,
         database_password: str = None,
         database_user: str = None,
         dba_id: str = None,
@@ -41507,15 +44442,15 @@
         self.description = description
         # The ID of the business scenario.
         self.scenario_id = scenario_id
         # The name of the business scenario.
         self.scenario_name = scenario_name
         # The ID of the tenant.
         # 
-        # >  The ID of the tenant is displayed when you move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the ["View information about the current tenant"](~~181330~~) section of the Manage DMS tenants topic.
+        # > : To view the ID of the tenant, go to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [View information about the current tenant](~~181330~~).
         self.tid = tid
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -44004,24 +46939,29 @@
         max_result_count: int = None,
         mobile: str = None,
         role_names: str = None,
         tid: int = None,
         uid: int = None,
         user_nick: str = None,
     ):
+        # The maximum number of queries that can be performed each day.
         self.max_execute_count = max_execute_count
+        # The maximum number of rows that can be queried each day.
         self.max_result_count = max_result_count
+        # The DingTalk ID or mobile number of the user.
         self.mobile = mobile
+        # The roles that the user assumes. For more information about the valid values, see the Request parameters section in the [RegisterUser](~~141565~~) topic.
         self.role_names = role_names
         # The ID of the tenant.
         # 
-        # >  To view the ID of the tenant, move the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console. For more information, see the "View information about the current tenant" section of the [Manage DMS tenants](~~181330~~) topic.
+        # > : To view the ID of the tenant, log on to the Data Management (DMS) console and move the pointer over the profile picture in the upper-right corner. For more information, see [Manage DMS tenants](~~181330~~).
         self.tid = tid
-        # The UID of the user. You can view your UID by moving the pointer over the profile picture in the upper-right corner of the Data Management (DMS) console.
+        # The Alibaba Cloud unique ID (UID) of the user to update.
         self.uid = uid
+        # The nickname of the user.
         self.user_nick = user_nick
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -44068,24 +47008,21 @@
     def __init__(
         self,
         error_code: str = None,
         error_message: str = None,
         request_id: str = None,
         success: bool = None,
     ):
-        # The error code returned if the request fails.
+        # The error code returned if the request failed.
         self.error_code = error_code
-        # The error message returned if the request fails.
+        # The error message returned if the request failed.
         self.error_message = error_message
         # The ID of the request.
         self.request_id = request_id
-        # Indicates whether the request was successful. Valid values:
-        # 
-        # *   **true**: The request was successful.
-        # *   **false**: The request failed.
+        # Indicates whether the request succeeded.
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO` & `alibabacloud_dms-enterprise20181101-1.45.0/alibabacloud_dms_enterprise20181101.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dms-enterprise20181101
-Version: 1.44.0
+Version: 1.45.0
 Summary: Alibaba Cloud dms-enterprise (20181101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dms-enterprise20181101-1.44.0/setup.py` & `alibabacloud_dms-enterprise20181101-1.45.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dms-enterprise20181101.
 
-Created on 13/01/2023
+Created on 11/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dms_enterprise20181101"
 NAME = "alibabacloud_dms-enterprise20181101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud dms-enterprise (20181101) SDK Library for Python"
```

