# Comparing `tmp/flow_helpers_tps-2023.4.11.1713.tar.gz` & `tmp/flow_helpers_tps-2023.4.11.1755.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow_helpers_tps-2023.4.11.1713.tar", max compression
+gzip compressed data, was "flow_helpers_tps-2023.4.11.1755.tar", max compression
```

## Comparing `flow_helpers_tps-2023.4.11.1713.tar` & `flow_helpers_tps-2023.4.11.1755.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1069 2023-04-11 17:12:33.901009 flow_helpers_tps-2023.4.11.1713/LICENSE
--rw-r--r--   0        0        0        0 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/__init__.py
--rw-r--r--   0        0        0     4868 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_bingwmt.py
--rw-r--r--   0        0        0      657 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_covidtracking.py
--rw-r--r--   0        0        0     3895 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_dcm.py
--rw-r--r--   0        0        0     3288 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_facebook.py
--rw-r--r--   0        0        0      488 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_file.py
--rw-r--r--   0        0        0     9315 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_firebasetransform.py
--rw-r--r--   0        0        0    10574 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_funneltransform.py
--rw-r--r--   0        0        0    24475 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gatransform.py
--rw-r--r--   0        0        0     6953 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gbq.py
--rw-r--r--   0        0        0     4308 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gcs.py
--rw-r--r--   0        0        0     2639 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gdrive.py
--rw-r--r--   0        0        0    11001 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_googleanalytics.py
--rw-r--r--   0        0        0     4408 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gsc.py
--rw-r--r--   0        0        0      631 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gsheet.py
--rw-r--r--   0        0        0      981 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_impact.py
--rw-r--r--   0        0        0     7255 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_journera.py
--rw-r--r--   0        0        0     2986 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_listen360.py
--rw-r--r--   0        0        0     6403 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_mssql.py
--rw-r--r--   0        0        0      505 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_s3.py
--rw-r--r--   0        0        0     7919 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sa360.py
--rw-r--r--   0        0        0    18284 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_salesforce.py
--rw-r--r--   0        0        0     2628 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_scrapinghub.py
--rw-r--r--   0        0        0     6739 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sftp.py
--rw-r--r--   0        0        0     6113 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sharepoint.py
--rw-r--r--   0        0        0    11123 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_snowflake.py
--rw-r--r--   0        0        0     2264 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_time.py
--rw-r--r--   0        0        0      592 2023-04-11 17:13:09.357071 flow_helpers_tps-2023.4.11.1713/pyproject.toml
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 flow_helpers_tps-2023.4.11.1713/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-11 17:55:08.719243 flow_helpers_tps-2023.4.11.1755/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/__init__.py
+-rw-r--r--   0        0        0     4868 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_bingwmt.py
+-rw-r--r--   0        0        0      657 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_covidtracking.py
+-rw-r--r--   0        0        0     3895 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_dcm.py
+-rw-r--r--   0        0        0     3230 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_facebook.py
+-rw-r--r--   0        0        0      488 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_file.py
+-rw-r--r--   0        0        0     9315 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_firebasetransform.py
+-rw-r--r--   0        0        0    10574 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_funneltransform.py
+-rw-r--r--   0        0        0    24475 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gatransform.py
+-rw-r--r--   0        0        0     6953 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gbq.py
+-rw-r--r--   0        0        0     4308 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gcs.py
+-rw-r--r--   0        0        0     2639 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gdrive.py
+-rw-r--r--   0        0        0    11001 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_googleanalytics.py
+-rw-r--r--   0        0        0     4408 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gsc.py
+-rw-r--r--   0        0        0      631 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gsheet.py
+-rw-r--r--   0        0        0      981 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_impact.py
+-rw-r--r--   0        0        0     7255 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_journera.py
+-rw-r--r--   0        0        0     2986 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_listen360.py
+-rw-r--r--   0        0        0     6403 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_mssql.py
+-rw-r--r--   0        0        0      505 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_s3.py
+-rw-r--r--   0        0        0     7919 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_sa360.py
+-rw-r--r--   0        0        0    18284 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_salesforce.py
+-rw-r--r--   0        0        0     2628 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_scrapinghub.py
+-rw-r--r--   0        0        0     6739 2023-04-11 17:55:08.731243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_sftp.py
+-rw-r--r--   0        0        0     6113 2023-04-11 17:55:08.735243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_sharepoint.py
+-rw-r--r--   0        0        0    11123 2023-04-11 17:55:08.735243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_snowflake.py
+-rw-r--r--   0        0        0     2264 2023-04-11 17:55:08.735243 flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_time.py
+-rw-r--r--   0        0        0      622 2023-04-11 17:55:56.687246 flow_helpers_tps-2023.4.11.1755/pyproject.toml
+-rw-r--r--   0        0        0      890 1970-01-01 00:00:00.000000 flow_helpers_tps-2023.4.11.1755/PKG-INFO
```

### Comparing `flow_helpers_tps-2023.4.11.1713/LICENSE` & `flow_helpers_tps-2023.4.11.1755/LICENSE`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_bingwmt.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_bingwmt.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_covidtracking.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_covidtracking.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_dcm.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_dcm.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_facebook.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_facebook.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
-# from facebook_business.adobjects.adaccount import AdAccount
-# from facebook_business.adobjects.adsinsights import AdsInsights
-# from facebook_business.api import FacebookAdsApi
+from facebook_business.adobjects.adaccount import AdAccount
+from facebook_business.adobjects.adsinsights import AdsInsights
+from facebook_business.api import FacebookAdsApi
 import hmac
 import hashlib
 import requests
 import json
 
 class Facebook:
     def __init__(self, app_id, app_secret, access_token):
@@ -14,37 +14,37 @@
         self.access_token = access_token
         self.appsecret_proof = hmac.new(
             self.app_secret.encode('utf-8'),
             msg=self.access_token.encode('utf-8'),
             digestmod=hashlib.sha256
         ).hexdigest()
 
-    # def pull_insights_sdk(self, adaccount_id, since, until, fieldlist, time_increment=1, level='ad'):
-    #     FacebookAdsApi.init(app_id=self.app_id, app_secret=self.app_secret, access_token=self.access_token)
-    #     # since / until is end date inclusive
-    #     # time_increment = 1 to break into individual days
-    #
-    #     params = {
-    #         'time_increment':time_increment,
-    #         'time_range': {
-    #             'since': f'{since}',
-    #             'until': f'{until}'
-    #         },
-    #         'fields': fieldlist,
-    #         'breakdowns': [],
-    #         'level': level,
-    #         'action_report_time': 'conversion',
-    #         'use_unified_attribution_setting': True
-    #     }
-    #
-    #     results = AdAccount(adaccount_id).get_insights(params=params)
-    #     results = str(results)
-    #     results = results.replace('<AdsInsights>','')
-    #     results = json.loads(results)
-    #     return results
+    def pull_insights_sdk(self, adaccount_id, since, until, fieldlist, time_increment=1, level='ad'):
+        FacebookAdsApi.init(app_id=self.app_id, app_secret=self.app_secret, access_token=self.access_token)
+        # since / until is end date inclusive
+        # time_increment = 1 to break into individual days
+
+        params = {
+            'time_increment':time_increment,
+            'time_range': {
+                'since': f'{since}',
+                'until': f'{until}'
+            },
+            'fields': fieldlist,
+            'breakdowns': [],
+            'level': level,
+            'action_report_time': 'conversion',
+            'use_unified_attribution_setting': True
+        }
+
+        results = AdAccount(adaccount_id).get_insights(params=params)
+        results = str(results)
+        results = results.replace('<AdsInsights>','')
+        results = json.loads(results)
+        return results
 
     def pull_insights_requests(self, adaccount_id, since, until, fieldlist, time_increment=1):
         # since / until is end date inclusive
         # time_increment = 1 to break into individual days
 
         url = f'https://graph.facebook.com/v16.0/{adaccount_id}/insights'
```

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_firebasetransform.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_firebasetransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_funneltransform.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_funneltransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gatransform.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gatransform.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gbq.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gbq.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gcs.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gcs.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gdrive.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gdrive.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_googleanalytics.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_googleanalytics.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gsc.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gsc.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gsheet.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_gsheet.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_impact.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_impact.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_journera.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_journera.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_listen360.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_listen360.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_mssql.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_mssql.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sa360.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_sa360.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_salesforce.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_salesforce.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_scrapinghub.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_scrapinghub.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sftp.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_sftp.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sharepoint.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_sharepoint.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_snowflake.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_snowflake.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_time.py` & `flow_helpers_tps-2023.4.11.1755/flow_helpers_tps/_time.py`

 * *Files identical despite different names*

### Comparing `flow_helpers_tps-2023.4.11.1713/pyproject.toml` & `flow_helpers_tps-2023.4.11.1755/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flow-helpers-tps"
-version = "2023.04.11.1713"
+version = "2023.04.11.1755"
 description = "Handy helpers for ETL and API interfacing."
 authors = [ "joshliu3 <jliu@theparkingspot.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 google-api-python-client = "^2.85.0"
@@ -17,9 +17,10 @@
 flatdict = "4.0.0"
 boto3 = "^1.26.110"
 Office365-REST-Python-Client = "^2.4.0"
 toml = "0.10.2"
 pendulum = "^2.1.2"
 pysftp = "0.2.9"
 SQLAlchemy = "^2.0.9"
+facebook-business = "^16.0.2"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `flow_helpers_tps-2023.4.11.1713/PKG-INFO` & `flow_helpers_tps-2023.4.11.1755/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: flow-helpers-tps
-Version: 2023.4.11.1713
+Version: 2023.4.11.1755
 Summary: Handy helpers for ETL and API interfacing.
 License: MIT
 Author: joshliu3
 Author-email: jliu@theparkingspot.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Office365-REST-Python-Client (>=2.4.0,<3.0.0)
 Requires-Dist: SQLAlchemy (>=2.0.9,<3.0.0)
 Requires-Dist: boto3 (>=1.26.110,<2.0.0)
+Requires-Dist: facebook-business (>=16.0.2,<17.0.0)
 Requires-Dist: flatdict (==4.0.0)
 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: google-api-python-client (>=2.85.0,<3.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pysftp (==0.2.9)
 Requires-Dist: toml (==0.10.2)
```

