# Comparing `tmp/gym-trading-env-0.1.3.tar.gz` & `tmp/gym-trading-env-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-trading-env-0.1.3.tar", last modified: Tue Apr 11 09:32:00 2023, max compression
+gzip compressed data, was "gym-trading-env-0.1.4.tar", last modified: Tue Apr 11 09:41:52 2023, max compression
```

## Comparing `gym-trading-env-0.1.3.tar` & `gym-trading-env-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.376202 gym-trading-env-0.1.3/
--rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0    14011 2023-04-11 09:32:00.374198 gym-trading-env-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    12149 2023-04-11 09:31:03.000000 gym-trading-env-0.1.3/README.md
--rw-rw-rw-   0        0        0      854 2023-04-11 09:28:09.000000 gym-trading-env-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 09:32:00.377196 gym-trading-env-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.290425 gym-trading-env-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.318349 gym-trading-env-0.1.3/src/gym_trading_env/
--rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.3/src/gym_trading_env/__init__.py
--rw-rw-rw-   0        0        0     3855 2023-04-10 19:15:33.000000 gym-trading-env-0.1.3/src/gym_trading_env/downloader.py
--rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.3/src/gym_trading_env/environments.py
--rw-rw-rw-   0        0        0     2502 2023-04-11 09:31:34.000000 gym-trading-env-0.1.3/src/gym_trading_env/renderer.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.372205 gym-trading-env-0.1.3/src/gym_trading_env/utils/
--rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.3/src/gym_trading_env/utils/__init__.py
--rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.3/src/gym_trading_env/utils/charts.py
--rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.3/src/gym_trading_env/utils/history.py
--rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.3/src/gym_trading_env/utils/portfolio.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:32:00.357280 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/
--rw-rw-rw-   0        0        0    14011 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-11 09:32:00.000000 gym-trading-env-0.1.3/src/gym_trading_env.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-11 09:41:52.164253 gym-trading-env-0.1.4/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 11:11:31.000000 gym-trading-env-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    14011 2023-04-11 09:41:52.163255 gym-trading-env-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    12149 2023-04-11 09:31:03.000000 gym-trading-env-0.1.4/README.md
+-rw-rw-rw-   0        0        0      854 2023-04-11 09:41:24.000000 gym-trading-env-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-11 09:41:52.164253 gym-trading-env-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-11 09:41:52.083468 gym-trading-env-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-11 09:41:52.106407 gym-trading-env-0.1.4/src/gym_trading_env/
+-rw-rw-rw-   0        0        0        0 2023-03-30 12:22:21.000000 gym-trading-env-0.1.4/src/gym_trading_env/__init__.py
+-rw-rw-rw-   0        0        0     3949 2023-04-11 09:40:58.000000 gym-trading-env-0.1.4/src/gym_trading_env/downloader.py
+-rw-rw-rw-   0        0        0     8624 2023-04-10 19:39:58.000000 gym-trading-env-0.1.4/src/gym_trading_env/environments.py
+-rw-rw-rw-   0        0        0     2502 2023-04-11 09:31:34.000000 gym-trading-env-0.1.4/src/gym_trading_env/renderer.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:41:52.161260 gym-trading-env-0.1.4/src/gym_trading_env/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-02 16:47:36.000000 gym-trading-env-0.1.4/src/gym_trading_env/utils/__init__.py
+-rw-rw-rw-   0        0        0    14334 2023-04-05 09:25:28.000000 gym-trading-env-0.1.4/src/gym_trading_env/utils/charts.py
+-rw-rw-rw-   0        0        0     3333 2023-04-02 16:57:28.000000 gym-trading-env-0.1.4/src/gym_trading_env/utils/history.py
+-rw-rw-rw-   0        0        0     3036 2023-04-02 16:57:45.000000 gym-trading-env-0.1.4/src/gym_trading_env/utils/portfolio.py
+drwxrwxrwx   0        0        0        0 2023-04-11 09:41:52.148295 gym-trading-env-0.1.4/src/gym_trading_env.egg-info/
+-rw-rw-rw-   0        0        0    14011 2023-04-11 09:41:52.000000 gym-trading-env-0.1.4/src/gym_trading_env.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-04-11 09:41:52.000000 gym-trading-env-0.1.4/src/gym_trading_env.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 09:41:52.000000 gym-trading-env-0.1.4/src/gym_trading_env.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-04-11 09:41:52.000000 gym-trading-env-0.1.4/src/gym_trading_env.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-11 09:41:52.000000 gym-trading-env-0.1.4/src/gym_trading_env.egg-info/top_level.txt
```

### Comparing `gym-trading-env-0.1.3/LICENSE.txt` & `gym-trading-env-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.3/PKG-INFO` & `gym-trading-env-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gym-trading-env-0.1.3/README.md` & `gym-trading-env-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.3/pyproject.toml` & `gym-trading-env-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gym-trading-env"
-version = "0.1.3"
+version = "0.1.4"
 license = {file = "LICENSE.txt"}
 authors = [
   { name="Clement Perroud", email="clement.perroud.pro@gmail.com" },
 ]
 description = "A simple, easy, customizable Open IA Gym environments for trading."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `gym-trading-env-0.1.3/src/gym_trading_env/downloader.py` & `gym-trading-env-0.1.4/src/gym_trading_env/downloader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import ccxt.async_support as ccxt
 import pandas as pd
 import datetime
-from tqdm import tqdm
 
 
 EXCHANGE_LIMIT_RATES = {
     "bitfinex2": {
         "limit":10_000,
         "pause_every": 1,
         "pause" : 3, #seconds
@@ -52,15 +51,17 @@
     final_df.drop_duplicates(inplace=True)
     return final_df
 
 async def _download_symbols(exchange_name, symbols, dir, timeframe,  **kwargs):
     exchange = getattr(ccxt, exchange_name)({ 'enableRateLimit': True })
     for symbol in symbols:
         df = await _download_symbol(exchange = exchange, symbol = symbol, timeframe= timeframe, **kwargs)
-        df.to_pickle(f"{dir}/{exchange_name}-{symbol.replace('/', '')}-{timeframe}.pkl")
+        save_file = f"{dir}/{exchange_name}-{symbol.replace('/', '')}-{timeframe}.pkl"
+        print(f"{symbol} downloaded from {exchange_name} and stored at {save_file}")
+        df.to_pickle(save_file)
     await exchange.close()
 
 async def _download(exchange_names, symbols, timeframe, dir, since : datetime.datetime, until : datetime.datetime = datetime.datetime.now()):
     tasks = []
     for exchange_name in exchange_names:
         
         limit = EXCHANGE_LIMIT_RATES[exchange_name]["limit"]
```

### Comparing `gym-trading-env-0.1.3/src/gym_trading_env/environments.py` & `gym-trading-env-0.1.4/src/gym_trading_env/environments.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.3/src/gym_trading_env/renderer.py` & `gym-trading-env-0.1.4/src/gym_trading_env/renderer.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.3/src/gym_trading_env/utils/charts.py` & `gym-trading-env-0.1.4/src/gym_trading_env/utils/charts.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.3/src/gym_trading_env/utils/history.py` & `gym-trading-env-0.1.4/src/gym_trading_env/utils/history.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.3/src/gym_trading_env/utils/portfolio.py` & `gym-trading-env-0.1.4/src/gym_trading_env/utils/portfolio.py`

 * *Files identical despite different names*

### Comparing `gym-trading-env-0.1.3/src/gym_trading_env.egg-info/PKG-INFO` & `gym-trading-env-0.1.4/src/gym_trading_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-trading-env
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple, easy, customizable Open IA Gym environments for trading.
 Author-email: Clement Perroud <clement.perroud.pro@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gym-trading-env-0.1.3/src/gym_trading_env.egg-info/SOURCES.txt` & `gym-trading-env-0.1.4/src/gym_trading_env.egg-info/SOURCES.txt`

 * *Files identical despite different names*

