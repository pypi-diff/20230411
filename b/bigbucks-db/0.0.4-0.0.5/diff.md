# Comparing `tmp/bigbucks_db-0.0.4.tar.gz` & `tmp/bigbucks_db-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigbucks_db-0.0.4.tar", last modified: Thu Apr  6 02:26:02 2023, max compression
+gzip compressed data, was "bigbucks_db-0.0.5.tar", last modified: Tue Apr 11 00:34:02 2023, max compression
```

## Comparing `bigbucks_db-0.0.4.tar` & `bigbucks_db-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hanyuduan   (501) staff       (20)        0 2023-04-06 02:26:02.669215 bigbucks_db-0.0.4/
--rw-r--r--   0 hanyuduan   (501) staff       (20)     1061 2023-03-26 18:43:13.000000 bigbucks_db-0.0.4/LICENSE
--rw-r--r--   0 hanyuduan   (501) staff       (20)    10843 2023-04-06 02:26:02.668678 bigbucks_db-0.0.4/PKG-INFO
--rw-r--r--   0 hanyuduan   (501) staff       (20)    10234 2023-04-06 02:20:04.000000 bigbucks_db-0.0.4/README.md
--rw-r--r--   0 hanyuduan   (501) staff       (20)      754 2023-04-06 02:23:08.000000 bigbucks_db-0.0.4/pyproject.toml
--rw-r--r--   0 hanyuduan   (501) staff       (20)       38 2023-04-06 02:26:02.669440 bigbucks_db-0.0.4/setup.cfg
-drwxr-xr-x   0 hanyuduan   (501) staff       (20)        0 2023-04-06 02:26:02.664761 bigbucks_db-0.0.4/src/
--rw-r--r--   0 hanyuduan   (501) staff       (20)        0 2023-03-26 18:25:25.000000 bigbucks_db-0.0.4/src/__init__.py
-drwxr-xr-x   0 hanyuduan   (501) staff       (20)        0 2023-04-06 02:26:02.666866 bigbucks_db-0.0.4/src/bigbucks_db.egg-info/
--rw-r--r--   0 hanyuduan   (501) staff       (20)    10843 2023-04-06 02:26:02.000000 bigbucks_db-0.0.4/src/bigbucks_db.egg-info/PKG-INFO
--rw-r--r--   0 hanyuduan   (501) staff       (20)      249 2023-04-06 02:26:02.000000 bigbucks_db-0.0.4/src/bigbucks_db.egg-info/SOURCES.txt
--rw-r--r--   0 hanyuduan   (501) staff       (20)        1 2023-04-06 02:26:02.000000 bigbucks_db-0.0.4/src/bigbucks_db.egg-info/dependency_links.txt
--rw-r--r--   0 hanyuduan   (501) staff       (20)       21 2023-04-06 02:26:02.000000 bigbucks_db-0.0.4/src/bigbucks_db.egg-info/top_level.txt
--rw-r--r--   0 hanyuduan   (501) staff       (20)    14497 2023-04-06 02:09:22.000000 bigbucks_db-0.0.4/src/bigbucks_db.py
-drwxr-xr-x   0 hanyuduan   (501) staff       (20)        0 2023-04-06 02:26:02.667484 bigbucks_db-0.0.4/tests/
--rw-r--r--   0 hanyuduan   (501) staff       (20)     1135 2023-04-06 02:23:30.000000 bigbucks_db-0.0.4/tests/test_bigbucks_db.py
+drwxr-xr-x   0 hanyuduan   (501) staff       (20)        0 2023-04-11 00:34:02.348994 bigbucks_db-0.0.5/
+-rw-r--r--   0 hanyuduan   (501) staff       (20)     1061 2023-03-26 18:43:13.000000 bigbucks_db-0.0.5/LICENSE
+-rw-r--r--   0 hanyuduan   (501) staff       (20)    10908 2023-04-11 00:34:02.348362 bigbucks_db-0.0.5/PKG-INFO
+-rw-r--r--   0 hanyuduan   (501) staff       (20)    10299 2023-04-11 00:32:29.000000 bigbucks_db-0.0.5/README.md
+-rw-r--r--   0 hanyuduan   (501) staff       (20)      754 2023-04-11 00:31:14.000000 bigbucks_db-0.0.5/pyproject.toml
+-rw-r--r--   0 hanyuduan   (501) staff       (20)       38 2023-04-11 00:34:02.349143 bigbucks_db-0.0.5/setup.cfg
+drwxr-xr-x   0 hanyuduan   (501) staff       (20)        0 2023-04-11 00:34:02.344455 bigbucks_db-0.0.5/src/
+-rw-r--r--   0 hanyuduan   (501) staff       (20)        0 2023-03-26 18:25:25.000000 bigbucks_db-0.0.5/src/__init__.py
+drwxr-xr-x   0 hanyuduan   (501) staff       (20)        0 2023-04-11 00:34:02.347195 bigbucks_db-0.0.5/src/bigbucks_db.egg-info/
+-rw-r--r--   0 hanyuduan   (501) staff       (20)    10908 2023-04-11 00:34:02.000000 bigbucks_db-0.0.5/src/bigbucks_db.egg-info/PKG-INFO
+-rw-r--r--   0 hanyuduan   (501) staff       (20)      249 2023-04-11 00:34:02.000000 bigbucks_db-0.0.5/src/bigbucks_db.egg-info/SOURCES.txt
+-rw-r--r--   0 hanyuduan   (501) staff       (20)        1 2023-04-11 00:34:02.000000 bigbucks_db-0.0.5/src/bigbucks_db.egg-info/dependency_links.txt
+-rw-r--r--   0 hanyuduan   (501) staff       (20)       21 2023-04-11 00:34:02.000000 bigbucks_db-0.0.5/src/bigbucks_db.egg-info/top_level.txt
+-rw-r--r--   0 hanyuduan   (501) staff       (20)    16376 2023-04-10 22:34:31.000000 bigbucks_db-0.0.5/src/bigbucks_db.py
+drwxr-xr-x   0 hanyuduan   (501) staff       (20)        0 2023-04-11 00:34:02.347708 bigbucks_db-0.0.5/tests/
+-rw-r--r--   0 hanyuduan   (501) staff       (20)     1177 2023-04-11 00:30:15.000000 bigbucks_db-0.0.5/tests/test_bigbucks_db.py
```

### Comparing `bigbucks_db-0.0.4/LICENSE` & `bigbucks_db-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bigbucks_db-0.0.4/PKG-INFO` & `bigbucks_db-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: bigbucks_db
-Version: 0.0.4
-Summary: This is for FINTECH 512 Group Project Backend Supabase Database
-Author-email: Jeff Duan <jeffduan19@gmail.com>
-Project-URL: Homepage, https://github.com/codemakerss/512_BigBucks_Proj_Pkg
-Project-URL: Bug Tracker, https://github.com/codemakerss/512_BigBucks_Proj_Pkg/issues
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 512_BigBucks_Proj_Pkg Documentation
 
 ## Preview
 
 This is for FINTECH 512 Group Project Backend Supabase Database.
 
 We are using Supabase PostgresSQL database for our project. For more information, visit [Supabase Website](https://supabase.com/).
@@ -152,15 +137,15 @@
 # tmp[0] is the table name, tmp[1] is the data needs to be updated
 db.supabase_insert_function(tmp[0], tmp[1]) 
 print(tmp)
 ```
 
 - Update Transaction_Records
 
-  Note : by running this function, both Stock_Information table and Customer_Information's account balance will be also synchronized
+  Note : by running this function, both Stock_Information table and Customer_Information's account balance will be also synchronized, now can also update the Stock_Price_Daily_Data at the same time
 
 ```python
 # Example Code
 # below are information needs to be included
 from bigbucks_db import *
 # Enter database url and keys here
 SUPABASE_URL = ""
```

### Comparing `bigbucks_db-0.0.4/README.md` & `bigbucks_db-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: bigbucks_db
+Version: 0.0.5
+Summary: This is for FINTECH 512 Group Project Backend Supabase Database
+Author-email: Jeff Duan <jeffduan19@gmail.com>
+Project-URL: Homepage, https://github.com/codemakerss/512_BigBucks_Proj_Pkg
+Project-URL: Bug Tracker, https://github.com/codemakerss/512_BigBucks_Proj_Pkg/issues
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 512_BigBucks_Proj_Pkg Documentation
 
 ## Preview
 
 This is for FINTECH 512 Group Project Backend Supabase Database.
 
 We are using Supabase PostgresSQL database for our project. For more information, visit [Supabase Website](https://supabase.com/).
@@ -137,15 +152,15 @@
 # tmp[0] is the table name, tmp[1] is the data needs to be updated
 db.supabase_insert_function(tmp[0], tmp[1]) 
 print(tmp)
 ```
 
 - Update Transaction_Records
 
-  Note : by running this function, both Stock_Information table and Customer_Information's account balance will be also synchronized
+  Note : by running this function, both Stock_Information table and Customer_Information's account balance will be also synchronized, now can also update the Stock_Price_Daily_Data at the same time
 
 ```python
 # Example Code
 # below are information needs to be included
 from bigbucks_db import *
 # Enter database url and keys here
 SUPABASE_URL = ""
```

### Comparing `bigbucks_db-0.0.4/pyproject.toml` & `bigbucks_db-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "yfinance"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "bigbucks_db"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jeff Duan", email="jeffduan19@gmail.com" },
 ]
 description = "This is for FINTECH 512 Group Project Backend Supabase Database"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `bigbucks_db-0.0.4/src/bigbucks_db.egg-info/PKG-INFO` & `bigbucks_db-0.0.5/src/bigbucks_db.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigbucks-db
-Version: 0.0.4
+Version: 0.0.5
 Summary: This is for FINTECH 512 Group Project Backend Supabase Database
 Author-email: Jeff Duan <jeffduan19@gmail.com>
 Project-URL: Homepage, https://github.com/codemakerss/512_BigBucks_Proj_Pkg
 Project-URL: Bug Tracker, https://github.com/codemakerss/512_BigBucks_Proj_Pkg/issues
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -152,15 +152,15 @@
 # tmp[0] is the table name, tmp[1] is the data needs to be updated
 db.supabase_insert_function(tmp[0], tmp[1]) 
 print(tmp)
 ```
 
 - Update Transaction_Records
 
-  Note : by running this function, both Stock_Information table and Customer_Information's account balance will be also synchronized
+  Note : by running this function, both Stock_Information table and Customer_Information's account balance will be also synchronized, now can also update the Stock_Price_Daily_Data at the same time
 
 ```python
 # Example Code
 # below are information needs to be included
 from bigbucks_db import *
 # Enter database url and keys here
 SUPABASE_URL = ""
```

### Comparing `bigbucks_db-0.0.4/src/bigbucks_db.py` & `bigbucks_db-0.0.5/src/bigbucks_db.py`

 * *Files 13% similar despite different names*

```diff
@@ -132,14 +132,18 @@
 		self.update_customer_balance(customer_id, stock_amount_spent, condition)
 
 		# update stock symbol information
 		objs = Stock_Data(self.url, self.keys, self.stock_keys)
 		stock_info = objs.get_stock_information(stock_symbol)
 		objs.update_stock_info(stock_info)
 
+		# update stock 5 year price data if not previously stored
+		objs2 = Table_View(self.url,self.keys)
+		objs2.update_five_year_data("Stock_Information")
+
 		return "Transaction_Records", transactions
 
 	def update_customer_balance(self, customer_id : int, stock_amount_spent : float, condition : str):
 		try:
 			# get current balance from customer info
 			api_url = self.url + "/rest/v1/" + "Customer_Information" + "?customer_id=eq." + str(customer_id)
 			parameters =  {"apikey":self.keys}
@@ -154,14 +158,15 @@
 
 			# update the customer account balance 
 			data_to_insert = {"account_balance" : update_balance}
 			response = requests.patch(url = api_url, params = parameters, json = data_to_insert)
 		except:
 			print("Fail to update customer balance")
 
+
 	def supabase_insert_function(self, table_name : str, data_to_insert : dict)->str:
 		"""
 		excute rest api command to insert data to supabase 
 		"""
 		try:
 			# route to table
 			api_url = self.url + "/rest/v1/" + table_name
@@ -315,14 +320,67 @@
 		api_url = self.url + "/rest/v1/" + table_name
 		parameters =  {"apikey":self.keys}
 		response = requests.get(url = api_url, params = parameters)
 		data = response.json()
 
 		return data
 
+	# more features
+	def store_stock_price_data2(self, stock_symbol : str):
+		base_url = 'https://www.alphavantage.co/query?'
+		params = {"function": "TIME_SERIES_DAILY_ADJUSTED", "symbol": stock_symbol, "outputsize" : "full","apikey": "9Q91BWGMOE13WOR3"}
+		
+		response = requests.get(base_url, params=params)
+		data = response.json() # dict
+		# store all data 
+		#all_data[stock_symbol] = data['Time Series (Daily)']
+
+		return data
+
+	# update 5 year stock data here
+	def update_five_year_data(self, table_name : str):
+		try:
+			# objs = Table_View(self.url, self.keys)
+			stock_info = self.view_table_data(table_name)
+
+			all_symbols = []
+			for d in stock_info:
+				all_symbols.append(d['stock_symbol'])
+
+			# check if exists in the stock information table
+			for sym in all_symbols:
+				price_data = self.view_symbol_price_data(sym)
+
+				if (len(price_data) == 0):
+					# get date now
+					now = pendulum.now()
+					five_years_ago = now.subtract(years=5).date()
+					#print('2018-05-01' >= str(five_years_ago))
+
+					price1 = self.store_stock_price_data2("MSFT")
+					# call Table_Updates object
+					db = Table_Updates(self.url, self.keys, "9Q91BWGMOE13WOR3")
+					price = price1["Time Series (Daily)"]
+					ct = 0
+
+					for date, p in price.items():
+						if (str(date) >= str(five_years_ago)):
+							time.sleep(0.1)
+							data_to_insert = db.update_stock_daily_price(sym, date, p['1. open'], p['2. high'], p['3. low'], p['4. close'], p['5. adjusted close'], p['6. volume'])
+							db.supabase_insert_function(data_to_insert[0], data_to_insert[1])
+
+							ct = ct + 1
+							#print(ct)
+
+			#return all_symbols
+			print("all symbols not in database were updated")
+		except:
+			print("check symbol in the stock information")
+
+
 	# get all symbol 5 years price data
 	def view_symbol_price_data(self, symbol_name : str):
 		api_url = self.url + "/rest/v1/" + "Stock_Price_Daily_Data" + "?stock_symbol=eq." + symbol_name
 		parameters =  {"apikey":self.keys}
 		response = requests.get(url = api_url, params = parameters)
 		data = response.json()
 
@@ -459,11 +517,7 @@
 		data = yf.download(tickers= "^GSPC", period='1d')
 
 		return float(data.iloc[-1]["Adj Close"])
 
 
 
 
-
-
-
-
```

### Comparing `bigbucks_db-0.0.4/tests/test_bigbucks_db.py` & `bigbucks_db-0.0.5/tests/test_bigbucks_db.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import sys
 sys.path.append('../src') 
 
 import bigbucks_db as bk
 
 STOCK_API_KEYS = "9Q91BWGMOE13WOR3"
 # Enter database url and keys here
-SUPABASE_URL = ""
-KEYS = ""
+# SUPABASE_URL = ""
+# KEYS = ""
 
-# db = bk.Table_Updates(SUPABASE_URL, KEYS, STOCK_API_KEYS)
+import time
+start_time = time.time()
 
+db = bk.Table_Updates(SUPABASE_URL, KEYS, STOCK_API_KEYS)
+a = db.update_5_year_data()
+print()
 # objs = bk.Buy_And_Sell("9Q91BWGMOE13WOR3")
 # price = objs.get_realtime_stock_price("IBM")
 # print(price)
 
 # test = db.update_transaction_records("Jeffd", "buy", "IBM", 100, price)
 # print(test)
 
 # connect = db.supabase_insert_function(test[0], test[1])
 
-import time
-start_time = time.time()
 #ob2 = bk.Stock_Data(SUPABASE_URL, KEYS, STOCK_API_KEYS)
 # data = ob2.get_stock_information("IBM")
 # ob2.update_stock_info(data)
 
 # data2 = ob2.update_all_stock_price()
 # print(data2)
 # print(ob2.check_symbol_exist("AAPL"))
 
-data3 = bk.Table_View(SUPABASE_URL,KEYS)
-d3 = data3.view_customer_portfolio("Jeffd")
-print(d3)
+# data3 = bk.Table_View(SUPABASE_URL,KEYS)
+# d3 = data3.view_symbol_price_data("AAPL")
+# print(d3)
 # data4 = bk.SP500(SUPABASE_URL, KEYS, STOCK_API_KEYS)
 # d4 = data4.realtime_sp500()
 # print(d4)
 # test = bk.Buy_And_Sell(STOCK_API_KEYS)
 # print(test.realtime_price_bkp("MSFT"))
 
 end_time = time.time()
```

