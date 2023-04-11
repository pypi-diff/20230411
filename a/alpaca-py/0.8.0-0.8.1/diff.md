# Comparing `tmp/alpaca-py-0.8.0.tar.gz` & `tmp/alpaca_py-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca-py-0.8.0.tar", max compression
+gzip compressed data, was "alpaca_py-0.8.1.tar", max compression
```

## Comparing `alpaca-py-0.8.0.tar` & `alpaca_py-0.8.1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0    10872 2023-04-03 14:56:39.297899 alpaca-py-0.8.0/LICENSE
--rw-r--r--   0        0        0     9810 2023-04-03 14:56:39.298036 alpaca-py-0.8.0/README.md
--rw-r--r--   0        0        0       22 2023-04-03 14:56:39.298169 alpaca-py-0.8.0/alpaca/__init__.py
--rw-r--r--   0        0        0      100 2023-04-03 14:56:39.298311 alpaca-py-0.8.0/alpaca/broker/__init__.py
--rw-r--r--   0        0        0    64340 2023-04-03 14:56:39.298569 alpaca-py-0.8.0/alpaca/broker/client.py
--rw-r--r--   0        0        0    11012 2023-04-03 14:56:39.298706 alpaca-py-0.8.0/alpaca/broker/enums.py
--rw-r--r--   0        0        0      138 2023-04-03 14:56:39.298827 alpaca-py-0.8.0/alpaca/broker/models/__init__.py
--rw-r--r--   0        0        0    13998 2023-04-03 14:56:39.298969 alpaca-py-0.8.0/alpaca/broker/models/accounts.py
--rw-r--r--   0        0        0    14499 2023-04-03 14:56:39.299108 alpaca-py-0.8.0/alpaca/broker/models/cip.py
--rw-r--r--   0        0        0     6266 2023-04-03 14:56:39.299219 alpaca-py-0.8.0/alpaca/broker/models/documents.py
--rw-r--r--   0        0        0     4372 2023-04-03 14:56:39.299327 alpaca-py-0.8.0/alpaca/broker/models/funding.py
--rw-r--r--   0        0        0     3216 2023-04-03 14:56:39.299426 alpaca-py-0.8.0/alpaca/broker/models/journals.py
--rw-r--r--   0        0        0      305 2023-04-03 14:56:39.299514 alpaca-py-0.8.0/alpaca/broker/models/trading.py
--rw-r--r--   0        0        0    43935 2023-04-03 14:56:39.299781 alpaca-py-0.8.0/alpaca/broker/requests.py
--rw-r--r--   0        0        0      136 2023-04-03 14:56:39.299924 alpaca-py-0.8.0/alpaca/common/__init__.py
--rw-r--r--   0        0        0      347 2023-04-03 14:56:39.300018 alpaca-py-0.8.0/alpaca/common/constants.py
--rw-r--r--   0        0        0     1705 2023-04-03 14:56:39.300106 alpaca-py-0.8.0/alpaca/common/enums.py
--rw-r--r--   0        0        0      987 2023-04-03 14:56:39.300203 alpaca-py-0.8.0/alpaca/common/exceptions.py
--rw-r--r--   0        0        0      403 2023-04-03 14:56:39.300291 alpaca-py-0.8.0/alpaca/common/models.py
--rw-r--r--   0        0        0     1991 2023-04-03 14:56:39.300428 alpaca-py-0.8.0/alpaca/common/requests.py
--rw-r--r--   0        0        0    13961 2023-04-03 14:56:39.300571 alpaca-py-0.8.0/alpaca/common/rest.py
--rw-r--r--   0        0        0      173 2023-04-03 14:56:39.300660 alpaca-py-0.8.0/alpaca/common/types.py
--rw-r--r--   0        0        0     1916 2023-04-03 14:56:39.300743 alpaca-py-0.8.0/alpaca/common/utils.py
--rw-r--r--   0        0        0    17332 2023-04-03 14:56:39.300876 alpaca-py-0.8.0/alpaca/common/websocket.py
--rw-r--r--   0        0        0      118 2023-04-03 14:56:39.301001 alpaca-py-0.8.0/alpaca/data/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-03 14:56:39.301111 alpaca-py-0.8.0/alpaca/data/enums.py
--rw-r--r--   0        0        0       92 2023-04-03 14:56:39.301255 alpaca-py-0.8.0/alpaca/data/historical/__init__.py
--rw-r--r--   0        0        0    14142 2023-04-03 14:56:39.301369 alpaca-py-0.8.0/alpaca/data/historical/crypto.py
--rw-r--r--   0        0        0    12392 2023-04-03 14:56:39.301458 alpaca-py-0.8.0/alpaca/data/historical/stock.py
--rw-r--r--   0        0        0     4474 2023-04-03 14:56:39.301544 alpaca-py-0.8.0/alpaca/data/historical/utils.py
--rw-r--r--   0        0        0       72 2023-04-03 14:56:39.301643 alpaca-py-0.8.0/alpaca/data/live/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-03 14:56:39.301714 alpaca-py-0.8.0/alpaca/data/live/crypto.py
--rw-r--r--   0        0        0     1935 2023-04-03 14:56:39.301787 alpaca-py-0.8.0/alpaca/data/live/stock.py
--rw-r--r--   0        0        0     1012 2023-04-03 14:56:39.301862 alpaca-py-0.8.0/alpaca/data/mappings.py
--rw-r--r--   0        0        0      115 2023-04-03 14:56:39.301954 alpaca-py-0.8.0/alpaca/data/models/__init__.py
--rw-r--r--   0        0        0     2304 2023-04-03 14:56:39.302030 alpaca-py-0.8.0/alpaca/data/models/bars.py
--rw-r--r--   0        0        0     1752 2023-04-03 14:56:39.302103 alpaca-py-0.8.0/alpaca/data/models/base.py
--rw-r--r--   0        0        0     1643 2023-04-03 14:56:39.302201 alpaca-py-0.8.0/alpaca/data/models/orderbooks.py
--rw-r--r--   0        0        0     2581 2023-04-03 14:56:39.302326 alpaca-py-0.8.0/alpaca/data/models/quotes.py
--rw-r--r--   0        0        0     1979 2023-04-03 14:56:39.302405 alpaca-py-0.8.0/alpaca/data/models/snapshots.py
--rw-r--r--   0        0        0     2318 2023-04-03 14:56:39.302478 alpaca-py-0.8.0/alpaca/data/models/trades.py
--rw-r--r--   0        0        0    12288 2023-04-03 14:56:39.302571 alpaca-py-0.8.0/alpaca/data/requests.py
--rw-r--r--   0        0        0     4303 2023-04-03 14:56:39.303466 alpaca-py-0.8.0/alpaca/data/timeframe.py
--rw-r--r--   0        0        0        0 2023-04-03 14:56:39.303525 alpaca-py-0.8.0/alpaca/py.typed
--rw-r--r--   0        0        0       89 2023-04-03 14:56:39.303645 alpaca-py-0.8.0/alpaca/trading/__init__.py
--rw-r--r--   0        0        0    21010 2023-04-03 14:56:39.303935 alpaca-py-0.8.0/alpaca/trading/client.py
--rw-r--r--   0        0        0     7758 2023-04-03 14:56:39.304051 alpaca-py-0.8.0/alpaca/trading/enums.py
--rw-r--r--   0        0        0    23324 2023-04-03 14:56:39.304211 alpaca-py-0.8.0/alpaca/trading/models.py
--rw-r--r--   0        0        0    19232 2023-04-03 14:56:39.304453 alpaca-py-0.8.0/alpaca/trading/requests.py
--rw-r--r--   0        0        0     7505 2023-04-03 14:56:39.304563 alpaca-py-0.8.0/alpaca/trading/stream.py
--rw-r--r--   0        0        0      915 2023-04-03 14:56:39.312835 alpaca-py-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    11027 2023-04-03 14:56:59.317808 alpaca-py-0.8.0/setup.py
--rw-r--r--   0        0        0    10765 2023-04-03 14:56:59.318307 alpaca-py-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    10872 2023-03-20 15:12:59.606686 alpaca_py-0.8.1/LICENSE
+-rw-r--r--   0        0        0     9810 2023-04-03 17:13:32.842661 alpaca_py-0.8.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-11 19:35:09.619996 alpaca_py-0.8.1/alpaca/__init__.py
+-rw-r--r--   0        0        0      100 2023-03-20 15:12:59.607787 alpaca_py-0.8.1/alpaca/broker/__init__.py
+-rw-r--r--   0        0        0    64825 2023-04-11 19:21:35.937449 alpaca_py-0.8.1/alpaca/broker/client.py
+-rw-r--r--   0        0        0    11012 2023-03-20 15:12:59.608585 alpaca_py-0.8.1/alpaca/broker/enums.py
+-rw-r--r--   0        0        0      138 2023-03-20 15:12:59.608839 alpaca_py-0.8.1/alpaca/broker/models/__init__.py
+-rw-r--r--   0        0        0    13998 2023-04-03 17:13:32.844395 alpaca_py-0.8.1/alpaca/broker/models/accounts.py
+-rw-r--r--   0        0        0    14499 2023-03-20 15:12:59.609458 alpaca_py-0.8.1/alpaca/broker/models/cip.py
+-rw-r--r--   0        0        0     6266 2023-03-20 15:12:59.609667 alpaca_py-0.8.1/alpaca/broker/models/documents.py
+-rw-r--r--   0        0        0     4372 2023-03-20 15:12:59.609845 alpaca_py-0.8.1/alpaca/broker/models/funding.py
+-rw-r--r--   0        0        0     3216 2023-04-03 17:13:32.845068 alpaca_py-0.8.1/alpaca/broker/models/journals.py
+-rw-r--r--   0        0        0      305 2023-03-20 15:12:59.610382 alpaca_py-0.8.1/alpaca/broker/models/trading.py
+-rw-r--r--   0        0        0    43935 2023-04-03 17:13:32.846078 alpaca_py-0.8.1/alpaca/broker/requests.py
+-rw-r--r--   0        0        0      136 2023-03-20 15:12:59.610982 alpaca_py-0.8.1/alpaca/common/__init__.py
+-rw-r--r--   0        0        0      347 2023-03-20 15:12:59.611141 alpaca_py-0.8.1/alpaca/common/constants.py
+-rw-r--r--   0        0        0     1705 2023-04-03 17:13:32.846674 alpaca_py-0.8.1/alpaca/common/enums.py
+-rw-r--r--   0        0        0      987 2023-03-20 15:12:59.611559 alpaca_py-0.8.1/alpaca/common/exceptions.py
+-rw-r--r--   0        0        0      403 2023-03-20 15:12:59.611781 alpaca_py-0.8.1/alpaca/common/models.py
+-rw-r--r--   0        0        0     1991 2023-03-20 15:12:59.612115 alpaca_py-0.8.1/alpaca/common/requests.py
+-rw-r--r--   0        0        0    13960 2023-04-11 19:21:35.938278 alpaca_py-0.8.1/alpaca/common/rest.py
+-rw-r--r--   0        0        0      173 2023-03-20 15:12:59.612704 alpaca_py-0.8.1/alpaca/common/types.py
+-rw-r--r--   0        0        0     1916 2023-03-20 15:12:59.612900 alpaca_py-0.8.1/alpaca/common/utils.py
+-rw-r--r--   0        0        0    17332 2023-03-20 15:12:59.613119 alpaca_py-0.8.1/alpaca/common/websocket.py
+-rw-r--r--   0        0        0      118 2023-03-20 15:12:59.613409 alpaca_py-0.8.1/alpaca/data/__init__.py
+-rw-r--r--   0        0        0     1968 2023-04-03 14:46:59.759940 alpaca_py-0.8.1/alpaca/data/enums.py
+-rw-r--r--   0        0        0       92 2023-03-20 15:12:59.613798 alpaca_py-0.8.1/alpaca/data/historical/__init__.py
+-rw-r--r--   0        0        0    14142 2023-04-03 14:46:59.761182 alpaca_py-0.8.1/alpaca/data/historical/crypto.py
+-rw-r--r--   0        0        0    12392 2023-03-20 15:12:59.614199 alpaca_py-0.8.1/alpaca/data/historical/stock.py
+-rw-r--r--   0        0        0     4474 2023-03-20 15:12:59.614356 alpaca_py-0.8.1/alpaca/data/historical/utils.py
+-rw-r--r--   0        0        0       72 2023-03-20 15:12:59.614560 alpaca_py-0.8.1/alpaca/data/live/__init__.py
+-rw-r--r--   0        0        0     1602 2023-04-03 17:13:34.312258 alpaca_py-0.8.1/alpaca/data/live/crypto.py
+-rw-r--r--   0        0        0     1935 2023-03-20 15:12:59.614841 alpaca_py-0.8.1/alpaca/data/live/stock.py
+-rw-r--r--   0        0        0     1012 2023-03-20 15:12:59.614987 alpaca_py-0.8.1/alpaca/data/mappings.py
+-rw-r--r--   0        0        0      115 2023-03-20 15:12:59.615222 alpaca_py-0.8.1/alpaca/data/models/__init__.py
+-rw-r--r--   0        0        0     2304 2023-03-20 15:12:59.615411 alpaca_py-0.8.1/alpaca/data/models/bars.py
+-rw-r--r--   0        0        0     1752 2023-03-20 15:12:59.615552 alpaca_py-0.8.1/alpaca/data/models/base.py
+-rw-r--r--   0        0        0     1643 2023-03-20 15:12:59.615704 alpaca_py-0.8.1/alpaca/data/models/orderbooks.py
+-rw-r--r--   0        0        0     2581 2023-03-20 15:12:59.615907 alpaca_py-0.8.1/alpaca/data/models/quotes.py
+-rw-r--r--   0        0        0     1979 2023-03-20 15:12:59.616060 alpaca_py-0.8.1/alpaca/data/models/snapshots.py
+-rw-r--r--   0        0        0     2318 2023-03-20 15:12:59.616284 alpaca_py-0.8.1/alpaca/data/models/trades.py
+-rw-r--r--   0        0        0    12288 2023-04-03 17:13:32.848638 alpaca_py-0.8.1/alpaca/data/requests.py
+-rw-r--r--   0        0        0     4303 2023-03-20 15:12:59.616739 alpaca_py-0.8.1/alpaca/data/timeframe.py
+-rw-r--r--   0        0        0        0 2023-03-20 15:12:59.616869 alpaca_py-0.8.1/alpaca/py.typed
+-rw-r--r--   0        0        0       89 2023-03-20 15:12:59.617081 alpaca_py-0.8.1/alpaca/trading/__init__.py
+-rw-r--r--   0        0        0    21010 2023-03-20 15:12:59.617276 alpaca_py-0.8.1/alpaca/trading/client.py
+-rw-r--r--   0        0        0     7758 2023-03-20 15:12:59.617427 alpaca_py-0.8.1/alpaca/trading/enums.py
+-rw-r--r--   0        0        0    25517 2023-04-11 19:30:55.555410 alpaca_py-0.8.1/alpaca/trading/models.py
+-rw-r--r--   0        0        0    19232 2023-03-20 15:12:59.617974 alpaca_py-0.8.1/alpaca/trading/requests.py
+-rw-r--r--   0        0        0     7505 2023-03-20 15:12:59.618140 alpaca_py-0.8.1/alpaca/trading/stream.py
+-rw-r--r--   0        0        0      915 2023-04-11 19:35:09.620743 alpaca_py-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 alpaca_py-0.8.1/PKG-INFO
```

### Comparing `alpaca-py-0.8.0/LICENSE` & `alpaca_py-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/README.md` & `alpaca_py-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/broker/client.py` & `alpaca_py-0.8.1/alpaca/broker/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import base64
-from typing import Callable, Iterator, List, Optional, Union
+from typing import Callable, Iterator, List, Optional, Union, Dict
 from uuid import UUID
 
 import sseclient
 
 from pydantic import parse_obj_as
 from requests import HTTPError, Response
 
@@ -46,14 +46,15 @@
     ACCOUNT_ACTIVITIES_DEFAULT_PAGE_SIZE,
     BROKER_DOCUMENT_UPLOAD_LIMIT,
 )
 from alpaca.common.enums import BaseURL, PaginationType
 from alpaca.trading.models import (
     PortfolioHistory,
     Position,
+    AllAccountsPositions,
     ClosePositionResponse,
     Asset,
     Watchlist,
     Calendar,
     Clock,
     CorporateActionAnnouncement,
     AccountConfiguration as TradeAccountConfiguration,
@@ -966,14 +967,30 @@
         response = self.get(f"/trading/accounts/{account_id}/positions")
 
         if self._use_raw_data:
             return response
 
         return parse_obj_as(List[Position], response)
 
+    def get_all_accounts_positions(
+        self,
+    ) -> Union[AllAccountsPositions, RawData]:
+        """
+        Gets all the current positions for every account in bulk.
+
+        Returns:
+            AllAccountsPositions: The collection of open positions keyed by account_id.
+        """
+        response = self.get("/accounts/positions")
+
+        if self._use_raw_data:
+            return response
+
+        return AllAccountsPositions(**response)
+
     def get_open_position_for_account(
         self, account_id: Union[UUID, str], symbol_or_asset_id: Union[UUID, str]
     ) -> Union[Position, RawData]:
         """
         Gets the open position for an account for a single asset. Throws an APIError if the position does not exist.
 
         Args:
@@ -1869,15 +1886,14 @@
 
         client = sseclient.SSEClient(response)
 
         for event in client.events():
             yield event.data
 
     def _get_sse_headers(self) -> dict:
-
         headers = self._get_default_headers()
 
         headers["Connection"] = "keep-alive"
         headers["Cache-Control"] = "no-cache"
         headers["Content-Type"] = "text/event-stream"
         headers["Accept"] = "text/event-stream"
```

### Comparing `alpaca-py-0.8.0/alpaca/broker/enums.py` & `alpaca_py-0.8.1/alpaca/broker/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/broker/models/accounts.py` & `alpaca_py-0.8.1/alpaca/broker/models/accounts.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/broker/models/cip.py` & `alpaca_py-0.8.1/alpaca/broker/models/cip.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/broker/models/documents.py` & `alpaca_py-0.8.1/alpaca/broker/models/documents.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/broker/models/funding.py` & `alpaca_py-0.8.1/alpaca/broker/models/funding.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/broker/models/journals.py` & `alpaca_py-0.8.1/alpaca/broker/models/journals.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/broker/requests.py` & `alpaca_py-0.8.1/alpaca/broker/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/common/enums.py` & `alpaca_py-0.8.1/alpaca/common/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/common/exceptions.py` & `alpaca_py-0.8.1/alpaca/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/common/requests.py` & `alpaca_py-0.8.1/alpaca/common/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/common/rest.py` & `alpaca_py-0.8.1/alpaca/common/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
         self,
         method: str,
         path: str,
         data: Optional[Union[dict, str]] = None,
         base_url: Optional[Union[BaseURL, str]] = None,
         api_version: Optional[str] = None,
     ) -> HTTPResult:
-
         """Prepares and submits HTTP requests to given API endpoint and returns response.
         Handles retrying if 429 (Rate Limit) error arises.
 
         Args:
             method (str): The API endpoint HTTP method
             path (str): The API endpoint path
             data (Optional[Union[dict, str]]): Either the payload in json format, query params urlencoded, or a dict
```

### Comparing `alpaca-py-0.8.0/alpaca/common/utils.py` & `alpaca_py-0.8.1/alpaca/common/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/common/websocket.py` & `alpaca_py-0.8.1/alpaca/common/websocket.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/enums.py` & `alpaca_py-0.8.1/alpaca/data/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/historical/crypto.py` & `alpaca_py-0.8.1/alpaca/data/historical/crypto.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/historical/stock.py` & `alpaca_py-0.8.1/alpaca/data/historical/stock.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/historical/utils.py` & `alpaca_py-0.8.1/alpaca/data/historical/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/live/crypto.py` & `alpaca_py-0.8.1/alpaca/data/live/crypto.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from alpaca.common.websocket import BaseStream
 from typing import Optional, Dict
 from alpaca.common.enums import BaseURL
+from alpaca.data.enums import CryptoFeed
 
 
 class CryptoDataStream(BaseStream):
     """
     A WebSocket client for streaming live crypto data.
 
     See BaseStream for more information on implementation and the methods available.
     """
 
     def __init__(
         self,
         api_key: str,
         secret_key: str,
         raw_data: bool = False,
+        feed: CryptoFeed = CryptoFeed.US,
         url_override: Optional[str] = None,
         websocket_params: Optional[Dict] = None,
     ) -> None:
         """
         Instantiates a WebSocket client for accessing live cryptocurrency data.
 
         Args:
@@ -29,14 +31,14 @@
             url_override (Optional[str]): If specified allows you to override the base url the client
               points to for proxy/testing. Defaults to None.
         """
         super().__init__(
             endpoint=(
                 url_override
                 if url_override is not None
-                else BaseURL.MARKET_DATA_STREAM.value + "/v1beta2/crypto"
+                else BaseURL.MARKET_DATA_STREAM.value + f"/v1beta3/crypto/{feed}"
             ),
             api_key=api_key,
             secret_key=secret_key,
             raw_data=raw_data,
             websocket_params=websocket_params,
         )
```

### Comparing `alpaca-py-0.8.0/alpaca/data/live/stock.py` & `alpaca_py-0.8.1/alpaca/data/live/stock.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/mappings.py` & `alpaca_py-0.8.1/alpaca/data/mappings.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/models/bars.py` & `alpaca_py-0.8.1/alpaca/data/models/bars.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/models/base.py` & `alpaca_py-0.8.1/alpaca/data/models/base.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/models/orderbooks.py` & `alpaca_py-0.8.1/alpaca/data/models/orderbooks.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/models/quotes.py` & `alpaca_py-0.8.1/alpaca/data/models/quotes.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/models/snapshots.py` & `alpaca_py-0.8.1/alpaca/data/models/snapshots.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/models/trades.py` & `alpaca_py-0.8.1/alpaca/data/models/trades.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/requests.py` & `alpaca_py-0.8.1/alpaca/data/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/data/timeframe.py` & `alpaca_py-0.8.1/alpaca/data/timeframe.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/trading/client.py` & `alpaca_py-0.8.1/alpaca/trading/client.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/trading/enums.py` & `alpaca_py-0.8.1/alpaca/trading/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/trading/models.py` & `alpaca_py-0.8.1/alpaca/trading/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from alpaca.common.models import ValidateBaseModel as BaseModel
 from uuid import UUID
 from datetime import datetime, date
-from typing import Any, Optional, List, Union
+from typing import Any, Optional, List, Union, Dict
 from alpaca.trading.enums import (
     AssetClass,
     AssetStatus,
     AssetExchange,
     DTBPCheck,
     OrderStatus,
     OrderType,
@@ -62,53 +62,107 @@
     fractionable: bool
     min_order_size: Optional[float] = None
     min_trade_increment: Optional[float] = None
     price_increment: Optional[float] = None
     maintenance_margin_requirement: Optional[float] = None
 
 
+class USDPositionValues(BaseModel):
+    """
+    Represents an open long or short holding in an asset in USD.
+
+    Attributes:
+        avg_entry_price (str): The average entry price of the position.
+        market_value (str): Total dollar amount of the position.
+        cost_basis (str): Total cost basis in dollars.
+        unrealized_pl (str): Unrealized profit/loss in dollars.
+        unrealized_plpc (str): Unrealized profit/loss percent.
+        unrealized_intraday_pl (str): Unrealized profit/loss in dollars for the day.
+        unrealized_intraday_plpc (str): Unrealized profit/loss percent for the day.
+        current_price (str): Current asset price per share.
+        lastday_price (str): Last day’s asset price per share based on the closing value of the last trading day.
+        change_today (str): Percent change from last day's price.
+
+    """
+
+    avg_entry_price: str
+    market_value: str
+    cost_basis: str
+    unrealized_pl: str
+    unrealized_plpc: str
+    unrealized_intraday_pl: str
+    unrealized_intraday_plpc: str
+    current_price: str
+    lastday_price: str
+    change_today: str
+
+
 class Position(BaseModel):
     """
     Represents an open long or short holding in an asset.
 
     Attributes:
         asset_id (UUID): ID of the asset.
         symbol (str): Symbol of the asset.
         exchange (AssetExchange): Exchange name of the asset.
         asset_class (AssetClass): Name of the asset's asset class.
+        asset_marginable (Optional[bool]): Indicates if this asset is marginable.
         avg_entry_price (str): The average entry price of the position.
         qty (str): The number of shares of the position.
         side (PositionSide): "long" or "short" representing the side of the position.
         market_value (str): Total dollar amount of the position.
         cost_basis (str): Total cost basis in dollars.
         unrealized_pl (str): Unrealized profit/loss in dollars.
         unrealized_plpc (str): Unrealized profit/loss percent.
         unrealized_intraday_pl (str): Unrealized profit/loss in dollars for the day.
         unrealized_intraday_plpc (str): Unrealized profit/loss percent for the day.
         current_price (str): Current asset price per share.
         lastday_price (str): Last day’s asset price per share based on the closing value of the last trading day.
         change_today (str): Percent change from last day's price.
+        swap_rate (Optional[str]): Swap rate is the exchange rate (without mark-up) used to convert the price into local currency or crypto asset.
+        avg_entry_swap_rate (Optional[str]): The average exchange rate the price was converted into the local currency at.
+        usd (USDPositionValues): Represents the position in USD values.
+        qty_available (Optional[str]): Total number of shares available minus open orders.
+
     """
 
     asset_id: UUID
     symbol: str
     exchange: AssetExchange
     asset_class: AssetClass
+    asset_marginable: Optional[bool]
     avg_entry_price: str
     qty: str
     side: PositionSide
     market_value: str
     cost_basis: str
     unrealized_pl: str
     unrealized_plpc: str
     unrealized_intraday_pl: str
     unrealized_intraday_plpc: str
     current_price: str
     lastday_price: str
     change_today: str
+    swap_rate: Optional[str]
+    avg_entry_swap_rate: Optional[str]
+    usd: Optional[USDPositionValues]
+    qty_available: Optional[str]
+
+
+class AllAccountsPositions(BaseModel):
+    """
+    Represents the positions of every account as of last market close.
+
+    Attributes:
+        as_of (datetime): Timestamp for which the positions are returned.
+        positions (Dict[str, List[Position]]): Positions held by an account, keyed by account_id.
+    """
+
+    as_of: datetime
+    positions: Dict[str, List[Position]]
 
 
 class Order(BaseModel):
     """
     Represents a request for the sale or purchase of an asset.
 
     Attributes:
```

### Comparing `alpaca-py-0.8.0/alpaca/trading/requests.py` & `alpaca_py-0.8.1/alpaca/trading/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/alpaca/trading/stream.py` & `alpaca_py-0.8.1/alpaca/trading/stream.py`

 * *Files identical despite different names*

### Comparing `alpaca-py-0.8.0/pyproject.toml` & `alpaca_py-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpaca-py"
-version = "0.8.0"
+version = "0.8.1"
 description = "The Official Python SDK for Alpaca APIs"
 authors = [
     "Rahul Chowdhury <rahul.chowdhury@alpaca.markets>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/alpacahq/alpaca-py"
```

### Comparing `alpaca-py-0.8.0/setup.py` & `alpaca_py-0.8.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,248 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: alpaca-py
+Version: 0.8.1
+Summary: The Official Python SDK for Alpaca APIs
+Home-page: https://github.com/alpacahq/alpaca-py
+License: Apache-2.0
+Author: Rahul Chowdhury
+Author-email: rahul.chowdhury@alpaca.markets
+Requires-Python: >=3.7.1,<4.0.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: msgpack (>=1.0.3,<2.0.0)
+Requires-Dist: pandas (>=1.3.5,<2.0.0)
+Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: sseclient-py (>=1.7.2,<2.0.0)
+Requires-Dist: websockets (>=10.2,<11.0)
+Project-URL: Documentation, https://alpaca.markets/docs/python-sdk/
+Project-URL: Repository, https://github.com/alpacahq/alpaca-py
+Description-Content-Type: text/markdown
 
-packages = \
-['alpaca',
- 'alpaca.broker',
- 'alpaca.broker.models',
- 'alpaca.common',
- 'alpaca.data',
- 'alpaca.data.historical',
- 'alpaca.data.live',
- 'alpaca.data.models',
- 'alpaca.trading']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['msgpack>=1.0.3,<2.0.0',
- 'pandas>=1.3.5,<2.0.0',
- 'pydantic>=1.9.0,<2.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'sseclient-py>=1.7.2,<2.0.0',
- 'websockets>=10.2,<11.0']
-
-setup_kwargs = {
-    'name': 'alpaca-py',
-    'version': '0.8.0',
-    'description': 'The Official Python SDK for Alpaca APIs',
-    'long_description': '[![Alpaca-py](https://github.com/alpacahq/alpaca-py/blob/master/docs/images/alpaca-py-banner.png?raw=true)](https://alpaca.markets/docs/python-sdk)\n\n[![Downloads](https://pepy.tech/badge/alpaca-py/month)](https://pepy.tech/project/alpaca-py)\n[![Python Versions](https://img.shields.io/pypi/pyversions/alpaca-py.svg?logo=python&logoColor=white)](https://pypi.org/project/alpaca-py)\n[![GitHub](https://img.shields.io/github/license/alpacahq/alpaca-py?color=blue)](https://github.com/alpacahq/alpaca-py/blob/master/LICENSE.md)\n[![PyPI](https://img.shields.io/pypi/v/alpaca-py?color=blue)](https://pypi.org/project/alpaca-py/)\n\n## Table of Contents\n* [About](#about)\n* [Documentation](#documentation)\n* [Installation](#installation)\n* [Update](#update)\n* [What\'s New?](#whats-new)\n   1. [Broker API](#broker-api-new)\n   2. [OOP Design](#oop-design)\n   3. [Data Validation](#data-validation)\n   4. [Many Clients](#many-clients)\n* [API Keys](#api-keys)\n   1. [Trading and Market Data API Keys](#trading-api-keys)\n   2. [Broker API Keys](#trading-api-keys)\n* [Usage](#usage)\n   1. [Broker API Example](#broker-api-example)\n   2. [Trading API Example](#trading-api-example)\n   3. [Market Data API Example](#data-api-example)\n* [Contributing](https://github.com/alpacahq/alpaca-py/blob/master/CONTRIBUTING.md)\n* [License](https://github.com/alpacahq/alpaca-py/blob/master/LICENSE)\n\n## About <a name="about"></a>\n\nAlpaca-py provides an interface for interacting with the API products Alpaca offers. These API products are provided as various REST, WebSocket and SSE endpoints that allow you to do everything from streaming market data to creating your own investment apps. \n\nLearn more about the API products Alpaca offers at https://alpaca.markets.\n\n## Documentation <a name="documentation"></a>\n\nAlpaca-py has a supplementary documentation site which contains references for all clients, methods and models found in this codebase. The documentation\nalso contains examples to get started with alpaca-py.\n\nYou can find the documentation site here: https://alpaca.markets/docs/python-sdk\n\n## Installation <a name="installation"></a>\n\nAlpaca-py is supported on Python 3.7+.  You can install Alpaca-py using pip.\n\nRun the following command in your terminal.\n\n```shell\n  pip install alpaca-py\n```\n\n## Update <a name="update"></a>\n\nIf you already have Alpaca-py installed, and would like to use the latest version available...\n\nRun the following command in your terminal:\n\n```shell\n  pip install alpaca-py --upgrade\n```\n\n## What’s New? <a name="whats-new"></a>\nIf you’ve used the previous python SDK alpaca-trade-api, there are a few key differences to be aware of.\n\n### Broker API <a name="broker-api-new"></a>\nAlpaca-py lets you use Broker API to start building your investment apps! Learn more at the [Broker](https://alpaca.markets/docs/python-sdk/broker.html) page.\n\n### OOP Design <a name="oop-design"></a>\nAlpaca-py uses a more OOP approach to submitting requests compared to the previous SDK. To submit a request, you will most likely need to create a request object containing the desired request data. Generally, there is a unique request model for each method. \n\nSome examples of request models corresponding to methods: \n\n* ``GetOrdersRequest`` for ``TradingClient.get_orders()``\n* ``CryptoLatestOrderbookRequest`` for ``CryptoHistoricalDataClient.get_crypto_latest_orderbook()``\n\n**Request Models Usage Example**\n\nTo get historical bar data for crypto, you will need to provide a ``CryptoBarsRequest`` object.\n\n```python\nfrom alpaca.data.historical import CryptoHistoricalDataClient\nfrom alpaca.data.requests import CryptoBarsRequest\nfrom alpaca.data.timeframe import TimeFrame\nfrom datetime import datetime\n\n# no keys required for crypto data\nclient = CryptoHistoricalDataClient()\n\nrequest_params = CryptoBarsRequest(\n                        symbol_or_symbols=["BTC/USD", "ETH/USD"],\n                        timeframe=TimeFrame.Day,\n                        start=datetime(2022, 7, 1)\n                 )\n\nbars = client.get_crypto_bars(request_params)\n```\n\n### Data Validation <a name="data-validation"></a>\nAlpaca-py uses *pydantic* to validate data models at run-time. This means if you are receiving request data via JSON from a client. You can handle parsing and validation through Alpaca’s request models. All request models can be instantiated by passing in data in dictionary format.\n\nHere is a rough example of what is possible.\n\n```python\n\n @app.route(\'/post_json\', methods=[\'POST\'])\n def do_trade():\n     # ...\n\n     order_data_json = request.get_json()\n\n     # validate data\n     MarketOrderRequest(**order_data_json)\n\n     # ...\n```\n\n### Many Clients <a name="many-clients"></a>\nAlpaca-py has a lot of client classes. There is a client for each API and even asset class specific clients (``StockHistoricalDataClient``, ``CryptoDataStream``). This requires you to pick and choose clients based on your needs.\n\n**Broker API:** ``BrokerClient``\n\n**Trading API:** ``TradingClient``\n\n**Market Data API:**  ``StockHistoricalDataClient``, ``CryptoHistoricalDataClient``, ``CryptoDataStream``, ``StockDataStream``\n\n## API Keys <a name="api-keys"></a>\n\n### Trading and Market Data API <a name="trading-api-keys"></a>\nIn order to use Alpaca’s services you’ll need to sign up for an Alpaca account and retrieve your API keys. Signing up is completely free and takes only a few minutes. Sandbox environments are available to test out the API. To use the sandbox environment, you will need to provide sandbox/paper keys. API keys are passed into Alpaca-py through either ``TradingClient``, ``StockHistoricalDataClient``, ``CryptoHistoricalDataClient``, ``StockDataStream``, or ``CryptoDataStream``.\n\n### Broker API <a name="broker-api-keys"></a>\nTo use the Broker API, you will need to sign up for a broker account and retrieve your Broker API keys. The API keys can be found on the dashboard once you’ve logged in. Alpaca also provides a sandbox environment to test out Broker API. To use the sandbox mode, provide your sandbox keys. Once you have your keys, you can pass them into ``BrokerClient`` to get started.\n\n## Usage <a name="usage"></a>\nAlpaca’s APIs allow you to do everything from building algorithmic trading strategies to building a full brokerage experience for your own end users. Here are some things you can do with Alpaca-py.\n\nTo view full descriptions and examples view the [documentation page](https://alpaca.markets/docs/python-sdk/index.html).\n\n**Market Data API**: Access live and historical market data for 5000+ stocks and 20+ crypto.\n\n**Trading API**: Trade stock and crypto with lightning fast execution speeds.\n\n**Broker API & Connect**: Build investment apps - from robo-advisors to brokerages.\n\n### Broker API Example <a name="broker-api-example"></a>\n\n**Listing All Accounts**\n\nThe ``BrokerClient.list_accounts`` method allows you to list all the brokerage accounts under your management. The method takes an optional parameter ``search_parameters`` which requires a ``ListAccountsRequest`` object. This parameter allows you to filter the list of accounts returned.\n\n```python\nfrom alpaca.broker.client import BrokerClient\nfrom alpaca.broker.requests import ListAccountsRequest\nfrom alpaca.broker.enums import AccountEntities\n\nbroker_client = BrokerClient(\'api-key\', \'secret-key\')\n\n# search for accounts created after January 30th 2022.\n# Response should contain Contact and Identity fields for each account.\nfilter = ListAccountsRequest(\n                    created_after=datetime.datetime.strptime("2022-01-30", "%Y-%m-%d"),\n                    entities=[AccountEntities.CONTACT, AccountEntities.IDENTITY]\n                    )\n\naccounts = broker_client.list_accounts(search_parameters=filter)\n```\n\n### Trading API Example <a name="trading-api-example"></a>\n\n**Submitting an Order**\n\nTo create an order on Alpaca-py you must use an ``OrderRequest`` object. There are different ``OrderRequest`` objects based on the type of order you want to make. For market orders, there is ``MarketOrderRequest``, limit orders have ``LimitOrderRequest``, stop orders ``StopOrderRequest``, and trailing stop orders have ``TrailingStopOrderRequest``. Each order type have their own required parameters for a successful order.\n\n\n```python\nfrom alpaca.trading.client import TradingClient\nfrom alpaca.trading.requests import MarketOrderRequest\nfrom alpaca.trading.enums import OrderSide, TimeInForce\n\ntrading_client = TradingClient(\'api-key\', \'secret-key\')\n\n\n# preparing order data\nmarket_order_data = MarketOrderRequest(\n                      symbol="BTC/USD",\n                      qty=0.0001,\n                      side=OrderSide.BUY,\n                      time_in_force=TimeInForce.DAY\n                  )\n\n# Market order\nmarket_order = trading_client.submit_order(\n                order_data=market_order_data\n                )\n```\n\n\n### Market Data API Example <a name="data-api-example"></a>\n**Querying Historical Bar Data**\n\nYou can request bar data via the HistoricalDataClients. In this example, we query daily bar data for “BTC/USD” and “ETH/USD” since July 1st 2022. You can convert the response to a multi-index pandas dataframe using the ``.df`` property.\n\n```python\nfrom alpaca.data.historical import CryptoHistoricalDataClient\nfrom alpaca.data.requests import CryptoBarsRequest\nfrom alpaca.data.timeframe import TimeFrame\nfrom datetime import datetime\n\n# no keys required for crypto data\nclient = CryptoHistoricalDataClient()\n\nrequest_params = CryptoBarsRequest(\n                        symbol_or_symbols=["BTC/USD", "ETH/USD"],\n                        timeframe=TimeFrame.Day,\n                        start=datetime.strptime("2022-07-01", \'%Y-%m-%d\')\n                        )\n\nbars = client.get_crypto_bars(request_params)\n\n# convert to dataframe\nbars.df\n\n```\n',
-    'author': 'Rahul Chowdhury',
-    'author_email': 'rahul.chowdhury@alpaca.markets',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/alpacahq/alpaca-py',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
+[![Alpaca-py](https://github.com/alpacahq/alpaca-py/blob/master/docs/images/alpaca-py-banner.png?raw=true)](https://alpaca.markets/docs/python-sdk)
 
+[![Downloads](https://pepy.tech/badge/alpaca-py/month)](https://pepy.tech/project/alpaca-py)
+[![Python Versions](https://img.shields.io/pypi/pyversions/alpaca-py.svg?logo=python&logoColor=white)](https://pypi.org/project/alpaca-py)
+[![GitHub](https://img.shields.io/github/license/alpacahq/alpaca-py?color=blue)](https://github.com/alpacahq/alpaca-py/blob/master/LICENSE.md)
+[![PyPI](https://img.shields.io/pypi/v/alpaca-py?color=blue)](https://pypi.org/project/alpaca-py/)
+
+## Table of Contents
+* [About](#about)
+* [Documentation](#documentation)
+* [Installation](#installation)
+* [Update](#update)
+* [What's New?](#whats-new)
+   1. [Broker API](#broker-api-new)
+   2. [OOP Design](#oop-design)
+   3. [Data Validation](#data-validation)
+   4. [Many Clients](#many-clients)
+* [API Keys](#api-keys)
+   1. [Trading and Market Data API Keys](#trading-api-keys)
+   2. [Broker API Keys](#trading-api-keys)
+* [Usage](#usage)
+   1. [Broker API Example](#broker-api-example)
+   2. [Trading API Example](#trading-api-example)
+   3. [Market Data API Example](#data-api-example)
+* [Contributing](https://github.com/alpacahq/alpaca-py/blob/master/CONTRIBUTING.md)
+* [License](https://github.com/alpacahq/alpaca-py/blob/master/LICENSE)
+
+## About <a name="about"></a>
+
+Alpaca-py provides an interface for interacting with the API products Alpaca offers. These API products are provided as various REST, WebSocket and SSE endpoints that allow you to do everything from streaming market data to creating your own investment apps. 
+
+Learn more about the API products Alpaca offers at https://alpaca.markets.
+
+## Documentation <a name="documentation"></a>
+
+Alpaca-py has a supplementary documentation site which contains references for all clients, methods and models found in this codebase. The documentation
+also contains examples to get started with alpaca-py.
+
+You can find the documentation site here: https://alpaca.markets/docs/python-sdk
+
+## Installation <a name="installation"></a>
+
+Alpaca-py is supported on Python 3.7+.  You can install Alpaca-py using pip.
+
+Run the following command in your terminal.
+
+```shell
+  pip install alpaca-py
+```
+
+## Update <a name="update"></a>
+
+If you already have Alpaca-py installed, and would like to use the latest version available...
+
+Run the following command in your terminal:
+
+```shell
+  pip install alpaca-py --upgrade
+```
+
+## What’s New? <a name="whats-new"></a>
+If you’ve used the previous python SDK alpaca-trade-api, there are a few key differences to be aware of.
+
+### Broker API <a name="broker-api-new"></a>
+Alpaca-py lets you use Broker API to start building your investment apps! Learn more at the [Broker](https://alpaca.markets/docs/python-sdk/broker.html) page.
+
+### OOP Design <a name="oop-design"></a>
+Alpaca-py uses a more OOP approach to submitting requests compared to the previous SDK. To submit a request, you will most likely need to create a request object containing the desired request data. Generally, there is a unique request model for each method. 
+
+Some examples of request models corresponding to methods: 
+
+* ``GetOrdersRequest`` for ``TradingClient.get_orders()``
+* ``CryptoLatestOrderbookRequest`` for ``CryptoHistoricalDataClient.get_crypto_latest_orderbook()``
+
+**Request Models Usage Example**
+
+To get historical bar data for crypto, you will need to provide a ``CryptoBarsRequest`` object.
+
+```python
+from alpaca.data.historical import CryptoHistoricalDataClient
+from alpaca.data.requests import CryptoBarsRequest
+from alpaca.data.timeframe import TimeFrame
+from datetime import datetime
+
+# no keys required for crypto data
+client = CryptoHistoricalDataClient()
+
+request_params = CryptoBarsRequest(
+                        symbol_or_symbols=["BTC/USD", "ETH/USD"],
+                        timeframe=TimeFrame.Day,
+                        start=datetime(2022, 7, 1)
+                 )
+
+bars = client.get_crypto_bars(request_params)
+```
+
+### Data Validation <a name="data-validation"></a>
+Alpaca-py uses *pydantic* to validate data models at run-time. This means if you are receiving request data via JSON from a client. You can handle parsing and validation through Alpaca’s request models. All request models can be instantiated by passing in data in dictionary format.
+
+Here is a rough example of what is possible.
+
+```python
+
+ @app.route('/post_json', methods=['POST'])
+ def do_trade():
+     # ...
+
+     order_data_json = request.get_json()
+
+     # validate data
+     MarketOrderRequest(**order_data_json)
+
+     # ...
+```
+
+### Many Clients <a name="many-clients"></a>
+Alpaca-py has a lot of client classes. There is a client for each API and even asset class specific clients (``StockHistoricalDataClient``, ``CryptoDataStream``). This requires you to pick and choose clients based on your needs.
+
+**Broker API:** ``BrokerClient``
+
+**Trading API:** ``TradingClient``
+
+**Market Data API:**  ``StockHistoricalDataClient``, ``CryptoHistoricalDataClient``, ``CryptoDataStream``, ``StockDataStream``
+
+## API Keys <a name="api-keys"></a>
+
+### Trading and Market Data API <a name="trading-api-keys"></a>
+In order to use Alpaca’s services you’ll need to sign up for an Alpaca account and retrieve your API keys. Signing up is completely free and takes only a few minutes. Sandbox environments are available to test out the API. To use the sandbox environment, you will need to provide sandbox/paper keys. API keys are passed into Alpaca-py through either ``TradingClient``, ``StockHistoricalDataClient``, ``CryptoHistoricalDataClient``, ``StockDataStream``, or ``CryptoDataStream``.
+
+### Broker API <a name="broker-api-keys"></a>
+To use the Broker API, you will need to sign up for a broker account and retrieve your Broker API keys. The API keys can be found on the dashboard once you’ve logged in. Alpaca also provides a sandbox environment to test out Broker API. To use the sandbox mode, provide your sandbox keys. Once you have your keys, you can pass them into ``BrokerClient`` to get started.
+
+## Usage <a name="usage"></a>
+Alpaca’s APIs allow you to do everything from building algorithmic trading strategies to building a full brokerage experience for your own end users. Here are some things you can do with Alpaca-py.
+
+To view full descriptions and examples view the [documentation page](https://alpaca.markets/docs/python-sdk/index.html).
+
+**Market Data API**: Access live and historical market data for 5000+ stocks and 20+ crypto.
+
+**Trading API**: Trade stock and crypto with lightning fast execution speeds.
+
+**Broker API & Connect**: Build investment apps - from robo-advisors to brokerages.
+
+### Broker API Example <a name="broker-api-example"></a>
+
+**Listing All Accounts**
+
+The ``BrokerClient.list_accounts`` method allows you to list all the brokerage accounts under your management. The method takes an optional parameter ``search_parameters`` which requires a ``ListAccountsRequest`` object. This parameter allows you to filter the list of accounts returned.
+
+```python
+from alpaca.broker.client import BrokerClient
+from alpaca.broker.requests import ListAccountsRequest
+from alpaca.broker.enums import AccountEntities
+
+broker_client = BrokerClient('api-key', 'secret-key')
+
+# search for accounts created after January 30th 2022.
+# Response should contain Contact and Identity fields for each account.
+filter = ListAccountsRequest(
+                    created_after=datetime.datetime.strptime("2022-01-30", "%Y-%m-%d"),
+                    entities=[AccountEntities.CONTACT, AccountEntities.IDENTITY]
+                    )
+
+accounts = broker_client.list_accounts(search_parameters=filter)
+```
+
+### Trading API Example <a name="trading-api-example"></a>
+
+**Submitting an Order**
+
+To create an order on Alpaca-py you must use an ``OrderRequest`` object. There are different ``OrderRequest`` objects based on the type of order you want to make. For market orders, there is ``MarketOrderRequest``, limit orders have ``LimitOrderRequest``, stop orders ``StopOrderRequest``, and trailing stop orders have ``TrailingStopOrderRequest``. Each order type have their own required parameters for a successful order.
+
+
+```python
+from alpaca.trading.client import TradingClient
+from alpaca.trading.requests import MarketOrderRequest
+from alpaca.trading.enums import OrderSide, TimeInForce
+
+trading_client = TradingClient('api-key', 'secret-key')
+
+
+# preparing order data
+market_order_data = MarketOrderRequest(
+                      symbol="BTC/USD",
+                      qty=0.0001,
+                      side=OrderSide.BUY,
+                      time_in_force=TimeInForce.DAY
+                  )
+
+# Market order
+market_order = trading_client.submit_order(
+                order_data=market_order_data
+                )
+```
+
+
+### Market Data API Example <a name="data-api-example"></a>
+**Querying Historical Bar Data**
+
+You can request bar data via the HistoricalDataClients. In this example, we query daily bar data for “BTC/USD” and “ETH/USD” since July 1st 2022. You can convert the response to a multi-index pandas dataframe using the ``.df`` property.
+
+```python
+from alpaca.data.historical import CryptoHistoricalDataClient
+from alpaca.data.requests import CryptoBarsRequest
+from alpaca.data.timeframe import TimeFrame
+from datetime import datetime
+
+# no keys required for crypto data
+client = CryptoHistoricalDataClient()
+
+request_params = CryptoBarsRequest(
+                        symbol_or_symbols=["BTC/USD", "ETH/USD"],
+                        timeframe=TimeFrame.Day,
+                        start=datetime.strptime("2022-07-01", '%Y-%m-%d')
+                        )
+
+bars = client.get_crypto_bars(request_params)
+
+# convert to dataframe
+bars.df
+
+```
 
-setup(**setup_kwargs)
```

