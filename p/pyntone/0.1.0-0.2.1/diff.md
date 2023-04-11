# Comparing `tmp/pyntone-0.1.0.tar.gz` & `tmp/pyntone-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntone-0.1.0.tar", last modified: Mon Apr 10 04:12:34 2023, max compression
+gzip compressed data, was "pyntone-0.2.1.tar", last modified: Tue Apr 11 15:04:10 2023, max compression
```

## Comparing `pyntone-0.1.0.tar` & `pyntone-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.182644 pyntone-0.1.0/
--rw-rw-rw-   0        0        0     1083 2022-10-20 13:41:34.000000 pyntone-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      435 2023-04-10 04:12:34.183066 pyntone-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.135632 pyntone-0.1.0/pyntone/
--rw-rw-rw-   0        0        0       91 2023-04-10 02:19:52.000000 pyntone-0.1.0/pyntone/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.166633 pyntone-0.1.0/pyntone/client/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:31:49.000000 pyntone-0.1.0/pyntone/client/__init__.py
--rw-rw-rw-   0        0        0     1924 2023-04-06 13:14:42.000000 pyntone-0.1.0/pyntone/client/bulk_request_client.py
--rw-rw-rw-   0        0        0    17136 2023-04-10 02:14:45.000000 pyntone-0.1.0/pyntone/client/record_client.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.170674 pyntone-0.1.0/pyntone/http/
--rw-rw-rw-   0        0        0        0 2022-02-26 06:27:39.000000 pyntone-0.1.0/pyntone/http/__init__.py
--rw-rw-rw-   0        0        0     1767 2023-04-05 14:54:36.000000 pyntone-0.1.0/pyntone/http/http_client.py
--rw-rw-rw-   0        0        0     6265 2023-04-09 12:25:24.000000 pyntone-0.1.0/pyntone/kintone_request_config_builder.py
--rw-rw-rw-   0        0        0     1262 2023-04-06 08:39:46.000000 pyntone-0.1.0/pyntone/kintone_rest_api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.176636 pyntone-0.1.0/pyntone/types/
--rw-rw-rw-   0        0        0      136 2023-04-07 07:20:19.000000 pyntone-0.1.0/pyntone/types/__init__.py
--rw-rw-rw-   0        0        0      522 2023-04-09 12:10:39.000000 pyntone-0.1.0/pyntone/types/auth.py
--rw-rw-rw-   0        0        0      966 2023-04-07 12:27:01.000000 pyntone-0.1.0/pyntone/types/record.py
--rw-rw-rw-   0        0        0      340 2023-03-12 12:27:40.000000 pyntone-0.1.0/pyntone/url.py
-drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.160633 pyntone-0.1.0/pyntone.egg-info/
--rw-rw-rw-   0        0        0      435 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-10 04:12:34.000000 pyntone-0.1.0/pyntone.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-09 12:28:30.000000 pyntone-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      556 2023-04-10 04:12:34.184634 pyntone-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 04:12:34.179633 pyntone-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2023-03-22 13:21:21.000000 pyntone-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     5872 2023-04-09 12:12:22.000000 pyntone-0.1.0/tests/record.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.517274 pyntone-0.2.1/
+-rw-rw-rw-   0        0        0     1083 2022-10-20 13:41:34.000000 pyntone-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      435 2023-04-11 15:04:10.517274 pyntone-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.471290 pyntone-0.2.1/pyntone/
+-rw-rw-rw-   0        0        0       91 2023-04-11 15:02:11.000000 pyntone-0.2.1/pyntone/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.503274 pyntone-0.2.1/pyntone/client/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:31:49.000000 pyntone-0.2.1/pyntone/client/__init__.py
+-rw-rw-rw-   0        0        0     1924 2023-04-11 15:00:31.000000 pyntone-0.2.1/pyntone/client/bulk_request_client.py
+-rw-rw-rw-   0        0        0    19740 2023-04-10 13:44:05.000000 pyntone-0.2.1/pyntone/client/record_client.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.506274 pyntone-0.2.1/pyntone/http/
+-rw-rw-rw-   0        0        0        0 2022-02-26 06:27:39.000000 pyntone-0.2.1/pyntone/http/__init__.py
+-rw-rw-rw-   0        0        0     1769 2023-04-11 15:00:54.000000 pyntone-0.2.1/pyntone/http/http_client.py
+-rw-rw-rw-   0        0        0     6251 2023-04-11 15:00:14.000000 pyntone-0.2.1/pyntone/kintone_request_config_builder.py
+-rw-rw-rw-   0        0        0     1262 2023-04-11 15:01:21.000000 pyntone-0.2.1/pyntone/kintone_rest_api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.511275 pyntone-0.2.1/pyntone/types/
+-rw-rw-rw-   0        0        0      136 2023-04-07 07:20:19.000000 pyntone-0.2.1/pyntone/types/__init__.py
+-rw-rw-rw-   0        0        0      488 2023-04-11 14:59:57.000000 pyntone-0.2.1/pyntone/types/auth.py
+-rw-rw-rw-   0        0        0      972 2023-04-11 15:01:15.000000 pyntone-0.2.1/pyntone/types/record.py
+-rw-rw-rw-   0        0        0      340 2023-04-11 15:01:27.000000 pyntone-0.2.1/pyntone/url.py
+drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.497278 pyntone-0.2.1/pyntone.egg-info/
+-rw-rw-rw-   0        0        0      435 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-11 15:04:10.000000 pyntone-0.2.1/pyntone.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-09 12:28:30.000000 pyntone-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      536 2023-04-11 15:04:10.523274 pyntone-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 15:04:10.515274 pyntone-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-22 13:21:21.000000 pyntone-0.2.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     6260 2023-04-10 13:36:36.000000 pyntone-0.2.1/tests/record.py
```

### Comparing `pyntone-0.1.0/LICENSE` & `pyntone-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntone-0.1.0/pyntone/client/bulk_request_client.py` & `pyntone-0.2.1/pyntone/client/bulk_request_client.py`

 * *Files identical despite different names*

### Comparing `pyntone-0.1.0/pyntone/client/record_client.py` & `pyntone-0.2.1/pyntone/client/record_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
                                   UpdateRecordForParameter,
                                   UpdateRecordStatusParameter)
 from pyntone.url import build_path
 
 ADD_RECORDS_LIMIT = 100
 UPDATE_RECORDS_LIMIT = 100
 DELETE_RECORDS_LIMIT = 100
+GET_RECORDS_LIMIT = 500
 
 class RecordClient:
     def __init__(
         self,
         client: HttpClent,
         bulk_request_client: BulkRequestClient,
         guest_space_id: Union[int, str, None]
@@ -59,23 +60,38 @@
             id=record_id,
             update_key=update_key,
             record=record,
             revision=revision
         )
         return self.client.put(path, params)
 
-    # TODO
     def upsert_record(
         self,
         app: AppID,
         update_key: UpdateKey,
         record: Optional[RecordForParameter] = None,
         revision: Optional[Revision] = None
     ):
-        raise NotImplementedError()
+        query = '{} = "{}"'.format(update_key['field'], update_key['value'])
+        records = self.get_records(app, query=query)['records']
+        if len(records) > 0:
+            if records[0]['$id']['type'] == '__ID__':
+                result = self.update_record(app, update_key=update_key, record=record, revision=revision)
+                return {
+                    'id': records[0]['$id']['value'],
+                    'revision': result['revision']
+                }
+            raise Exception('Missing `$id` in `getRecords` response.')
+        return self.add_record(
+            app,
+            {
+            f"{update_key['field']}": { 'value': update_key['value'] },
+            **({} if record is None else record)
+        }
+        )
 
     def get_records(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
         query: Optional[str] = None,
         total_count: Optional[bool] = None
@@ -167,30 +183,71 @@
     
     def get_all_records_with_id(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
         condition: Optional[str] = None
     ):
-        raise NotImplementedError()
-
-    def __get_all_records_recursive_with_id(self):
-        raise NotImplementedError()
+        if fields is not None and len(fields) > 0 and not '$id' in fields:
+            fields.append('$id')
+        return self.__get_all_records_recursive_with_id(app, fields, condition, '0', [])
+
+    def __get_all_records_recursive_with_id(
+        self,
+        app: AppID,
+        fields: Optional[list[str]],
+        condition: Optional[str],
+        id: str,
+        records: list
+    ):
+        condition_query = f'({condition}) and ' if condition is not None else ''
+        query = f'{condition_query}$id > {id} order by $id asc limit {GET_RECORDS_LIMIT}'
+        result = self.get_records(app, fields, query)
+        all_records = records + result['records']
+        if len(result['records']) < GET_RECORDS_LIMIT:
+            return all_records
+        last_record = result['records'][-1]
+        if last_record['$id']['type'] == '__ID__':
+            last_id = last_record['$id']['value']
+            return self.__get_all_records_recursive_with_id(app, fields, condition, last_id, all_records)
+        raise Exception('Missing `$id` in `getRecords` response.')
     
     def get_all_records_with_offset(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
         condition: Optional[str] = None,
         order_by: Optional[str] = None,
     ):
-        raise NotImplementedError()
+        return self.__get_all_records_recursive_with_offset(app, fields, condition, order_by, 0, [])
 
-    def __get_all_records_recursive_with_offset(self):
-        raise NotImplementedError()
+    def __get_all_records_recursive_with_offset(
+        self,
+        app: AppID,
+        fields: Optional[list[str]],
+        condition: Optional[str],
+        order_by: Optional[str],
+        offset: int,
+        records: list
+    ):
+        condition_query = f'{condition} ' if condition is not None else ''
+        order_by_query = f'order by {order_by} ' if order_by is not None else ''
+        query = f'{condition_query}{order_by_query}limit {GET_RECORDS_LIMIT} offset {offset}'
+        result = self.get_records(app, fields, query)
+        all_records = records + result['records']
+        if len(result['records']) < GET_RECORDS_LIMIT:
+            return all_records
+        return self.__get_all_records_recursive_with_offset(
+            app,
+            fields,
+            condition,
+            order_by,
+            offset + GET_RECORDS_LIMIT,
+            all_records
+        )
 
     def get_all_records_with_cursor(
         self,
         app: AppID,
         fields: Optional[list[str]] = None,
         query: Optional[str] = None
     ) -> list:
```

### Comparing `pyntone-0.1.0/pyntone/http/http_client.py` & `pyntone-0.2.1/pyntone/http/http_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any
 
 import requests
+
 from pyntone.kintone_request_config_builder import (
     HttpMethod, KintoneRequestConfigBuilder, KintoneRequestParams)
 
 
 class KintoneError(Exception):
     def __init__(self, message, text, json, status_code) -> None:
         self.text = text
```

### Comparing `pyntone-0.1.0/pyntone/kintone_request_config_builder.py` & `pyntone-0.2.1/pyntone/kintone_request_config_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import base64
 import json
+from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Optional, Union
 from urllib.parse import urljoin
-from dataclasses import dataclass
-
-from pydantic import BaseModel
 
 from pyntone.types import AppID, CommentID, RecordID, Revision
 from pyntone.types.auth import ApiTokenAuth, DiscriminatedAuth, PasswordAuth
 from pyntone.types.record import (Comment, RecordForParameter, UpdateKey,
                                   UpdateKeyRecordForParameter,
                                   UpdateRecordForParameter,
                                   UpdateRecordStatusParameter)
@@ -55,14 +53,15 @@
             'headers': self._build_headers(method, self.auth),
         }
         if method == HttpMethod.GET:
             url_params: Any = {
                 'app': params.app
             }
             if params.id is not None: url_params['id'] = params.id
+            if params.query is not None: url_params['query'] = params.query
             if params.fields is not None:
                 for index, v in enumerate(params.fields):
                     url_params[f'fields[{index}]'] = v
             if params.total_count is not None: url_params['totalCount'] = str(params.total_count).lower()
             if params.record is not None: url_params['record'] = params.record
             if params.order is not None: url_params['order'] = params.order
             if params.offset is not None: url_params['offset'] = params.offset
@@ -100,23 +99,19 @@
                 'app': params.app
             }
             if params.id is not None: payload['id'] = params.id
             if params.ids is not None: payload['ids'] = params.ids
             if params.revisions is not None: payload['revisions'] = params.revisions
             if params.comment is not None: payload['comment'] = params.comment
             if params.record is not None: payload['record'] = params.record
-
             config['data'] = json.dumps(payload)
         else:
             raise RuntimeError()
         
         return config
-
-    def _convert_data(self, data: dict) -> dict:
-        return { key: { 'value': val } for key, val in data.items() }
     
     def _build_headers(self, method: HttpMethod, auth: DiscriminatedAuth) -> dict[str, str]:
         if type(auth) is ApiTokenAuth:
             api_token = auth.api_token
             if type(api_token) is not str:
                 api_token = ','.join(api_token)
 
@@ -135,8 +130,8 @@
                 'X-Cybozu-Authorization':b64_pass,
             }
             if method != HttpMethod.GET:
                 headers['Content-Type'] = 'application/json'
 
             return headers
         else:
-            raise NotImplementedError('未実装')
+            raise NotImplementedError('Unimplemented authentication method. Please use ApiTokenAuth or PasswordAuth.')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyntone-0.1.0/pyntone/kintone_rest_api_client.py` & `pyntone-0.2.1/pyntone/kintone_rest_api_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from typing import Optional, TypedDict, Union
 
-from pyntone.client.record_client import RecordClient
 from pyntone.client.bulk_request_client import BulkRequestClient
+from pyntone.client.record_client import RecordClient
 from pyntone.http.http_client import HttpClent
 from pyntone.kintone_request_config_builder import KintoneRequestConfigBuilder
 from pyntone.types.auth import DiscriminatedAuth
 
 
 class FeatureFlags(TypedDict):
     enableAbortSearchError: bool
```

### Comparing `pyntone-0.1.0/pyntone/types/record.py` & `pyntone-0.2.1/pyntone/types/record.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import TypedDict, Union, Optional, Literal
+from typing import Literal, TypedDict, Union
+
 from pyntone.types import RecordID, Revision
 
+
 class RecordItem(TypedDict):
     value: Union[int, str]
 
 RecordForParameter = dict[str, RecordItem]
 
 class UpdateKey(TypedDict):
     field: str
-    value: str
+    value: Union[int, str]
 
 class UpdateRecordForParameter(TypedDict, total=False):
     id: RecordID
     record: RecordForParameter
     revision: Revision
 
 class UpdateKeyRecordForParameter(TypedDict, total=False):
```

### Comparing `pyntone-0.1.0/pyntone.egg-info/SOURCES.txt` & `pyntone-0.2.1/pyntone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyntone-0.1.0/setup.cfg` & `pyntone-0.2.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796e 746f 6e65 0d0a 7665 7273   = pyntone..vers
-00000020: 696f 6e20 3d20 302e 312e 300d 0a64 6573  ion = 0.1.0..des
+00000020: 696f 6e20 3d20 302e 322e 310d 0a64 6573  ion = 0.2.1..des
 00000030: 6372 6970 7469 6f6e 203d 204b 696e 746f  cription = Kinto
 00000040: 6e65 2052 6573 7420 4150 4920 5772 6170  ne Rest API Wrap
 00000050: 7065 720d 0a75 726c 203d 2068 7474 7073  per..url = https
 00000060: 3a2f 2f67 6974 6875 622e 636f 6d2f 6b61  ://github.com/ka
 00000070: 7368 6930 332f 7079 6e74 6f6e 650d 0a6c  shi03/pyntone..l
 00000080: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
 00000090: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
@@ -23,13 +23,12 @@
 00000160: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
 00000170: 6e20 3a3a 2033 2e39 0d0a 0950 726f 6772  n :: 3.9...Progr
 00000180: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
 00000190: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
 000001a0: 300d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  0....[options]..
 000001b0: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
 000001c0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
-000001d0: 6573 203d 200d 0a09 7079 6461 6e74 6963  es = ...pydantic
-000001e0: 203e 3d20 312e 392e 300d 0a09 7265 7175   >= 1.9.0...requ
-000001f0: 6573 7473 203e 3d20 322e 3237 2e31 0d0a  ests >= 2.27.1..
-00000200: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000210: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000220: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+000001d0: 6573 203d 200d 0a09 7265 7175 6573 7473  es = ...requests
+000001e0: 203e 3d20 322e 3237 2e31 0d0a 0d0a 5b65   >= 2.27.1....[e
+000001f0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000200: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000210: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `pyntone-0.1.0/tests/record.py` & `pyntone-0.2.1/tests/record.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 from os import environ as env
+from uuid import uuid4
 
 import dotenv
 import pytest
-
 from pyntone import KintoneRestAPIClient
 from pyntone.types.auth import ApiTokenAuth
 
 
 @pytest.fixture(autouse=True, scope='session')
 def load_env():
     if os.path.exists('.env'):
@@ -20,152 +20,163 @@
         base_url=env['BASE_URL'],
         auth=auth
     )
     return client
 
 def test_add_record(client):
     add_record = {
-        'column1': { 'value': 'hello' },
+        'column1': { 'value': str(uuid4()) },
         'column2': { 'value': 'world' }
     }
     result = client.record.add_record(env['APP_ID'], add_record)
     assert result.get('id') is not None
     assert result.get('revision') is not None
 
 def test_get_record(client):
+    value = str(uuid4())
     add_record = {
-        'column1': { 'value': 'hello' },
+        'column1': { 'value': value },
         'column2': { 'value': 'world' }
     }
     result = client.record.add_record(env['APP_ID'], add_record)
     resp = client.record.get_record(env['APP_ID'], result['id'])
-    assert resp['record']['column1']['value'] == 'hello'
+    assert resp['record']['column1']['value'] == value
     assert resp['record']['column2']['value'] == 'world'
 
 def test_update_record(client):
     add_record = {
-        'column1': { 'value': 'hello' },
+        'column1': { 'value': str(uuid4()) },
         'column2': { 'value': 'world' }
     }
     add_result = client.record.add_record(env['APP_ID'], add_record)
     update_record = {
-        'column1': { 'value': 'hoge' }
+        'column1': { 'value': str(uuid4()) }
     }
     update_result = client.record.update_record(
         1,
         record_id=add_result['id'],
         record=update_record,
         revision=add_result['revision']
     )
     assert update_result.get('revision') is not None
 
+def test_upsert_record(client):
+    record = {
+        'column2': { 'value': 'upsert' }
+    }
+    update_key = {
+        'field': 'column1',
+        'value': str(uuid4())
+    }
+    client.record.upsert_record(env['APP_ID'], update_key, record)
+
 def test_get_all_records_with_cursor(client):
     client.record.get_all_records_with_cursor(env['APP_ID'])
     assert True
 
 def test_add_all_records(client):
     add_records_num = 400
     add_records = [
         {
-            'column1': { 'value': 'hello' },
+            'column1': { 'value': str(uuid4()) },
             'column2': { 'value': 'world' }
-        }
-    ] * add_records_num
+        } for _ in range(add_records_num)
+    ]
     results = client.record.add_all_records(env['APP_ID'], add_records)
     assert len(results['records']) == add_records_num
 
 def test_update_all_records(client):
     add_records_num = 400
     add_records = [
         {
-            'column1': { 'value': 'hello' },
+            'column1': { 'value': str(uuid4()) },
             'column2': { 'value': 'world' }
-        }
-    ] * add_records_num
+        } for _ in range(add_records_num)
+    ]
     results = client.record.add_all_records(env['APP_ID'], add_records)
     
     update_records = []
     for i in results['records']:
         update_records.append({
             'id': i['id'],
             'record': {
-                'column1': { 'value': 'hoge' },
+                'column1': { 'value': str(uuid4()) },
                 'column2': { 'value': 'fuga' }
             },
             'revision': i['revision']
         })
     results = client.record.update_all_records(env['APP_ID'], update_records)
     assert len(results['records']) == add_records_num
 
 def test_delete_all_reocrds(client):
     add_records_num = 400
     add_records = [
         {
-            'column1': { 'value': 'hello' },
+            'column1': { 'value': str(uuid4()) },
             'column2': { 'value': 'world' }
-        }
-    ] * add_records_num
+        } for _ in range(add_records_num)
+    ]
     results = client.record.add_all_records(env['APP_ID'], add_records)
     
     delete_records = []
     for i in results['records']:
         delete_records.append({
             'id': i['id'],
             # 'revision': i['revision']
         })
     results = client.record.delete_all_reocrds(env['APP_ID'], delete_records)
     assert results == {}
 
 def test_add_record_comment(client):
     add_record = {
-        'column1': { 'value': 'hello' },
+        'column1': { 'value': str(uuid4()) },
         'column2': { 'value': 'world' }
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
     add_comment = {
         'text': 'test comment'
     }
     add_comment_result = client.record.add_record_comment(env['APP_ID'], add_record_result.get('id'), add_comment)
     assert add_comment_result.get('id') is not None
 
 def test_delete_record_comment(client):
     add_record = {
-        'column1': { 'value': 'delete comment' },
+        'column1': { 'value': str(uuid4()) },
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
     add_comment = {
         'text': 'test comment'
     }
     add_comment_result = client.record.add_record_comment(env['APP_ID'], add_record_result['id'], add_comment)
     delete_comment_result = client.record.delete_record_comment(env['APP_ID'], add_record_result['id'], add_comment_result['id'])
     assert delete_comment_result == {}
 
 def test_get_record_comments(client):
     add_record = {
-        'column1': { 'value': 'get comment' },
+        'column1': { 'value': str(uuid4()) },
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
     add_comment = {
         'text': 'test comment'
     }
     add_comment_result = client.record.add_record_comment(env['APP_ID'], add_record_result['id'], add_comment)
     get_comment_result = client.record.get_record_comments(env['APP_ID'], add_record_result['id'])
     import json
     with open('test.json', 'w', encoding='utf-8') as f:
         json.dump(get_comment_result, f, indent=2)
     assert get_comment_result['comments'][0]['text'] == 'test comment '
 
 def test_update_record_assigness(client):
     add_record = {
-        'column1': { 'value': 'hello' },
+        'column1': { 'value': str(uuid4()) },
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
     result = client.record.update_record_assigness(env['APP_ID'], add_record_result['id'], ['testuser'])
     assert result.get('revision') is not None
 
 def test_update_record_status(client):
     add_record = {
-        'column1': { 'value': 'hello' },
+        'column1': { 'value': str(uuid4()) },
     }
     add_record_result = client.record.add_record(env['APP_ID'], add_record)
     result = client.record.update_record_status(env['APP_ID'], add_record_result['id'], '処理開始')
     assert result.get('revision') is not None
```

