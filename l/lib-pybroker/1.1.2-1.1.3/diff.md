# Comparing `tmp/lib-pybroker-1.1.2.tar.gz` & `tmp/lib-pybroker-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-pybroker-1.1.2.tar", last modified: Tue Apr 11 08:04:18 2023, max compression
+gzip compressed data, was "lib-pybroker-1.1.3.tar", last modified: Tue Apr 11 08:38:33 2023, max compression
```

## Comparing `lib-pybroker-1.1.2.tar` & `lib-pybroker-1.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.508905 lib-pybroker-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-11 08:04:18.508905 lib-pybroker-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-11 08:04:18.508905 lib-pybroker-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.500904 lib-pybroker-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.504904 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 08:04:18.000000 lib-pybroker-1.1.2/src/lib_pybroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.504904 lib-pybroker-1.1.2/src/pybroker/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    43313 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/src/pybroker/vect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:04:18.508905 lib-pybroker-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    71585 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-11 08:04:02.000000 lib-pybroker-1.1.2/tests/test_vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.521611 lib-pybroker-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-11 08:38:33.521611 lib-pybroker-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-11 08:38:33.521611 lib-pybroker-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.509611 lib-pybroker-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.513611 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 08:38:33.000000 lib-pybroker-1.1.3/src/lib_pybroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.517611 lib-pybroker-1.1.3/src/pybroker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43490 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19068 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34553 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15188 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15398 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38568 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25106 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/src/pybroker/vect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 08:38:33.521611 lib-pybroker-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21167 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18876 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16082 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72675 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-11 08:38:19.000000 lib-pybroker-1.1.3/tests/test_vect.py
```

### Comparing `lib-pybroker-1.1.2/LICENSE` & `lib-pybroker-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/PKG-INFO` & `lib-pybroker-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.2
+Version: 1.1.3
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.2/README.md` & `lib-pybroker-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/setup.cfg` & `lib-pybroker-1.1.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lib-pybroker
-version = 1.1.2
+version = 1.1.3
 url = http://www.pybroker.com
 author = Edward West
 author_email = edwest@pybroker.com
 description = Algorithmic trading with machine learning
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache License 2.0 with Commons Clause
```

### Comparing `lib-pybroker-1.1.2/src/lib_pybroker.egg-info/PKG-INFO` & `lib-pybroker-1.1.3/src/lib_pybroker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pybroker
-Version: 1.1.2
+Version: 1.1.3
 Summary: Algorithmic trading with machine learning
 Home-page: http://www.pybroker.com
 Author: Edward West
 Author-email: edwest@pybroker.com
 License: Apache License 2.0 with Commons Clause
 Classifier: License :: Free for non-commercial use
 Description-Content-Type: text/markdown
```

### Comparing `lib-pybroker-1.1.2/src/lib_pybroker.egg-info/SOURCES.txt` & `lib-pybroker-1.1.3/src/lib_pybroker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/__init__.py` & `lib-pybroker-1.1.3/src/pybroker/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/cache.py` & `lib-pybroker-1.1.3/src/pybroker/cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/common.py` & `lib-pybroker-1.1.3/src/pybroker/common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/config.py` & `lib-pybroker-1.1.3/src/pybroker/config.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/context.py` & `lib-pybroker-1.1.3/src/pybroker/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -905,14 +905,18 @@
 
     def cancel_all_pending_orders(self, symbol: Optional[str] = None):
         r"""Cancels all :class:`pybroker.scope.PendingOrder`\ s for ``symbol``.
         When ``symbol`` is ``None``, all pending orders are canceled.
         """
         self._pending_order_scope.remove_all(symbol)
 
+    def cancel_stop(self, stop_id: int) -> bool:
+        """Cancels a :class:`pybroker.portfolio.Stop` with ``stop_id``."""
+        return self._portfolio.remove_stop(stop_id)
+
     def cancel_stops(
         self,
         val: Union[str, Position, Entry],
         stop_type: Optional[StopType] = None,
     ):
         r"""Cancels :class:`pybroker.portfolio.Stop`\ s.
```

### Comparing `lib-pybroker-1.1.2/src/pybroker/data.py` & `lib-pybroker-1.1.3/src/pybroker/data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/eval.py` & `lib-pybroker-1.1.3/src/pybroker/eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/indicator.py` & `lib-pybroker-1.1.3/src/pybroker/indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/log.py` & `lib-pybroker-1.1.3/src/pybroker/log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/model.py` & `lib-pybroker-1.1.3/src/pybroker/model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/portfolio.py` & `lib-pybroker-1.1.3/src/pybroker/portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/scope.py` & `lib-pybroker-1.1.3/src/pybroker/scope.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/strategy.py` & `lib-pybroker-1.1.3/src/pybroker/strategy.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/src/pybroker/vect.py` & `lib-pybroker-1.1.3/src/pybroker/vect.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_cache.py` & `lib-pybroker-1.1.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_common.py` & `lib-pybroker-1.1.3/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_context.py` & `lib-pybroker-1.1.3/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_data.py` & `lib-pybroker-1.1.3/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_eval.py` & `lib-pybroker-1.1.3/tests/test_eval.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_indicator.py` & `lib-pybroker-1.1.3/tests/test_indicator.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_log.py` & `lib-pybroker-1.1.3/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_model.py` & `lib-pybroker-1.1.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_portfolio.py` & `lib-pybroker-1.1.3/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_scope.py` & `lib-pybroker-1.1.3/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `lib-pybroker-1.1.2/tests/test_strategy.py` & `lib-pybroker-1.1.3/tests/test_strategy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1909,14 +1909,40 @@
         assert sell_order["type"] == "sell"
         assert sell_order["symbol"] == "SPY"
         assert sell_order["date"] == dates[10]
         assert sell_order["shares"] == 100
         assert np.isnan(sell_order["limit_price"])
         assert sell_order["fees"] == 0
 
+    def test_backtest_when_cancel_stop(self, data_source_df):
+        def exec_fn(ctx):
+            if ctx.bars == 1:
+                ctx.buy_shares = 100
+                ctx.stop_loss = 10
+            elif ctx.bars == 10:
+                entry = tuple(ctx.long_pos().entries)[0]
+                stop = next(iter(entry.stops))
+                assert ctx.cancel_stop(stop_id=stop.id)
+
+        df = data_source_df[data_source_df["symbol"] == "SPY"]
+        dates = df["date"].unique()
+        dates = dates[dates <= np.datetime64(END_DATE)]
+        strategy = Strategy(data_source_df, START_DATE, END_DATE)
+        strategy.add_execution(exec_fn, "SPY")
+        result = strategy.backtest(calc_bootstrap=False)
+        assert not len(result.trades)
+        assert len(result.orders) == 1
+        buy_order = result.orders.iloc[0]
+        assert buy_order["type"] == "buy"
+        assert buy_order["symbol"] == "SPY"
+        assert buy_order["date"] == dates[1]
+        assert buy_order["shares"] == 100
+        assert np.isnan(buy_order["limit_price"])
+        assert buy_order["fees"] == 0
+
     def test_backtest_when_cancel_stops(self, data_source_df):
         def exec_fn(ctx):
             if ctx.bars == 1:
                 ctx.buy_shares = 100
                 ctx.stop_loss = 10
                 ctx.stop_trailing = 10
             elif ctx.bars == 10:
```

### Comparing `lib-pybroker-1.1.2/tests/test_vect.py` & `lib-pybroker-1.1.3/tests/test_vect.py`

 * *Files identical despite different names*

