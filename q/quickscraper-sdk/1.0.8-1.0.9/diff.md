# Comparing `tmp/quickscraper_sdk-1.0.8-py3-none-any.whl.zip` & `tmp/quickscraper_sdk-1.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6203 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat     7613 b- defN 23-Apr-03 07:36 quickscraper_sdk/__init__.py
--rw-rw-rw-  2.0 fat      272 b- defN 23-Apr-03 08:49 quickscraper_sdk/constant.py
+Zip file size: 6398 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat     8851 b- defN 23-Apr-11 05:19 quickscraper_sdk/__init__.py
+-rw-rw-rw-  2.0 fat      272 b- defN 23-Apr-11 05:19 quickscraper_sdk/constant.py
 -rw-rw-rw-  2.0 fat       70 b- defN 23-Mar-31 09:41 tests/__init__.py
 -rw-rw-rw-  2.0 fat      192 b- defN 23-Mar-31 09:41 tests/constant.py
 -rw-rw-rw-  2.0 fat     5250 b- defN 23-Mar-31 09:41 tests/test_cases.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-03 08:49 quickscraper_sdk-1.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3225 b- defN 23-Apr-03 08:49 quickscraper_sdk-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-03 08:49 quickscraper_sdk-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-03 08:49 quickscraper_sdk-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      821 b- defN 23-Apr-03 08:49 quickscraper_sdk-1.0.8.dist-info/RECORD
-10 files, 18650 bytes uncompressed, 4795 bytes compressed:  74.3%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4126 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      821 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/RECORD
+10 files, 20789 bytes uncompressed, 4990 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tests/constant.py
 Comment: 
 
 Filename: tests/test_cases.py
 Comment: 
 
-Filename: quickscraper_sdk-1.0.8.dist-info/LICENSE
+Filename: quickscraper_sdk-1.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: quickscraper_sdk-1.0.8.dist-info/METADATA
+Filename: quickscraper_sdk-1.0.9.dist-info/METADATA
 Comment: 
 
-Filename: quickscraper_sdk-1.0.8.dist-info/WHEEL
+Filename: quickscraper_sdk-1.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: quickscraper_sdk-1.0.8.dist-info/top_level.txt
+Filename: quickscraper_sdk-1.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: quickscraper_sdk-1.0.8.dist-info/RECORD
+Filename: quickscraper_sdk-1.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quickscraper_sdk/__init__.py

```diff
@@ -22,40 +22,47 @@
                 session_number: str = None,
                 country_code: str = None,
                 premium: bool = None,
                 keep_headers: bool = None,
                 headers: dict = {},
                 format: str = 'html',
                 device_type: str = None,
-                parserSubscriptionId: str = None):
+                parserSubscriptionId: str = None,
+                webhookRequestId: str = None):
         request_url = self.__prepareRequestUrl(
             url=url, render=render, session_number=session_number,
             country_code=country_code,
             premium=premium, keep_headers=keep_headers, format=format,
-            device_type=device_type, parserSubscriptionId=parserSubscriptionId)
+            device_type=device_type, parserSubscriptionId=parserSubscriptionId,
+            webhookRequestId=webhookRequestId)
         custom_headers = headers
         request_options = self.__prepareHeaders(custom_headers, keep_headers)
         try:
             response = requests.get(request_url, headers=request_options)
-            body_json = response.json()
-            response._content = bytes(str(body_json), 'utf-8')
+            if parserSubscriptionId is not None:
+                response._content = response.json()
+            else:
+                response._content = response.text
+
         except ValueError:
             pass
         return response
 
     def writeHtmlToFile(self, url: str, file_path: str, render: bool = None,
                         session_number: str = None, country_code: str = None,
                         premium: bool = None, keep_headers: bool = None,
                         headers: dict = {}, format: str = None,
                         device_type: str = None,
-                        parserSubscriptionId: str = None):
+                        parserSubscriptionId: str = None,
+                        webhookRequestId: str = None):
         with open(file_path, 'wb') as file:
             response = self.getHtml(
                 url, render, session_number, country_code, premium,
-                keep_headers, headers, format, device_type, parserSubscriptionId)
+                keep_headers, headers, format, device_type, parserSubscriptionId,
+                webhookRequestId)
             if format == 'images' or format == 'docx':
                 try:
                     response._content = b64decode(response.text)
                 except ValueError:
                     pass
             file.write(response.content)
         return response
@@ -115,20 +122,22 @@
                   render: bool = None,
                   session_number: str = None,
                   country_code: str = None,
                   premium: bool = None,
                   keep_headers: bool = None,
                   format: str = 'html',
                   device_type: str = None,
-                  parserSubscriptionId: str = None):
+                  parserSubscriptionId: str = None,
+                  webhookRequestId: str = None):
         request_url = self.__prepareRequestUrl(
             url=url, render=render, session_number=session_number,
             country_code=country_code,
             premium=premium, keep_headers=keep_headers, format=format,
-            device_type=device_type, parserSubscriptionId=parserSubscriptionId)
+            device_type=device_type, parserSubscriptionId=parserSubscriptionId,
+            webhookRequestId=webhookRequestId)
         return request_url
 
     def account(self):
         response = requests.get(self.account_url,
                                 params={'access_token':
                                         self.access_token}).json()
         if response.get('message'):
@@ -145,14 +154,16 @@
             'premium': 'true' if kwargs['premium'] is True else None,
             'keep_headers': 'true' if kwargs['keep_headers'] is True else None,
             'format': kwargs['format'],
             'device_type': kwargs['device_type'],
         }
         if kwargs.get('parserSubscriptionId') is not None:
             url_options['parserSubscriptionRequestId'] = kwargs['parserSubscriptionId']
+        if kwargs.get('webhookRequestId') is not None:
+            url_options['webhookRequestId'] = kwargs['webhookRequestId']
 
         url_options_filtered = {
             key: value for key, value in
             url_options.items() if value is not None
         }
         option_string = urlencode(url_options_filtered)
         request_url = self.parse_url + '?' + option_string
@@ -164,7 +175,22 @@
             'Client-Version': VERSION
         }
         merged_headers = headers.copy()
         merged_headers.update(custom_headers)
         if keep_headers is True:
             return merged_headers
         return headers
+
+    # This function is used for csv, json, excel
+    def getData(self, url: str, render: bool = None, session_number: str = None,
+                country_code: str = None,
+                premium: bool = None, keep_headers: bool = None,
+                headers: dict = {}, format: str = None,
+                device_type: str = None,
+                parserSubscriptionId: str = None, webhookRequestId: str = None):
+        try:
+            response = self.getHtml(url, render, session_number, country_code, premium,
+                                    keep_headers, headers, format, device_type,
+                                    parserSubscriptionId, webhookRequestId)
+        except ValueError:
+            pass
+        return response
```

## quickscraper_sdk/constant.py

```diff
@@ -1,10 +1,10 @@
 import os
 
 
 BASE_URL = os.environ.get('QS_BASE_URL') or 'https://api.quickscraper.co/'
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 
 
 # from importlib.metadata import version
 # VERSION = version('quickscraper-sdk')
 # Not working this approach with pytest, so version is defined statically
```

## Comparing `quickscraper_sdk-1.0.8.dist-info/LICENSE` & `quickscraper_sdk-1.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `quickscraper_sdk-1.0.8.dist-info/METADATA` & `quickscraper_sdk-1.0.9.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickscraper-sdk
-Version: 1.0.8
+Version: 1.0.9
 Summary: https://quickscraper.co
 Home-page: https://quickscraper.co/
 Author: QuickScraper
 Author-email: app@quickscraper.co
 License: BSD
 Keywords: quickscraper
 Classifier: Development Status :: 3 - Alpha
@@ -31,15 +31,15 @@
 
 ### Basic Usage
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
 response = quickscraper_client.getHtml('http://httpbin.org/ip')
-print(response.text)
+print(response._content)
 ```
 
 ### Write a HTML to File
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
@@ -49,53 +49,53 @@
 
 ### Rendering Javascript
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
 response = quickscraper_client.getHtml('http://httpbin.org/ip', render=True)
-print(response.text)
+print(response._content)
 ```
 
 ### Custom Headers
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
 response = quickscraper_client.getHtml(
     'https://httpbin.org/headers', keep_headers=True, headers={'X-My-Custom-Header': 'QS-APP'})
-print(response.text)
+print(response._content)
 ```
 
 ### Geographic Location
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
 response = quickscraper_client.getHtml(
     'http://httpbin.org/ip', country_code='US')
-print(response.text)
+print(response._content)
 ```
 
 ### Premium Residential/Mobile Proxy Pools
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
 response = quickscraper_client.getHtml('http://httpbin.org/ip', premium=True)
-print(response.text)
+print(response._content)
 ```
 
 ### Device Type
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
 response = quickscraper_client.getHtml('http://httpbin.org/ip', device_type='mobile')
-print(response.text)
+print(response._content)
 ```
 
 ### Account Information
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
@@ -105,15 +105,40 @@
 
 ### Parser Addon
 
 ```python
 from quickscraper_sdk import QuickScraper
 quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
 response = quickscraper_client.getHtml('http://httpbin.org/ip', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
-print(response.text)
+print(response._content)
+```
+
+### Webhook Addon
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getHtml('http://httpbin.org/ip', webhookRequestId='WEBHOOK_ID')
+print(response._content)
+```
+### Get JSON from data
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.getData('http://httpbin.org/ip', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
+print(response._content)
+```
+### Write CSV, EXCEL to file from data
+
+```python
+from quickscraper_sdk import QuickScraper
+quickscraper_client = QuickScraper('YOUR_ACCESS_TOKEN')
+response = quickscraper_client.writeHtmlToFile('http://httpbin.org/ip', file_path='YOUR_FILE_PATH', parserSubscriptionId='PARSER_SUBSCRIPTION_ID')
+print(response._content)
 ```
 
 
 ## Do you need an expert?
 
 Are you finding a developer for your world-class product? If yes, please contact here.
 Originally by [QuickScraper Developers - app@quickscraper.co](mailto:app@quickscraper.co).
```

## Comparing `quickscraper_sdk-1.0.8.dist-info/RECORD` & `quickscraper_sdk-1.0.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-quickscraper_sdk/__init__.py,sha256=lwnqf1c2Y0E095GJZH_PlqtkCthCnA0I7kA2-JKS_EI,7613
-quickscraper_sdk/constant.py,sha256=nQJogsgXk2AlxErLQla0_lruywYZ06ZDTaulupZdT4k,272
+quickscraper_sdk/__init__.py,sha256=m8TF4hZaCvVNWddAjmvFCmKCudzrxxdHixKGbPgijiQ,8851
+quickscraper_sdk/constant.py,sha256=qdecmtVe3tbYkB1Ac3flZFLoJJiNnILJ9HR7h21H3Rs,272
 tests/__init__.py,sha256=FspmhViTO62HL15bC5o4qXWEALYaCRXsIaPi6Suj_Ls,70
 tests/constant.py,sha256=2r5201gu1BXxBJgSddaIK8vKhAdLUxkhnG_veOpv0_Q,192
 tests/test_cases.py,sha256=mrO6M4vbqp4Sekt4uHUnOPKyyhyVxPyVX1xjN3fhMzk,5250
-quickscraper_sdk-1.0.8.dist-info/LICENSE,sha256=DfrJyVjirZSu1qGS0tb7LR8OFpCVBJqaUM27NSvA9Ug,1092
-quickscraper_sdk-1.0.8.dist-info/METADATA,sha256=Kyve3nq31NNGbBZaBazIBRW9cbWenSyLlGUM5GVBHa0,3225
-quickscraper_sdk-1.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-quickscraper_sdk-1.0.8.dist-info/top_level.txt,sha256=QkNMMYAEdAj6OURlUcHxYLG5ZMoiRfYfyNPgxD8JLFY,23
-quickscraper_sdk-1.0.8.dist-info/RECORD,,
+quickscraper_sdk-1.0.9.dist-info/LICENSE,sha256=DfrJyVjirZSu1qGS0tb7LR8OFpCVBJqaUM27NSvA9Ug,1092
+quickscraper_sdk-1.0.9.dist-info/METADATA,sha256=pGEcQqD9RLJzofDKuiOyRqQVO1GWqwWtP92J4rNaqmA,4126
+quickscraper_sdk-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+quickscraper_sdk-1.0.9.dist-info/top_level.txt,sha256=QkNMMYAEdAj6OURlUcHxYLG5ZMoiRfYfyNPgxD8JLFY,23
+quickscraper_sdk-1.0.9.dist-info/RECORD,,
```

