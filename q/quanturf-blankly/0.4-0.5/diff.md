# Comparing `tmp/quanturf_blankly-0.4.tar.gz` & `tmp/quanturf_blankly-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanturf_blankly-0.4.tar", last modified: Tue Apr 11 13:34:06 2023, max compression
+gzip compressed data, was "quanturf_blankly-0.5.tar", last modified: Tue Apr 11 13:51:32 2023, max compression
```

## Comparing `quanturf_blankly-0.4.tar` & `quanturf_blankly-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 13:34:06.065414 quanturf_blankly-0.4/
--rw-rw-rw-   0        0        0      509 2023-04-11 13:34:06.063426 quanturf_blankly-0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 13:34:06.048442 quanturf_blankly-0.4/quanturf_blankly/
--rw-rw-rw-   0        0        0        0 2023-03-21 18:01:57.000000 quanturf_blankly-0.4/quanturf_blankly/__init__.py
--rw-rw-rw-   0        0        0    14719 2023-04-10 19:46:29.000000 quanturf_blankly-0.4/quanturf_blankly/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 13:34:06.058444 quanturf_blankly-0.4/quanturf_blankly.egg-info/
--rw-rw-rw-   0        0        0      509 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       58 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-11 13:34:05.000000 quanturf_blankly-0.4/quanturf_blankly.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 13:34:06.065414 quanturf_blankly-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1066 2023-04-11 13:33:54.000000 quanturf_blankly-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:51:32.083830 quanturf_blankly-0.5/
+-rw-rw-rw-   0        0        0      509 2023-04-11 13:51:32.082828 quanturf_blankly-0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 13:51:32.071819 quanturf_blankly-0.5/quanturf_blankly/
+-rw-rw-rw-   0        0        0        0 2023-03-21 18:01:57.000000 quanturf_blankly-0.5/quanturf_blankly/__init__.py
+-rw-rw-rw-   0        0        0    14967 2023-04-11 13:50:00.000000 quanturf_blankly-0.5/quanturf_blankly/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:51:32.081817 quanturf_blankly-0.5/quanturf_blankly.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-04-11 13:51:31.000000 quanturf_blankly-0.5/quanturf_blankly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-04-11 13:51:31.000000 quanturf_blankly-0.5/quanturf_blankly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:51:31.000000 quanturf_blankly-0.5/quanturf_blankly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-11 13:51:31.000000 quanturf_blankly-0.5/quanturf_blankly.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       58 2023-04-11 13:51:31.000000 quanturf_blankly-0.5/quanturf_blankly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-11 13:51:31.000000 quanturf_blankly-0.5/quanturf_blankly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 13:51:32.083830 quanturf_blankly-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1066 2023-04-11 13:51:20.000000 quanturf_blankly-0.5/setup.py
```

### Comparing `quanturf_blankly-0.4/quanturf_blankly/__main__.py` & `quanturf_blankly-0.5/quanturf_blankly/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,36 @@
 import requests
 import pandas as pd
 import datetime as dt
 import numpy as np
 import os
 
 api=""
+base_dir=""
 
 def environment(dir_path):
     global api
-  
+    global base_dir
+    
+    base_dir=dir_path
     with open(os.path.join(dir_path, 'keys.json')) as keys_file:
         json_data=json.load(keys_file)
         strategy_name=""
         for x in json_data["alpaca"]:
             strategy_name=x
     
     api=tradeapi.REST(key_id=json_data['alpaca'][strategy_name]['API_KEY'],
                      secret_key=json_data['alpaca'][strategy_name]['API_SECRET'],
                      base_url="https://paper-api.alpaca.markets",
                      api_version='V2')
             
 
 def realized_profit_df_strategy():
-    with open('transactions.json') as json_data:
+    global base_dir
+    with open(os.path.join(base_dir, 'transactions.json')) as json_data:
         data = json.load(json_data)
     df = pd.json_normalize(data,record_path=['transaction'])
 
     result_df = pd.DataFrame(columns = ['Qty','Price','Symbol','Transaction_time','order_id','Type'])
     order_id_list = []
     qty_list = []
     price_list = []
@@ -99,15 +103,15 @@
                     for ix in idx:
                         obs.append(ix)
     
     return output_frame
 
 def unrealised_profit_df_strategy():
 
-    with open('transactions.json') as json_data:
+    with open(os.path.join(base_dir, 'transactions.json')) as json_data:
         data = json.load(json_data)
     df = pd.json_normalize(data,record_path=['transaction'])
 
     sell_order_list=[]
     buy_order_list=[]    
 
     for index,obj in df.iterrows():
@@ -306,15 +310,15 @@
     cum_returns = np.cumsum(pnl_vector_list)
     cum_high = np.maximum.accumulate(cum_returns)
     np.seterr(invalid='ignore')
     drawdown = (cum_high - cum_returns) / cum_high
     drawdown=np.max(drawdown)
     drawdown=round(drawdown,2)
 
-    json_file=open("transactions.json","r")
+    json_file=open(os.path.join(base_dir, 'transactions.json'),"r")
     data=json.load(json_file)
     data=dict(data)
     container_id=data['container_id']
     json_file.close()
     
     json_data={
         'container_id':container_id,
@@ -353,34 +357,34 @@
             'Time':order['created_at'],
             'Status':order['status'],
             'Type':order['side'],
             'order ID':order['id'],
             'Formated_time':order_datetime
         }
     
-    json_file=open("transactions.json","r")
+    json_file=open(os.path.join(base_dir, 'transactions.json'),"r")
     data=json.load(json_file)
     data=dict(data)
     data["transaction"].append(dict(transaction_data))
     json_file.close()
-    json_file=open("transactions.json","w")
+    json_file=open(os.path.join(base_dir, 'transactions.json'),"w")
     json_file.write(json.dumps(data))
     json_file.close()
 
-    json_file=open("transactions.json","r")
+    json_file=open(os.path.join(base_dir, 'transactions.json'),"r")
     data=json.load(json_file)
     data=dict(data)
    
     close_positions=realized_profit_df_strategy()
     open_positions=unrealised_profit_df_strategy()
     data['open']=open_positions
     data['close']=close_positions
     json_file.close()
 
-    json_file=open("transactions.json","w")
+    json_file=open(os.path.join(base_dir, 'transactions.json'),"w")
     json_file.write(json.dumps(data))
     json_file.close()
 
     transaction_data=json.dumps(data)
     URL="https://quanturf.com/api/transaction/"
     headers = {'Content-type': 'application/json'}
     transaction_request=requests.post(url=URL,data=transaction_data,headers=headers)
```

### Comparing `quanturf_blankly-0.4/setup.py` & `quanturf_blankly-0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 import sys
 
 setup_args=dict(
     name="quanturf_blankly",
     packages=['quanturf_blankly'],
-    version='0.4',
+    version='0.5',
     description="",
     long_description="",
     author="Quanturf",
     url="https://github.com/Quanturf/quanturf_blankly_package",
     author_email="quanturf.finance@gmail.com",
     classifiers=[
         'Intended Audience :: Developers',
```

