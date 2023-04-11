# Comparing `tmp/lib-pybroker-1.1.1.tar.gz` & `tmp/lib-pybroker-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-pybroker-1.1.1.tar", last modified: Sat Apr  1 01:26:03 2023, max compression
+gzip compressed data, was "lib-pybroker-1.1.2.tar", last modified: Tue Apr 11 08:04:18 2023, max compression
```

## Comparing `lib-pybroker-1.1.1.tar` & `lib-pybroker-1.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:26:03.635354 lib-pybroker-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-01 01:26:03.635354 lib-pybroker-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-01 01:26:03.639354 lib-pybroker-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:26:03.631354 lib-pybroker-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:26:03.631354 lib-pybroker-1.1.1/src/lib_pybroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-01 01:26:03.000000 lib-pybroker-1.1.1/src/lib_pybroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-01 01:26:03.000000 lib-pybroker-1.1.1/src/lib_pybroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 01:26:03.000000 lib-pybroker-1.1.1/src/lib_pybroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-01 01:26:03.000000 lib-pybroker-1.1.1/src/lib_pybroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-01 01:26:03.000000 lib-pybroker-1.1.1/src/lib_pybroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:26:03.635354 lib-pybroker-1.1.1/src/pybroker/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    38542 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/src/pybroker/vect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:26:03.635354 lib-pybroker-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20974 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    71529 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-01 01:25:52.000000 lib-pybroker-1.1.1/tests/test_vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.508905 lib-pybroker-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-11 08:04:18.508905 lib-pybroker-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-11 08:04:18.508905 lib-pybroker-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.500904 lib-pybroker-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.504904 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.504904 lib-pybroker-1.1.2/src/pybroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43313 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.508905 lib-pybroker-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71585 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_vect.py
```

### Comparing `lib-pybroker-1.1.1/LICENSE` & `lib-pybroker-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/PKG-INFO` & `lib-pybroker-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.1
+Version: 1.1.2
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.1/README.md` & `lib-pybroker-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/setup.cfg` & `lib-pybroker-1.1.2/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lib-pybroker
-version = 1.1.1
+version = 1.1.2
 url = http://www.pybroker.com
 author = Edward West
 author_email = edwest@pybroker.com
 description = Algorithmic trading with machine learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0 with Commons Clause
```

### Comparing `lib-pybroker-1.1.1/src/lib_pybroker.egg-info/PKG-INFO` & `lib-pybroker-1.1.2/src/lib_pybroker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.1
+Version: 1.1.2
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.1/src/lib_pybroker.egg-info/SOURCES.txt` & `lib-pybroker-1.1.2/src/lib_pybroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/__init__.py` & `lib-pybroker-1.1.2/src/pybroker/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/cache.py` & `lib-pybroker-1.1.2/src/pybroker/cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/common.py` & `lib-pybroker-1.1.2/src/pybroker/common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/config.py` & `lib-pybroker-1.1.2/src/pybroker/config.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/context.py` & `lib-pybroker-1.1.2/src/pybroker/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -905,18 +905,14 @@
 
     def cancel_all_pending_orders(self, symbol: Optional[str] = None):
         r"""Cancels all :class:`pybroker.scope.PendingOrder`\ s for ``symbol``.
         When ``symbol`` is ``None``, all pending orders are canceled.
         """
         self._pending_order_scope.remove_all(symbol)
 
-    def cancel_stop(self, stop_id: int) -> bool:
-        """Cancels a :class:`pybroker.portfolio.Stop` with ``stop_id``."""
-        return self._portfolio.remove_stop(stop_id)
-
     def cancel_stops(
         self,
         val: Union[str, Position, Entry],
         stop_type: Optional[StopType] = None,
     ):
         r"""Cancels :class:`pybroker.portfolio.Stop`\ s.
 
@@ -959,15 +955,15 @@
                 raise ValueError("Percent or points must be set.")
             if percent is not None:
                 percent_dec = to_decimal(percent)
             elif points is not None:
                 points_dec = to_decimal(points)
         if limit_price is not None:
             limit_price_dec = to_decimal(limit_price)
-        self._stop_id += 1
+        ExecContext._stop_id += 1
         return Stop(
             id=self._stop_id,
             symbol=self._get_symbol(),
             stop_type=stop_type,
             pos_type=pos_type,
             percent=percent_dec,
             points=points_dec,
```

### Comparing `lib-pybroker-1.1.1/src/pybroker/data.py` & `lib-pybroker-1.1.2/src/pybroker/data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/eval.py` & `lib-pybroker-1.1.2/src/pybroker/eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/indicator.py` & `lib-pybroker-1.1.2/src/pybroker/indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/log.py` & `lib-pybroker-1.1.2/src/pybroker/log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/model.py` & `lib-pybroker-1.1.2/src/pybroker/model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/portfolio.py` & `lib-pybroker-1.1.2/src/pybroker/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,18 +297,14 @@
             sorted in ascending chronological order.
         position_bars: ``deque`` of snapshots of :class:`.Position` states on
             every bar, sorted in ascending chronological order.
         win_rate: Running win rate of trades.
         loss_rate: Running loss rate of trades.
     """
 
-    _order_id: int = 0
-    _entry_id: int = 0
-    _trade_id: int = 0
-
     def __init__(
         self,
         cash: float,
         fee_mode: Optional[FeeMode] = None,
         fee_amount: Optional[float] = None,
         enable_fractional_shares: bool = False,
         max_long_positions: Optional[int] = None,
@@ -336,14 +332,17 @@
         self.bars: deque[PortfolioBar] = deque()
         self.position_bars: deque[PositionBar] = deque()
         self.win_rate: Decimal = Decimal()
         self.loss_rate: Decimal = Decimal()
         self._wins: Decimal = Decimal()
         self._logger = StaticScope.instance().logger
         self._stop_data: dict[int, _StopData] = {}
+        self._order_id: int = 0
+        self._entry_id: int = 0
+        self._trade_id: int = 0
 
     def _calculate_fees(self, fill_price: Decimal, shares: Decimal) -> Decimal:
         fees = Decimal()
         if self._fee_mode is None or self._fee_amount is None:
             return fees
         if self._fee_mode == FeeMode.ORDER_PERCENT:
             fees = self._fee_amount / Decimal(100) * fill_price * shares
```

### Comparing `lib-pybroker-1.1.1/src/pybroker/scope.py` & `lib-pybroker-1.1.2/src/pybroker/scope.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/strategy.py` & `lib-pybroker-1.1.2/src/pybroker/strategy.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/src/pybroker/vect.py` & `lib-pybroker-1.1.2/src/pybroker/vect.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_cache.py` & `lib-pybroker-1.1.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_common.py` & `lib-pybroker-1.1.2/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_context.py` & `lib-pybroker-1.1.2/tests/test_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from pybroker.context import (
     ExecContext,
     ExecResult,
     PosSizeContext,
     set_exec_ctx_data,
     set_pos_size_ctx_data,
 )
-from pybroker.portfolio import Order, Portfolio, Position, Stop, Trade
+from pybroker.portfolio import Order, Portfolio, Position, Trade
 
 
 @pytest.fixture()
 def portfolio():
     return Portfolio(100_000)
 
 
@@ -468,42 +468,35 @@
     ctx.buy_limit_price = 99.99
     ctx.sell_fill_price: PriceType = PriceType.HIGH
     ctx.sell_shares = 20
     ctx.sell_limit_price = 110.11
     ctx.hold_bars = 2
     ctx.score = 7
     result = ctx.to_result()
-    assert result == ExecResult(
-        symbol=symbol,
-        date=date,
-        buy_fill_price=PriceType.AVERAGE,
-        buy_shares=20,
-        buy_limit_price=Decimal("99.99"),
-        sell_fill_price=PriceType.HIGH,
-        sell_shares=20,
-        sell_limit_price=Decimal("110.11"),
-        hold_bars=2,
-        score=7,
-        long_stops=frozenset(
-            [
-                Stop(
-                    id=1,
-                    symbol=symbol,
-                    stop_type=StopType.BAR,
-                    pos_type="long",
-                    percent=None,
-                    points=None,
-                    bars=2,
-                    fill_price=PriceType.HIGH,
-                    limit_price=None,
-                )
-            ]
-        ),
-        short_stops=None,
-    )
+    assert result.symbol == symbol
+    assert result.date == date
+    assert result.buy_fill_price == PriceType.AVERAGE
+    assert result.buy_shares == 20
+    assert result.buy_limit_price == Decimal("99.99")
+    assert result.sell_fill_price == PriceType.HIGH
+    assert result.sell_shares == 20
+    assert result.sell_limit_price == Decimal("110.11")
+    assert result.hold_bars == 2
+    assert result.score == 7
+    assert len(result.long_stops) == 1
+    assert result.short_stops is None
+    stop = next(iter(result.long_stops))
+    assert stop.symbol == symbol
+    assert stop.stop_type == StopType.BAR
+    assert stop.pos_type == "long"
+    assert stop.percent is None
+    assert stop.points is None
+    assert stop.bars == 2
+    assert stop.fill_price == PriceType.HIGH
+    assert stop.limit_price is None
 
 
 @pytest.mark.parametrize("pos_type", ["long", "short"])
 @pytest.mark.parametrize(
     "stop_attr, expected_stop_type",
     [
         ("stop_loss", StopType.LOSS),
@@ -521,58 +514,53 @@
     stop_amount = 20
     percent = None
     points = None
     if stop_attr.endswith("_pct"):
         percent = stop_amount
     else:
         points = stop_amount
-    expected_stops = frozenset(
-        [
-            Stop(
-                id=1,
-                symbol=symbol,
-                stop_type=expected_stop_type,
-                pos_type=pos_type,
-                percent=percent,
-                points=points,
-                bars=None,
-                fill_price=None,
-                limit_price=stop_limit,
-            )
-        ]
-    )
     buy_shares = None
     sell_shares = None
-    long_stops = None
-    short_stops = None
     if pos_type == "long":
         buy_shares = 100
-        long_stops = expected_stops
     else:
         sell_shares = 100
-        short_stops = expected_stops
     ctx.buy_shares = buy_shares
     ctx.sell_shares = sell_shares
     setattr(ctx, stop_attr, stop_amount)
     setattr(ctx, f"{stop_attr.replace('_pct', '')}_limit", stop_limit)
     result = ctx.to_result()
-    assert result == ExecResult(
-        symbol=symbol,
-        date=date,
-        buy_fill_price=PriceType.MIDDLE,
-        buy_shares=buy_shares,
-        buy_limit_price=None,
-        sell_fill_price=PriceType.MIDDLE,
-        sell_shares=sell_shares,
-        sell_limit_price=None,
-        hold_bars=None,
-        score=None,
-        long_stops=long_stops,
-        short_stops=short_stops,
-    )
+    assert result.symbol == symbol
+    assert result.date == date
+    assert result.buy_fill_price == PriceType.MIDDLE
+    assert result.buy_limit_price is None
+    assert result.sell_fill_price == PriceType.MIDDLE
+    assert result.sell_limit_price is None
+    assert result.hold_bars is None
+    assert result.score is None
+    if pos_type == "long":
+        assert result.buy_shares == 100
+        assert result.sell_shares is None
+        assert len(result.long_stops) == 1
+        assert result.short_stops is None
+        stop = next(iter(result.long_stops))
+    else:
+        assert result.sell_shares == 100
+        assert result.buy_shares is None
+        assert len(result.short_stops) == 1
+        assert result.long_stops is None
+        stop = next(iter(result.short_stops))
+    assert stop.symbol == symbol
+    assert stop.stop_type == expected_stop_type
+    assert stop.pos_type == pos_type
+    assert stop.percent == percent
+    assert stop.points == points
+    assert stop.bars is None
+    assert stop.fill_price is None
+    assert stop.limit_price == stop_limit
 
 
 @pytest.mark.parametrize(
     "stop_attr", ["stop_loss", "stop_profit", "stop_trailing"]
 )
 def test_to_result_when_stop_pct_and_points_then_error(ctx, stop_attr):
     ctx.buy_shares = 100
```

### Comparing `lib-pybroker-1.1.1/tests/test_data.py` & `lib-pybroker-1.1.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_eval.py` & `lib-pybroker-1.1.2/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_indicator.py` & `lib-pybroker-1.1.2/tests/test_indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_log.py` & `lib-pybroker-1.1.2/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_model.py` & `lib-pybroker-1.1.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_portfolio.py` & `lib-pybroker-1.1.2/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_scope.py` & `lib-pybroker-1.1.2/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.1/tests/test_strategy.py` & `lib-pybroker-1.1.2/tests/test_strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1816,45 +1816,68 @@
 
     def test_backtest_when_stop_loss(self, data_source_df):
         def exec_fn(ctx):
             if ctx.bars == 1:
                 ctx.buy_shares = 100
                 ctx.stop_loss = 10
 
-        df = data_source_df[data_source_df["symbol"] == "SPY"]
+        df = data_source_df[data_source_df["symbol"].isin(["SPY", "AAPL"])]
         dates = df["date"].unique()
         dates = dates[dates <= np.datetime64(END_DATE)]
         strategy = Strategy(data_source_df, START_DATE, END_DATE)
-        strategy.add_execution(exec_fn, "SPY")
+        strategy.add_execution(exec_fn, ["SPY", "AAPL"])
         result = strategy.backtest(calc_bootstrap=False)
-        assert len(result.trades) == 1
+        assert len(result.trades) == 2
         trade = result.trades.iloc[0]
         assert trade["type"] == "long"
         assert trade["symbol"] == "SPY"
         assert trade["entry_date"] == dates[1]
         assert trade["exit"] == trade["entry"] - 10
         assert trade["shares"] == 100
         assert trade["pnl"] == -1000
         assert trade["agg_pnl"] == -1000
         assert trade["pnl_per_bar"] == round(-1000 / trade["bars"], 2)
         assert trade["stop"] == "loss"
-        assert len(result.orders) == 2
+        trade = result.trades.iloc[1]
+        assert trade["type"] == "long"
+        assert trade["symbol"] == "AAPL"
+        assert trade["entry_date"] == dates[1]
+        assert trade["exit"] == trade["entry"] - 10
+        assert trade["shares"] == 100
+        assert trade["pnl"] == -1000
+        assert trade["agg_pnl"] == -2000
+        assert trade["pnl_per_bar"] == round(-1000 / trade["bars"], 2)
+        assert trade["stop"] == "loss"
+        assert len(result.orders) == 4
         buy_order = result.orders.iloc[0]
         assert buy_order["type"] == "buy"
         assert buy_order["symbol"] == "SPY"
         assert buy_order["date"] == dates[1]
         assert buy_order["shares"] == 100
         assert np.isnan(buy_order["limit_price"])
         assert buy_order["fees"] == 0
-        sell_order = result.orders.iloc[1]
+        buy_order = result.orders.iloc[1]
+        assert buy_order["type"] == "buy"
+        assert buy_order["symbol"] == "AAPL"
+        assert buy_order["date"] == dates[1]
+        assert buy_order["shares"] == 100
+        assert np.isnan(buy_order["limit_price"])
+        assert buy_order["fees"] == 0
+        sell_order = result.orders.iloc[2]
         assert sell_order["type"] == "sell"
         assert sell_order["symbol"] == "SPY"
         assert sell_order["shares"] == 100
         assert np.isnan(sell_order["limit_price"])
         assert sell_order["fees"] == 0
+        sell_order = result.orders.iloc[3]
+        assert sell_order["type"] == "sell"
+        assert sell_order["symbol"] == "AAPL"
+        assert sell_order["shares"] == 100
+        assert np.isnan(sell_order["limit_price"])
+        assert sell_order["fees"] == 0
 
     def test_backtest_when_sell_before_stop_loss(self, data_source_df):
         def exec_fn(ctx):
             if ctx.bars == 1:
                 ctx.buy_shares = 100
                 ctx.stop_loss = 10
             elif ctx.bars == 10:
@@ -1886,38 +1909,14 @@
         assert sell_order["type"] == "sell"
         assert sell_order["symbol"] == "SPY"
         assert sell_order["date"] == dates[10]
         assert sell_order["shares"] == 100
         assert np.isnan(sell_order["limit_price"])
         assert sell_order["fees"] == 0
 
-    def test_backtest_when_cancel_stop(self, data_source_df):
-        def exec_fn(ctx):
-            if ctx.bars == 1:
-                ctx.buy_shares = 100
-                ctx.stop_loss = 10
-            elif ctx.bars == 10:
-                assert ctx.cancel_stop(stop_id=1)
-
-        df = data_source_df[data_source_df["symbol"] == "SPY"]
-        dates = df["date"].unique()
-        dates = dates[dates <= np.datetime64(END_DATE)]
-        strategy = Strategy(data_source_df, START_DATE, END_DATE)
-        strategy.add_execution(exec_fn, "SPY")
-        result = strategy.backtest(calc_bootstrap=False)
-        assert not len(result.trades)
-        assert len(result.orders) == 1
-        buy_order = result.orders.iloc[0]
-        assert buy_order["type"] == "buy"
-        assert buy_order["symbol"] == "SPY"
-        assert buy_order["date"] == dates[1]
-        assert buy_order["shares"] == 100
-        assert np.isnan(buy_order["limit_price"])
-        assert buy_order["fees"] == 0
-
     def test_backtest_when_cancel_stops(self, data_source_df):
         def exec_fn(ctx):
             if ctx.bars == 1:
                 ctx.buy_shares = 100
                 ctx.stop_loss = 10
                 ctx.stop_trailing = 10
             elif ctx.bars == 10:
```

### Comparing `lib-pybroker-1.1.1/tests/test_vect.py` & `lib-pybroker-1.1.2/tests/test_vect.py`

 * *Files identical despite different names*

