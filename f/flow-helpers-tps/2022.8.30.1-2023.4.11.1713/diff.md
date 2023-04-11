# Comparing `tmp/flow-helpers-tps-2022.8.30.1.tar.gz` & `tmp/flow_helpers_tps-2023.4.11.1713.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flow-helpers-tps-2022.8.30.1.tar", max compression
+gzip compressed data, was "flow_helpers_tps-2023.4.11.1713.tar", max compression
```

## Comparing `flow-helpers-tps-2022.8.30.1.tar` & `flow_helpers_tps-2023.4.11.1713.tar`

### file list

```diff
@@ -1,33 +1,30 @@
--rw-r--r--   0        0        0     1069 2022-08-30 17:40:58.455136 flow-helpers-tps-2022.8.30.1/LICENSE
--rw-r--r--   0        0        0      396 2022-08-30 17:40:58.455136 flow-helpers-tps-2022.8.30.1/README.md
--rw-r--r--   0        0        0        0 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/__init__.py
--rw-r--r--   0        0        0     4868 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_bingwmt.py
--rw-r--r--   0        0        0      657 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_covidtracking.py
--rw-r--r--   0        0        0     3895 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_dcm.py
--rw-r--r--   0        0        0     3230 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_facebook.py
--rw-r--r--   0        0        0      488 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_file.py
--rw-r--r--   0        0        0     9354 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_firebasetransform.py
--rw-r--r--   0        0        0    10574 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_funneltransform.py
--rw-r--r--   0        0        0    24475 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gatransform.py
--rw-r--r--   0        0        0     6953 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gbq.py
--rw-r--r--   0        0        0     4308 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gcs.py
--rw-r--r--   0        0        0     2639 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gdrive.py
--rw-r--r--   0        0        0    11001 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_googleanalytics.py
--rw-r--r--   0        0        0     4408 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gsc.py
--rw-r--r--   0        0        0      631 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gsheet.py
--rw-r--r--   0        0        0      981 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_impact.py
--rw-r--r--   0        0        0     7255 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_journera.py
--rw-r--r--   0        0        0     2986 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_listen360.py
--rw-r--r--   0        0        0     6403 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_mssql.py
--rw-r--r--   0        0        0      505 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_s3.py
--rw-r--r--   0        0        0     7919 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_sa360.py
--rw-r--r--   0        0        0    18284 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_salesforce.py
--rw-r--r--   0        0        0     2628 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_scrapinghub.py
--rw-r--r--   0        0        0     6739 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_sftp.py
--rw-r--r--   0        0        0     6113 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_sharepoint.py
--rw-r--r--   0        0        0    11123 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_snowflake.py
--rw-r--r--   0        0        0       68 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_test.py
--rw-r--r--   0        0        0     2264 2022-08-30 17:40:58.463136 flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_time.py
--rw-r--r--   0        0        0      649 2022-08-30 17:40:58.467136 flow-helpers-tps-2022.8.30.1/pyproject.toml
--rw-r--r--   0        0        0     1273 2022-08-30 17:42:37.691297 flow-helpers-tps-2022.8.30.1/setup.py
--rw-r--r--   0        0        0     1297 2022-08-30 17:42:37.691624 flow-helpers-tps-2022.8.30.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-11 17:12:33.901009 flow_helpers_tps-2023.4.11.1713/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/__init__.py
+-rw-r--r--   0        0        0     4868 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_bingwmt.py
+-rw-r--r--   0        0        0      657 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_covidtracking.py
+-rw-r--r--   0        0        0     3895 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_dcm.py
+-rw-r--r--   0        0        0     3288 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_facebook.py
+-rw-r--r--   0        0        0      488 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_file.py
+-rw-r--r--   0        0        0     9315 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_firebasetransform.py
+-rw-r--r--   0        0        0    10574 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_funneltransform.py
+-rw-r--r--   0        0        0    24475 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gatransform.py
+-rw-r--r--   0        0        0     6953 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gbq.py
+-rw-r--r--   0        0        0     4308 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gcs.py
+-rw-r--r--   0        0        0     2639 2023-04-11 17:12:33.909010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gdrive.py
+-rw-r--r--   0        0        0    11001 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_googleanalytics.py
+-rw-r--r--   0        0        0     4408 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gsc.py
+-rw-r--r--   0        0        0      631 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gsheet.py
+-rw-r--r--   0        0        0      981 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_impact.py
+-rw-r--r--   0        0        0     7255 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_journera.py
+-rw-r--r--   0        0        0     2986 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_listen360.py
+-rw-r--r--   0        0        0     6403 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_mssql.py
+-rw-r--r--   0        0        0      505 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_s3.py
+-rw-r--r--   0        0        0     7919 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sa360.py
+-rw-r--r--   0        0        0    18284 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_salesforce.py
+-rw-r--r--   0        0        0     2628 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_scrapinghub.py
+-rw-r--r--   0        0        0     6739 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sftp.py
+-rw-r--r--   0        0        0     6113 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sharepoint.py
+-rw-r--r--   0        0        0    11123 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_snowflake.py
+-rw-r--r--   0        0        0     2264 2023-04-11 17:12:33.913010 flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_time.py
+-rw-r--r--   0        0        0      592 2023-04-11 17:13:09.357071 flow_helpers_tps-2023.4.11.1713/pyproject.toml
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 flow_helpers_tps-2023.4.11.1713/PKG-INFO
```

### Comparing `flow-helpers-tps-2022.8.30.1/LICENSE` & `flow_helpers_tps-2023.4.11.1713/LICENSE`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_bingwmt.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_bingwmt.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_covidtracking.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_covidtracking.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_dcm.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_dcm.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_facebook.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_facebook.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
-from facebook_business.adobjects.adaccount import AdAccount
-from facebook_business.adobjects.adsinsights import AdsInsights
-from facebook_business.api import FacebookAdsApi
+# from facebook_business.adobjects.adaccount import AdAccount
+# from facebook_business.adobjects.adsinsights import AdsInsights
+# from facebook_business.api import FacebookAdsApi
 import hmac
 import hashlib
 import requests
 import json
 
 class Facebook:
     def __init__(self, app_id, app_secret, access_token):
@@ -14,43 +14,43 @@
         self.access_token = access_token
         self.appsecret_proof = hmac.new(
             self.app_secret.encode('utf-8'),
             msg=self.access_token.encode('utf-8'),
             digestmod=hashlib.sha256
         ).hexdigest()
 
-    def pull_insights_sdk(self, adaccount_id, since, until, fieldlist, time_increment=1, level='ad'):
-        FacebookAdsApi.init(app_id=self.app_id, app_secret=self.app_secret, access_token=self.access_token)
-        # since / until is end date inclusive
-        # time_increment = 1 to break into individual days
-
-        params = {
-            'time_increment':time_increment,
-            'time_range': {
-                'since': f'{since}',
-                'until': f'{until}'
-            },
-            'fields': fieldlist,
-            'breakdowns': [],
-            'level': level,
-            'action_report_time': 'conversion',
-            'use_unified_attribution_setting': True
-        }
-
-        results = AdAccount(adaccount_id).get_insights(params=params)
-        results = str(results)
-        results = results.replace('<AdsInsights>','')
-        results = json.loads(results)
-        return results
+    # def pull_insights_sdk(self, adaccount_id, since, until, fieldlist, time_increment=1, level='ad'):
+    #     FacebookAdsApi.init(app_id=self.app_id, app_secret=self.app_secret, access_token=self.access_token)
+    #     # since / until is end date inclusive
+    #     # time_increment = 1 to break into individual days
+    #
+    #     params = {
+    #         'time_increment':time_increment,
+    #         'time_range': {
+    #             'since': f'{since}',
+    #             'until': f'{until}'
+    #         },
+    #         'fields': fieldlist,
+    #         'breakdowns': [],
+    #         'level': level,
+    #         'action_report_time': 'conversion',
+    #         'use_unified_attribution_setting': True
+    #     }
+    #
+    #     results = AdAccount(adaccount_id).get_insights(params=params)
+    #     results = str(results)
+    #     results = results.replace('<AdsInsights>','')
+    #     results = json.loads(results)
+    #     return results
 
     def pull_insights_requests(self, adaccount_id, since, until, fieldlist, time_increment=1):
         # since / until is end date inclusive
         # time_increment = 1 to break into individual days
 
-        url = f'https://graph.facebook.com/v11.0/{adaccount_id}/insights'
+        url = f'https://graph.facebook.com/v16.0/{adaccount_id}/insights'
 
         params = {
             'access_token': self.access_token,
             'appsecret_proof': self.appsecret_proof,
             'time_range': str({'since': f'{since}', 'until': f'{until}'}),
             'time_increment': time_increment,
             'fields': fieldlist,
```

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_firebasetransform.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_firebasetransform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pandas as pd
 import json
 from flatdict import FlatDict
-from pandas.io.json import json_normalize
 from datetime import datetime, timedelta, date
 import numpy as np
 
 # standard columns
 ## add additional as needed for specific transform requirements + end table
 standard_columns = ['event_date',
                  'event_timestamp',
@@ -100,15 +99,15 @@
 
         event = FlatDict(event)
         rename_keys = [key.replace(':', '_') for key in event.keys()]
         event = dict(zip(rename_keys, list(event.values())))
         event_list[i] = event
         print(f'{i + 1}/{len(event_list)} rows complete.', end='\r')
 
-    df = json_normalize(event_list)
+    df = pd.json_normalize(event_list)
 
     return df
 
 def transform_initial(df):
     df1 = df[df['platform'] != 'WEB'].copy()
 
     columns = df1.columns
```

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_funneltransform.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_funneltransform.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gatransform.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gatransform.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gbq.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gbq.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gcs.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gcs.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gdrive.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gdrive.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_googleanalytics.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_googleanalytics.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gsc.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gsc.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_gsheet.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_gsheet.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_impact.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_impact.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_journera.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_journera.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_listen360.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_listen360.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_mssql.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_mssql.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_sa360.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sa360.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_salesforce.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_salesforce.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_scrapinghub.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_scrapinghub.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_sftp.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sftp.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_sharepoint.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_sharepoint.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_snowflake.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_snowflake.py`

 * *Files identical despite different names*

### Comparing `flow-helpers-tps-2022.8.30.1/flow_helpers_tps/_time.py` & `flow_helpers_tps-2023.4.11.1713/flow_helpers_tps/_time.py`

 * *Files identical despite different names*

