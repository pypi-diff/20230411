# Comparing `tmp/tap-linkedin-ads-2.0.1.tar.gz` & `tmp/tap-linkedin-ads-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-linkedin-ads-2.0.1.tar", last modified: Wed Mar 22 17:22:24 2023, max compression
+gzip compressed data, was "tap-linkedin-ads-2.1.0.tar", last modified: Tue Apr 11 13:58:33 2023, max compression
```

## Comparing `tap-linkedin-ads-2.0.1.tar` & `tap-linkedin-ads-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-22 17:22:24.452412 tap-linkedin-ads-2.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      339 2023-03-22 17:22:24.452412 tap-linkedin-ads-2.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16976 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-22 17:22:24.452412 tap-linkedin-ads-2.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      840 2023-03-22 17:21:48.000000 tap-linkedin-ads-2.0.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-22 17:22:24.448412 tap-linkedin-ads-2.0.1/tap_linkedin_ads/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1620 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14765 2023-03-22 17:21:48.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      612 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2017 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-22 17:22:24.452412 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1696 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/account_users.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3471 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/accounts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13824 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13791 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/ad_analytics_by_creative.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2989 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/campaign_groups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12277 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2192 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/creatives.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/video_ads.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32739 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5605 2023-03-15 14:38:35.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12355 2023-03-14 18:56:00.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads/transform.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-22 17:22:24.448412 tap-linkedin-ads-2.0.1/tap_linkedin_ads.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      339 2023-03-22 17:22:24.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      822 2023-03-22 17:22:24.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-22 17:22:24.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-03-22 17:22:24.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       73 2023-03-22 17:22:24.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-03-22 17:22:24.000000 tap-linkedin-ads-2.0.1/tap_linkedin_ads.egg-info/top_level.txt
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-04-11 13:58:33.141007 tap-linkedin-ads-2.1.0/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    34523 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/LICENSE
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      339 2023-04-11 13:58:33.141007 tap-linkedin-ads-2.1.0/PKG-INFO
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    16976 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/README.md
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       38 2023-04-11 13:58:33.141007 tap-linkedin-ads-2.1.0/setup.cfg
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      840 2023-04-11 13:57:05.000000 tap-linkedin-ads-2.1.0/setup.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-04-11 13:58:33.137007 tap-linkedin-ads-2.1.0/tap_linkedin_ads/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1620 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/__init__.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    14809 2023-04-11 13:57:05.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/client.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      612 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/discover.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2706 2023-04-11 13:57:05.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schema.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-04-11 13:58:33.137007 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1696 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/account_users.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     3471 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/accounts.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    13824 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    13791 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2989 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/campaign_groups.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    12277 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/campaigns.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     2192 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/creatives.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     1989 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/video_ads.json
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    31980 2023-04-11 13:57:05.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/streams.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)     5605 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/sync.py
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)    12355 2023-04-07 18:22:18.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads/transform.py
+drwxrwxr-x   0 dsprayberry  (1001) dsprayberry  (1001)        0 2023-04-11 13:58:33.137007 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      339 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/PKG-INFO
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)      822 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)        1 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       84 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/entry_points.txt
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       73 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/requires.txt
+-rw-rw-r--   0 dsprayberry  (1001) dsprayberry  (1001)       17 2023-04-11 13:58:32.000000 tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/top_level.txt
```

### Comparing `tap-linkedin-ads-2.0.1/LICENSE` & `tap-linkedin-ads-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/README.md` & `tap-linkedin-ads-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/setup.py` & `tap-linkedin-ads-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-linkedin-ads',
-      version='2.0.1',
+      version='2.1.0',
       description='Singer.io tap for extracting data from the LinkedIn Marketing Ads API API 2.0',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_linkedin_ads'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
```

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/__init__.py` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/client.py` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from singer import metrics
 import singer
 
 LOGGER = singer.get_logger()
 BASE_URL = 'https://api.linkedin.com/rest'
 LINKEDIN_TOKEN_URI = 'https://www.linkedin.com/oauth/v2/accessToken'
 INTROSPECTION_URI = 'https://www.linkedin.com/oauth/v2/introspectToken'
+LINKEDIN_VERSION = '202302'
 
 # set default timeout of 300 seconds
 REQUEST_TIMEOUT = 300
 
 class LinkedInError(Exception):
     pass
 
@@ -289,15 +290,15 @@
                           factor=2)
     def check_accounts(self, config):
         headers = {}
         if self.__user_agent:
             headers['User-Agent'] = self.__user_agent
         headers['Authorization'] = 'Bearer {}'.format(self.__access_token)
         headers['Accept'] = 'application/json'
-        headers['LinkedIn-Version'] = "202207"
+        headers['LinkedIn-Version'] = LINKEDIN_VERSION
 
         if config.get('accounts'):
             account_list = config['accounts'].replace(" ", "").split(",")
             invalid_account = []
             for account in account_list:
                 response = self.__session.get(
                     url='https://api.linkedin.com/rest/adAccountUsers?q=accounts&count=1&start=0&accounts=urn:li:sponsoredAccount:{}'.format(account),
@@ -344,15 +345,15 @@
         else:
             endpoint = None
 
         if 'headers' not in kwargs:
             kwargs['headers'] = {}
         kwargs['headers']['Authorization'] = 'Bearer {}'.format(self.__access_token)
         kwargs['headers']['Accept'] = 'application/json'
-        kwargs['headers']['LinkedIn-Version'] = "202207"
+        kwargs['headers']['LinkedIn-Version'] = LINKEDIN_VERSION
         kwargs['headers']['Cache-Control'] = "no-cache"
 
         if self.__user_agent:
             kwargs['headers']['User-Agent'] = self.__user_agent
 
         if method == 'POST':
             kwargs['headers']['Content-Type'] = 'application/json'
```

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/discover.py` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/discover.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/account_users.json` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/account_users.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/accounts.json` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/ad_analytics_by_campaign.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/ad_analytics_by_creative.json` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/ad_analytics_by_creative.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/campaign_groups.json` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/campaign_groups.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/campaigns.json` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/creatives.json` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/creatives.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/schemas/video_ads.json` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/schemas/video_ads.json`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/streams.py` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,32 +14,15 @@
 # We will skip these fields while passing selected fields in the API parameters.
 FIELDS_UNAVAILABLE_FOR_AD_ANALYTICS = {
     'campaign',
     'campaignId',
     'startAt',
     'endAt',
     'creative',
-    'creativeId'
-}
-
-# As mentioned here some fields of ads_analytics are currently in beta:
-# https://docs.microsoft.com/en-us/linkedin/marketing/integrations/ads-reporting/ads-reporting?view=li-lms-2022-08&tabs=http#accuracy
-FIELDS_UNACCEPTED_BY_API = {
-    "ad_analytics_by_creative": {
-        "averageDailyReachMetrics",
-        "averagePreviousSevenDayReachMetrics",
-        "averagePreviousThirtyDayReachMetrics",
-        "approximateUniqueImpressions"
-    },
-    "ad_analytics_by_campaign": {
-        "averageDailyReachMetrics",
-        "averagePreviousSevenDayReachMetrics",
-        "averagePreviousThirtyDayReachMetrics",
-        "approximateUniqueImpressions"
-    }
+    'creativeId',
 }
 
 def write_bookmark(state, value, stream_name):
     """
     Write the bookmark in the state corresponding to the stream.
     """
     if 'bookmarks' not in state:
@@ -484,16 +467,15 @@
                          'dateRange.end.month': window_end_date.month,
                          'dateRange.end.year': window_end_date.year,}
 
         # Here, valid_selected_fields is a list of fields that the user has selected.
         # API accepts these fields in the parameter and returns its value in the response.
         valid_selected_fields = [snake_case_to_camel_case(field)
                                  for field in selected_fields(catalog.get_stream(self.tap_stream_id))
-                                 if snake_case_to_camel_case(field) not in FIELDS_UNAVAILABLE_FOR_AD_ANALYTICS.union(
-                                     FIELDS_UNACCEPTED_BY_API.get(self.tap_stream_id, set()))]
+                                 if snake_case_to_camel_case(field) not in FIELDS_UNAVAILABLE_FOR_AD_ANALYTICS]
 
         # When testing the API, if the fields in `field` all return `0` then
         # the API returns its empty response.
 
         # However, the API distinguishes between a day with non-null values
         # (even if this means the values are all `0`) and a day with null
         # values. We found that requesting these fields gives you the days with
```

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/sync.py` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/sync.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads/transform.py` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads/transform.py`

 * *Files identical despite different names*

### Comparing `tap-linkedin-ads-2.0.1/tap_linkedin_ads.egg-info/SOURCES.txt` & `tap-linkedin-ads-2.1.0/tap_linkedin_ads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

