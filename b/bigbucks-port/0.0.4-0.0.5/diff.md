# Comparing `tmp/bigbucks_port-0.0.4.tar.gz` & `tmp/bigbucks_port-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigbucks_port-0.0.4.tar", last modified: Thu Apr  6 03:46:51 2023, max compression
+gzip compressed data, was "bigbucks_port-0.0.5.tar", last modified: Tue Apr 11 03:48:33 2023, max compression
```

## Comparing `bigbucks_port-0.0.4.tar` & `bigbucks_port-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-06 03:46:51.850742 bigbucks_port-0.0.4/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     1065 2023-04-03 00:48:13.000000 bigbucks_port-0.0.4/LICENSE
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-06 03:46:51.850583 bigbucks_port-0.0.4/PKG-INFO
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3264 2023-04-06 03:40:05.000000 bigbucks_port-0.0.4/README.md
--rw-r--r--   0 cuiwenjie   (501) staff       (20)       38 2023-04-06 03:46:51.850785 bigbucks_port-0.0.4/setup.cfg
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      346 2023-04-06 03:46:18.000000 bigbucks_port-0.0.4/setup.py
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-06 03:46:51.848605 bigbucks_port-0.0.4/src/
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-06 03:46:51.849668 bigbucks_port-0.0.4/src/bigbucks_port/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)        0 2023-04-02 23:17:45.000000 bigbucks_port-0.0.4/src/bigbucks_port/__init__.py
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     8751 2023-04-06 03:37:05.000000 bigbucks_port-0.0.4/src/bigbucks_port/portfolio.py
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-06 03:46:51.850251 bigbucks_port-0.0.4/src/bigbucks_port.egg-info/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-06 03:46:51.000000 bigbucks_port-0.0.4/src/bigbucks_port.egg-info/PKG-INFO
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      275 2023-04-06 03:46:51.000000 bigbucks_port-0.0.4/src/bigbucks_port.egg-info/SOURCES.txt
--rw-r--r--   0 cuiwenjie   (501) staff       (20)        1 2023-04-06 03:46:51.000000 bigbucks_port-0.0.4/src/bigbucks_port.egg-info/dependency_links.txt
--rw-r--r--   0 cuiwenjie   (501) staff       (20)       14 2023-04-06 03:46:51.000000 bigbucks_port-0.0.4/src/bigbucks_port.egg-info/top_level.txt
-drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-06 03:46:51.850392 bigbucks_port-0.0.4/tests/
--rw-r--r--   0 cuiwenjie   (501) staff       (20)      582 2023-04-06 03:41:07.000000 bigbucks_port-0.0.4/tests/test_portfolio.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.985796 bigbucks_port-0.0.5/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     1065 2023-04-03 00:48:13.000000 bigbucks_port-0.0.5/LICENSE
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-11 03:48:33.985619 bigbucks_port-0.0.5/PKG-INFO
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3264 2023-04-06 03:40:05.000000 bigbucks_port-0.0.5/README.md
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)       38 2023-04-11 03:48:33.985848 bigbucks_port-0.0.5/setup.cfg
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      346 2023-04-11 03:41:43.000000 bigbucks_port-0.0.5/setup.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.983076 bigbucks_port-0.0.5/src/
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.984236 bigbucks_port-0.0.5/src/bigbucks_port/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)        0 2023-04-02 23:17:45.000000 bigbucks_port-0.0.5/src/bigbucks_port/__init__.py
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     8947 2023-04-11 03:34:35.000000 bigbucks_port-0.0.5/src/bigbucks_port/portfolio.py
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.984969 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)     3464 2023-04-11 03:48:33.000000 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/PKG-INFO
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      275 2023-04-11 03:48:33.000000 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/SOURCES.txt
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)        1 2023-04-11 03:48:33.000000 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/dependency_links.txt
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)       14 2023-04-11 03:48:33.000000 bigbucks_port-0.0.5/src/bigbucks_port.egg-info/top_level.txt
+drwxr-xr-x   0 cuiwenjie   (501) staff       (20)        0 2023-04-11 03:48:33.985159 bigbucks_port-0.0.5/tests/
+-rw-r--r--   0 cuiwenjie   (501) staff       (20)      531 2023-04-11 03:43:40.000000 bigbucks_port-0.0.5/tests/test_portfolio.py
```

### Comparing `bigbucks_port-0.0.4/LICENSE` & `bigbucks_port-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bigbucks_port-0.0.4/PKG-INFO` & `bigbucks_port-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbucks_port
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package used for portfolio analysis in Fintech512
 Author: Wenjie Cui
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
```

### Comparing `bigbucks_port-0.0.4/README.md` & `bigbucks_port-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bigbucks_port-0.0.4/src/bigbucks_port/portfolio.py` & `bigbucks_port-0.0.5/src/bigbucks_port/portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,23 @@
     return current_holding(objs,id).to_json(orient='index')
 
 # Calculate the daily returns for the stocks in the portfolio
 def cal_returns(objs,id):
     # Get the symbols in the holding
     holdings = current_holding(objs,id)
     symbols = holdings.index.to_numpy()
+    if len(symbols) ==0:
+        raise Exception("This user has no holding")
     stockreturns = pd.DataFrame(columns=symbols)
     # Get the daily prices for the given symbol
     for s in symbols:
-        stockprice = pd.json_normalize(objs.view_symbol_price_data(s))
+        data = objs.view_symbol_price_data(s)
+        if len(data) == 0:
+            raise Exception("This symbol has no historical price data")
+        stockprice = pd.json_normalize(data)
         # Sort prices by date
         stockprice.sort_values(by='date',inplace=True)
         # calculate the daily returns
         returns = np.log(stockprice['adjusted_close']/stockprice['adjusted_close'].shift(1))
         stockreturns[s]=returns.to_numpy()
     stockreturns.index = stockprice['date']
     stockreturns.dropna(inplace=True)
```

### Comparing `bigbucks_port-0.0.4/src/bigbucks_port.egg-info/PKG-INFO` & `bigbucks_port-0.0.5/src/bigbucks_port.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbucks-port
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package used for portfolio analysis in Fintech512
 Author: Wenjie Cui
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Introduction
```

