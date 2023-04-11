# Comparing `tmp/qbosdk-0.8.0.tar.gz` & `tmp/qbosdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbosdk-0.8.0.tar", last modified: Tue Feb 23 06:56:47 2021, max compression
+gzip compressed data, was "qbosdk-0.9.0.tar", last modified: Tue Mar 30 14:23:48 2021, max compression
```

## Comparing `qbosdk-0.8.0.tar` & `qbosdk-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:47.506186 qbosdk-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-02-23 06:56:47.506186 qbosdk-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2021-02-23 06:56:37.000000 qbosdk-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:47.502186 qbosdk-0.8.0/qbosdk/
--rw-r--r--   0 runner    (1001) docker     (121)      394 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:47.502186 qbosdk-0.8.0/qbosdk/apis/
--rw-r--r--   0 runner    (1001) docker     (121)      785 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     7625 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/attachments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/bill_payments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/bills.py
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/classes.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/company_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/customers.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/departments.py
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/employees.py
--rw-r--r--   0 runner    (1001) docker     (121)      849 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/exchange_rates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/journal_entries.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/preferences.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/purchases.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/apis/vendors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1377 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5706 2021-02-23 06:56:37.000000 qbosdk-0.8.0/qbosdk/qbosdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:47.502186 qbosdk-0.8.0/qbosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-02-23 06:56:47.000000 qbosdk-0.8.0/qbosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      790 2021-02-23 06:56:47.000000 qbosdk-0.8.0/qbosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-23 06:56:47.000000 qbosdk-0.8.0/qbosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2021-02-23 06:56:47.000000 qbosdk-0.8.0/qbosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-02-23 06:56:47.000000 qbosdk-0.8.0/qbosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-23 06:56:47.506186 qbosdk-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      904 2021-02-23 06:56:37.000000 qbosdk-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:47.502186 qbosdk-0.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:37.000000 qbosdk-0.8.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:47.506186 qbosdk-0.8.0/test/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:37.000000 qbosdk-0.8.0/test/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2021-02-23 06:56:37.000000 qbosdk-0.8.0/test/common/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:47.506186 qbosdk-0.8.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-23 06:56:37.000000 qbosdk-0.8.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-02-23 06:56:37.000000 qbosdk-0.8.0/test/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2021-02-23 06:56:37.000000 qbosdk-0.8.0/test/integration/test_qbo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:48.228463 qbosdk-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-03-30 14:23:48.228463 qbosdk-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2021-03-30 14:23:37.000000 qbosdk-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:48.224462 qbosdk-0.9.0/qbosdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:48.228463 qbosdk-0.9.0/qbosdk/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7625 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1171 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/bill_payments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/bills.py
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/classes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/company_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)      460 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/customers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/departments.py
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/employees.py
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/exchange_rates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/journal_entries.py
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/purchases.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/apis/vendors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1377 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5706 2021-03-30 14:23:37.000000 qbosdk-0.9.0/qbosdk/qbosdk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:48.224462 qbosdk-0.9.0/qbosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2021-03-30 14:23:47.000000 qbosdk-0.9.0/qbosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2021-03-30 14:23:48.000000 qbosdk-0.9.0/qbosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-30 14:23:47.000000 qbosdk-0.9.0/qbosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2021-03-30 14:23:47.000000 qbosdk-0.9.0/qbosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-03-30 14:23:47.000000 qbosdk-0.9.0/qbosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-03-30 14:23:48.228463 qbosdk-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2021-03-30 14:23:37.000000 qbosdk-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:48.228463 qbosdk-0.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:37.000000 qbosdk-0.9.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:48.228463 qbosdk-0.9.0/test/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:37.000000 qbosdk-0.9.0/test/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2843 2021-03-30 14:23:37.000000 qbosdk-0.9.0/test/common/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:48.228463 qbosdk-0.9.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-30 14:23:37.000000 qbosdk-0.9.0/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-03-30 14:23:37.000000 qbosdk-0.9.0/test/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4952 2021-03-30 14:23:37.000000 qbosdk-0.9.0/test/integration/test_qbo.py
```

### Comparing `qbosdk-0.8.0/PKG-INFO` & `qbosdk-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbosdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python SDK for accessing Quickbooks Online APIs
 Home-page: https://github.com/fylein/qbo-sdk-py
 Author: Shwetabh Kumar
 Author-email: shwetabh.kumar@fyle.in
 License: MIT
 Description: # QuickbooksOnlineSDK
```

### Comparing `qbosdk-0.8.0/README.md` & `qbosdk-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/__init__.py` & `qbosdk-0.9.0/qbosdk/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/api_base.py` & `qbosdk-0.9.0/qbosdk/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/attachments.py` & `qbosdk-0.9.0/qbosdk/apis/attachments.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/bill_payments.py` & `qbosdk-0.9.0/qbosdk/apis/bill_payments.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/bills.py` & `qbosdk-0.9.0/qbosdk/apis/bills.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/company_info.py` & `qbosdk-0.9.0/qbosdk/apis/company_info.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/employees.py` & `qbosdk-0.9.0/qbosdk/apis/employees.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/exchange_rates.py` & `qbosdk-0.9.0/qbosdk/apis/exchange_rates.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/journal_entries.py` & `qbosdk-0.9.0/qbosdk/apis/journal_entries.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/purchases.py` & `qbosdk-0.9.0/qbosdk/apis/purchases.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/apis/vendors.py` & `qbosdk-0.9.0/qbosdk/apis/vendors.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 class Vendors(ApiBase):
     """Class for Categories APIs."""
 
     GET_VENDORS = '/query?query=select * from Vendor STARTPOSITION {0} MAXRESULTS 1000'
     POST_VENDOR = '/vendor?minorversion=38'
+    SEARCH_VENDOR = "/query?query=select * from Vendor where DisplayName = '{0}'"
 
     def get(self):
         """Get a list of the existing Vendors in the Organization.
 
         Returns:
             List with dicts in Vendors schema.
         """
@@ -23,7 +24,17 @@
     def post(self, data: Dict):
         """
         Post Vendor to Quickbooks Online
         :param data: Dict in Vendor schema
         :return:
         """
         return self._post_request(data, Vendors.POST_VENDOR)
+
+    def search_vendor_by_display_name(self, display_name=None):
+        """
+        Search vendor by display name
+        :param display_name: Quickbooks Vendor Display Name
+        :return: Vendor
+        """
+        response = self._get_request('QueryResponse', Vendors.SEARCH_VENDOR.format(display_name))
+
+        return response['Vendor'][0] if 'Vendor' in response else None
```

### Comparing `qbosdk-0.8.0/qbosdk/exceptions.py` & `qbosdk-0.9.0/qbosdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk/qbosdk.py` & `qbosdk-0.9.0/qbosdk/qbosdk.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/qbosdk.egg-info/PKG-INFO` & `qbosdk-0.9.0/qbosdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qbosdk
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python SDK for accessing Quickbooks Online APIs
 Home-page: https://github.com/fylein/qbo-sdk-py
 Author: Shwetabh Kumar
 Author-email: shwetabh.kumar@fyle.in
 License: MIT
 Description: # QuickbooksOnlineSDK
```

### Comparing `qbosdk-0.8.0/qbosdk.egg-info/SOURCES.txt` & `qbosdk-0.9.0/qbosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/setup.py` & `qbosdk-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='qbosdk',
-    version='0.8.0',
+    version='0.9.0',
     author='Shwetabh Kumar',
     author_email='shwetabh.kumar@fyle.in',
     description='Python SDK for accessing Quickbooks Online APIs',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['quickbooks-online', 'quickbooks', 'fyle', 'api', 'python', 'sdk'],
```

### Comparing `qbosdk-0.8.0/test/common/utilities.py` & `qbosdk-0.9.0/test/common/utilities.py`

 * *Files identical despite different names*

### Comparing `qbosdk-0.8.0/test/integration/test_qbo.py` & `qbosdk-0.9.0/test/integration/test_qbo.py`

 * *Files identical despite different names*

