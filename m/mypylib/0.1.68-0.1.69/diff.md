# Comparing `tmp/mypylib-0.1.68.tar.gz` & `tmp/mypylib-0.1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.68.tar", last modified: Wed Mar 15 15:28:13 2023, max compression
+gzip compressed data, was "mypylib-0.1.69.tar", last modified: Tue Apr 11 13:56:02 2023, max compression
```

## Comparing `mypylib-0.1.68.tar` & `mypylib-0.1.69.tar`

### file list

```diff
@@ -1,38 +1,34 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-03-15 15:28:13.608386 mypylib-0.1.68/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-03-15 15:28:13.608098 mypylib-0.1.68/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.68/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-03-15 15:28:13.603472 mypylib-0.1.68/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.68/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    46895 2023-03-15 15:26:38.000000 mypylib-0.1.68/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.68/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.68/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.68/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.68/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2023-03-05 12:39:52.000000 mypylib-0.1.68/mypylib/dealer.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.68/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.68/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24230 2022-06-02 06:59:21.000000 mypylib-0.1.68/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.68/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.68/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.68/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2540 2023-03-05 12:39:52.000000 mypylib-0.1.68/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.68/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6857 2023-03-05 12:39:52.000000 mypylib-0.1.68/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.68/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7662 2022-06-02 06:59:21.000000 mypylib-0.1.68/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-03-15 15:28:13.607459 mypylib-0.1.68/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.68/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      627 2023-03-05 12:39:52.000000 mypylib-0.1.68/mypylib/tmpDevelopment/binance_api_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      162 2023-03-05 12:39:52.000000 mypylib-0.1.68/mypylib/tmpDevelopment/testssss.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1057 2023-03-05 12:39:52.000000 mypylib-0.1.68/mypylib/tmpDevelopment/visit_all_sj_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.68/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2443 2023-01-29 12:44:04.000000 mypylib-0.1.68/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.68/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-02-23 13:59:18.000000 mypylib-0.1.68/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-03-15 15:28:13.605170 mypylib-0.1.68/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-03-15 15:28:12.000000 mypylib-0.1.68/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      795 2023-03-15 15:28:13.000000 mypylib-0.1.68/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-03-15 15:28:13.000000 mypylib-0.1.68/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-03-15 15:28:13.000000 mypylib-0.1.68/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-03-15 15:28:13.608498 mypylib-0.1.68/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.68/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-11 13:56:02.123034 mypylib-0.1.69/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-04-11 13:56:02.122779 mypylib-0.1.69/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.69/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-11 13:56:02.120380 mypylib-0.1.69/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.69/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    46944 2023-04-11 13:50:45.000000 mypylib-0.1.69/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.69/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.69/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.69/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.69/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.69/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.69/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24230 2022-06-02 06:59:21.000000 mypylib-0.1.69/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.69/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.69/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.69/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.69/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.69/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6947 2023-04-11 13:47:35.000000 mypylib-0.1.69/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.69/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7662 2022-06-02 06:59:21.000000 mypylib-0.1.69/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-11 13:56:02.122064 mypylib-0.1.69/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.69/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.69/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2443 2023-01-29 12:44:04.000000 mypylib-0.1.69/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.69/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.69/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-04-11 13:56:02.121575 mypylib-0.1.69/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-04-11 13:56:01.000000 mypylib-0.1.69/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-04-11 13:56:02.000000 mypylib-0.1.69/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-04-11 13:56:01.000000 mypylib-0.1.69/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-04-11 13:56:01.000000 mypylib-0.1.69/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-04-11 13:56:02.123118 mypylib-0.1.69/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.69/setup.py
```

### Comparing `mypylib-0.1.68/README.md` & `mypylib-0.1.69/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.69/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/__init__.py` & `mypylib-0.1.69/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import requests
 
 ssl._create_default_https_context = ssl._create_unverified_context
 from termcolor import cprint
 from inspect import currentframe
 
-__version__ = '0.1.68'
+__version__ = '0.1.69'
 
 __info__ = {
     '2022/01/04: 0.1.18 加入 __info__。',
     '2022/01/04: 0.1.18 Carey修改 MVP的部分。',
     '2022/01/05: 0.1.19 add check_place_cover 預防漲停鎖住',
     '2022/01/06: 0.1.20 add get_stock_future_data(). 用來抓取每天股票期貨資料',
     '2022/01/06: 0.1.20 add get_stock_future_snapshot(). 用來抓每天股票、股票期貨漲停、跌停價格',
@@ -56,15 +56,16 @@
     '2023/01/07: 0.1.60 加入 Pause/TradeType/BestBuy/BestSell',
     '2023/01/12: 0.1.61 Remove redis debug message. Too annoying',
     '2023/01/29: 0.1.63 del xls in read_warrant_bible()',
     '2023/01/29: 0.1.64 add block for playsound class',
     '2023/02/12: 0.1.65 修改 sjtools parse timestamp的方法，以免crash',
     '2023/02/13: 0.1.66 Move toggle_btn_off and toggle_btn_on here ',
     '2023/02/23: 0.1.67 get_new_warrant_list() 元富修改網站，封鎖 read_html()',
-    '2023/03/15: 0.1.68 修正一些宣告'
+    '2023/03/15: 0.1.68 修正一些宣告',
+    '2023/04/11: 0.1.69 換成shioaji 1.0 API',
 
 }
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
```

### Comparing `mypylib-0.1.68/mypylib/binance_copy_bot.py` & `mypylib-0.1.69/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.69/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/chdbif.py` & `mypylib-0.1.69/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/crypto.py` & `mypylib-0.1.69/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/finmind.py` & `mypylib-0.1.69/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/libexcel.py` & `mypylib-0.1.69/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/mvp.py` & `mypylib-0.1.69/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/mytest.py` & `mypylib-0.1.69/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/option_test.py` & `mypylib-0.1.69/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.69/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/shioaji_kline.py` & `mypylib-0.1.69/mypylib/shioaji_kline.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
         if self.ts_end == 0:
             self.ts_end = (int(ts_now) // self.seconds + 1) * self.seconds
             self.OHLC = OHLC(self.ts_end)
 
         if ts_now > self.ts_end and self.OHLC is not None:
             self.feed()
-            ret = True
 
         self.OHLC.push(quote['Close'][0])
 
     def __getitem__(self, index):
         return self.list_OHLC.__getitem__(index)
 
 
@@ -77,9 +76,7 @@
             if topic[0] != 'M':
                 continue
 
             kline.feed_shioaji_quote(quote)
 
     for OHLC in kline.list_OHLC:
         print(f'{OHLC.datetime} {OHLC.Open} {OHLC.High} {OHLC.Low} {OHLC.Close}')
-
-    print(kline[-1].Open)
```

### Comparing `mypylib-0.1.68/mypylib/shioaji_ticks.py` & `mypylib-0.1.69/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/sjtools.py` & `mypylib-0.1.69/mypylib/sjtools.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,26 +134,26 @@
         return super().get('BestBuy')
 
     def BestSell(self) -> int:
         return super().get('BestSell')
 
 
 class SJ_wrapper:
-    def __init__(self, _id='H121933940', password='123'):
-        self._id = _id
-        self.password = password
+    def __init__(self, api_key, secret_key):
+        self.api_key = api_key
+        self.secret_key = secret_key
 
-        print(f'使用正式帳號 {_id} {password}')
+        print(f'使用正式帳號')
         self.api = sj.Shioaji()
-        self.api.login(_id, password, contracts_cb=lambda security_type: print(f"{repr(security_type)} fetch done."))
+        self.api.login(self.api_key, self.secret_key, contracts_cb=lambda security_type: print(f"{repr(security_type)} fetch done."))
 
 
 class SJ_downloader(SJ_wrapper):
-    def __init__(self, _id='H121933940', password='123'):
-        super(SJ_downloader, self).__init__(_id=_id, password=password)
+    def __init__(self, api_key, secret_key):
+        super(SJ_downloader, self).__init__(api_key, secret_key)
 
         self.ticks = None
 
     def download_ticks(self, contract: contracts, date: Union[str, datetime.datetime]):
         print(contract, date)
         ticks = self.api.ticks(contract=contract, date=date if isinstance(date, str) else datetime.datetime.strftime('%Y-%m-%d'))
         self.ticks = ticks
@@ -163,15 +163,16 @@
         df = pd.DataFrame({**self.ticks})
         df.ts = pd.to_datetime(df.ts)
 
         df.to_csv(filename)
 
 
 def unit_test_SJ_downloader():
-    downloader = SJ_downloader(_id='H121933940', password='123')
+    downloader = SJ_downloader(api_key='6Dkp67EVdMQBWE8Z6DZ5zPQAFTbvVPxEGzAEFiZ5ByhN',
+                               secret_key='2NCQAhfP73PfKYaAi8xJVHZSp4Y91mSNViiFU7zQ19T2')
 
     if not os.path.isfile('trade_days.txt'):
         trade_days = get_trade_days('2018-01-01', datetime.datetime.today())
         trade_days.reverse()
         with open('trade_days.txt', 'w+') as fp:
             json.dump(trade_days, fp)
     else:
```

### Comparing `mypylib-0.1.68/mypylib/tLineNotify.py` & `mypylib-0.1.69/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/ti.py` & `mypylib-0.1.69/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.69/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/tplaysound.py` & `mypylib-0.1.69/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/tredis.py` & `mypylib-0.1.69/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib/warrant.py` & `mypylib-0.1.69/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.68/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.69/mypylib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 setup.py
 mypylib/MP_shioaji_ticks.py
 mypylib/__init__.py
 mypylib/binance_copy_bot.py
 mypylib/binance_copy_bot_test.py
 mypylib/chdbif.py
 mypylib/crypto.py
-mypylib/dealer.py
 mypylib/finmind.py
 mypylib/libexcel.py
 mypylib/mvp.py
 mypylib/mytest.py
 mypylib/option_test.py
 mypylib/shioaji_history_ticks.py
 mypylib/shioaji_kline.py
@@ -22,11 +21,8 @@
 mypylib/tredis.py
 mypylib/warrant.py
 mypylib.egg-info/PKG-INFO
 mypylib.egg-info/SOURCES.txt
 mypylib.egg-info/dependency_links.txt
 mypylib.egg-info/top_level.txt
 mypylib/tmpDevelopment/__init__.py
-mypylib/tmpDevelopment/binance_api_test.py
-mypylib/tmpDevelopment/testssss.py
-mypylib/tmpDevelopment/visit_all_sj_ticks.py
 mypylib/tmpDevelopment/warrant_test.py
```

### Comparing `mypylib-0.1.68/setup.py` & `mypylib-0.1.69/setup.py`

 * *Files identical despite different names*

