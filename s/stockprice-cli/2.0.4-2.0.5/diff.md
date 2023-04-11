# Comparing `tmp/stockprice_cli-2.0.4-py3-none-any.whl.zip` & `tmp/stockprice_cli-2.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3158 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 14:48 stockprice/__init__.py
--rw-r--r--  2.0 unx     2404 b- defN 23-Apr-10 14:48 stockprice/calculate_price_movement.py
--rw-r--r--  2.0 unx      733 b- defN 23-Apr-10 14:48 stockprice/main.py
--rw-r--r--  2.0 unx      612 b- defN 23-Apr-10 14:49 stockprice_cli-2.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 14:49 stockprice_cli-2.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-10 14:49 stockprice_cli-2.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-10 14:49 stockprice_cli-2.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      672 b- defN 23-Apr-10 14:49 stockprice_cli-2.0.4.dist-info/RECORD
-8 files, 4577 bytes uncompressed, 1966 bytes compressed:  57.0%
+Zip file size: 3192 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 16:51 stockprice/__init__.py
+-rw-r--r--  2.0 unx     2404 b- defN 23-Apr-11 16:51 stockprice/calculate_price_movement.py
+-rw-r--r--  2.0 unx      872 b- defN 23-Apr-11 16:51 stockprice/main.py
+-rw-r--r--  2.0 unx      612 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      672 b- defN 23-Apr-11 16:51 stockprice_cli-2.0.5.dist-info/RECORD
+8 files, 4716 bytes uncompressed, 2000 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: stockprice/calculate_price_movement.py
 Comment: 
 
 Filename: stockprice/main.py
 Comment: 
 
-Filename: stockprice_cli-2.0.4.dist-info/METADATA
+Filename: stockprice_cli-2.0.5.dist-info/METADATA
 Comment: 
 
-Filename: stockprice_cli-2.0.4.dist-info/WHEEL
+Filename: stockprice_cli-2.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: stockprice_cli-2.0.4.dist-info/entry_points.txt
+Filename: stockprice_cli-2.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: stockprice_cli-2.0.4.dist-info/top_level.txt
+Filename: stockprice_cli-2.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: stockprice_cli-2.0.4.dist-info/RECORD
+Filename: stockprice_cli-2.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stockprice/main.py

```diff
@@ -1,17 +1,22 @@
 import sys
 
 from stockprice.calculate_price_movement import calculate_price_movement
 
 
 def main(args: list = sys.argv) -> None:
-    raw_input = args[1]
-    stocks = raw_input.upper().replace(" ", "").split(",")
+    raw_inputs = args[1:]
+    stock_tickers = []
+    for input in raw_inputs:
+        input = input.upper()
+        if input[-1] == ",":
+            input = input[:-1]
 
-    for ticker in stocks:
+        stock_tickers.extend(input.split(","))
+    for ticker in stock_tickers:
         (
             current_price,
             currency,
             percentage_change_1day,
             percentage_change_7day,
             percentage_change_30day,
         ) = calculate_price_movement(ticker)
```

## Comparing `stockprice_cli-2.0.4.dist-info/METADATA` & `stockprice_cli-2.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockprice-cli
-Version: 2.0.4
+Version: 2.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/Thomas-mcinally/stockprice
 Author: Thomas Mcinally
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

