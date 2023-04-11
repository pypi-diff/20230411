# Comparing `tmp/cchenutils-0.4.1-py3-none-any.whl.zip` & `tmp/cchenutils-0.4.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 122834 bytes, number of entries: 103
+Zip file size: 123440 bytes, number of entries: 104
 -rw-rw-rw-  2.0 fat      151 b- defN 23-Apr-11 05:09 cchenutils/__init__.py
+-rw-rw-rw-  2.0 fat     1162 b- defN 23-Apr-11 07:30 cchenutils/_monitor.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Mar-31 11:06 cchenutils/dict.py
--rw-rw-rw-  2.0 fat     1017 b- defN 23-Apr-11 02:40 cchenutils/gmail.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-11 07:18 cchenutils/gmail.py
 -rw-rw-rw-  2.0 fat     1936 b- defN 23-Apr-10 09:39 cchenutils/session.py
 -rw-rw-rw-  2.0 fat     4375 b- defN 23-Apr-11 06:27 cchenutils/timer.py
 -rw-rw-rw-  2.0 fat      150 b- defN 20-Mar-21 19:46 wanghong/__init__.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 20-Mar-24 05:56 wanghong/async.py
 -rw-rw-rw-  2.0 fat     1347 b- defN 20-Mar-23 22:38 wanghong/dataprep.py
 -rw-rw-rw-  2.0 fat      784 b- defN 20-Apr-06 03:33 wanghong/opts.py
 -rw-rw-rw-  2.0 fat     1717 b- defN 21-Mar-06 19:19 wanghong/test.py
@@ -93,13 +94,13 @@
 -rw-rw-rw-  2.0 fat     3312 b- defN 20-Mar-24 00:35 wanghong/video/prep/wav_split.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/__init__.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/taobao/__init__.py
 -rw-rw-rw-  2.0 fat     4548 b- defN 20-Apr-05 03:47 wanghong/webscraping/taobao/items_cover.py
 -rw-rw-rw-  2.0 fat     4874 b- defN 20-Mar-27 20:44 wanghong/webscraping/taobao/taobao_shopinfo_manual.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/yizhibo/__init__.py
 -rw-rw-rw-  2.0 fat     8389 b- defN 20-Mar-26 19:40 wanghong/webscraping/yizhibo/ts_downbind.py
--rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-11 06:28 cchenutils-0.4.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 06:28 cchenutils-0.4.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 06:28 cchenutils-0.4.1.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.4.1.dist-info/zip-safe
--rw-rw-r--  2.0 fat     9115 b- defN 23-Apr-11 06:28 cchenutils-0.4.1.dist-info/RECORD
-103 files, 351394 bytes uncompressed, 108322 bytes compressed:  69.2%
+-rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-11 07:37 cchenutils-0.4.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 07:37 cchenutils-0.4.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 07:37 cchenutils-0.4.2.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.4.2.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     9194 b- defN 23-Apr-11 07:37 cchenutils-0.4.2.dist-info/RECORD
+104 files, 352682 bytes uncompressed, 108808 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -1,10 +1,13 @@
 Filename: cchenutils/__init__.py
 Comment: 
 
+Filename: cchenutils/_monitor.py
+Comment: 
+
 Filename: cchenutils/dict.py
 Comment: 
 
 Filename: cchenutils/gmail.py
 Comment: 
 
 Filename: cchenutils/session.py
@@ -288,23 +291,23 @@
 
 Filename: wanghong/webscraping/yizhibo/__init__.py
 Comment: 
 
 Filename: wanghong/webscraping/yizhibo/ts_downbind.py
 Comment: 
 
-Filename: cchenutils-0.4.1.dist-info/METADATA
+Filename: cchenutils-0.4.2.dist-info/METADATA
 Comment: 
 
-Filename: cchenutils-0.4.1.dist-info/WHEEL
+Filename: cchenutils-0.4.2.dist-info/WHEEL
 Comment: 
 
-Filename: cchenutils-0.4.1.dist-info/top_level.txt
+Filename: cchenutils-0.4.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cchenutils-0.4.1.dist-info/zip-safe
+Filename: cchenutils-0.4.2.dist-info/zip-safe
 Comment: 
 
-Filename: cchenutils-0.4.1.dist-info/RECORD
+Filename: cchenutils-0.4.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cchenutils/gmail.py

```diff
@@ -1,28 +1,29 @@
 import smtplib
 
 
 class Gmail:
-    def __init__(self, account, app_password):
+    def __init__(self, account, app_password, to=None, subject=None):
         """App password can be obtained:
         1. https://myaccount.google.com/
         2. Security
         3. under `How you sign in to Google`, click 2-Step Verification
         4. App passwords
 
         Reference: https://support.google.com/accounts/answer/185833
         """
         self.account = account if '@' in account else f'{account}@gmail.com'
         self.server = smtplib.SMTP('smtp.gmail.com', 587)
         self.server.starttls()
         self.server.login(self.account, app_password)
+        self.to = self.account if to is None else (to if '@' in to else f'{to}@gmail.com')
+        self.subject = subject
 
-    def send(self, to=None, subject=None, body=None):
-        to = self.account if to is None else (to if '@' in to else f'{to}@gmail.com')
-        message = body if subject is None else 'Subject: {}\n\n{}'.format(subject, body)
-        self.server.sendmail(self.account, to, message)
+    def send(self, body):
+        message = body if self.subject is None else 'Subject: {}\n\n{}'.format(self.subject, body)
+        self.server.sendmail(self.account, self.to, message)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.server.quit()
```

## Comparing `cchenutils-0.4.1.dist-info/RECORD` & `cchenutils-0.4.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 cchenutils/__init__.py,sha256=NK8fpQKQxgbn5P3wN9Bxi_LPo5A68xczmzBnKKMI1n0,151
+cchenutils/_monitor.py,sha256=drOt6YBZGcbb2ZqMqGEslQlZWcCJW3GeN6T-XpHJ5R0,1162
 cchenutils/dict.py,sha256=IO_6WLY3xZB8huHpwgKCbYEL3d31TllDWdhoSF8Kz6c,613
-cchenutils/gmail.py,sha256=yRuA6TxNTxYSTnMV23SFsW0I4xpCm6gMoTxe1bqFT68,1017
+cchenutils/gmail.py,sha256=5VIF9-OyzpjWbB0waR1hogtbT66ZqXwFeaCPdrIcMko,1064
 cchenutils/session.py,sha256=7k67EyOxZFBhEB4Mr4sj7PS8IZeb5Whiic4de2g540c,1936
 cchenutils/timer.py,sha256=kyeBOyQSoByfevSjpKVFUjU3rGswzYkjG9-hSfs0Ols,4375
 wanghong/__init__.py,sha256=nNr59H3MLTTN-oZoTCUhyOXw0282nv2lzsyom0EbEi0,150
 wanghong/async.py,sha256=5Mb-lTfhRaSYtBHcw4-PT9iV3ohu3aRNaC33okI9Pb8,1372
 wanghong/dataprep.py,sha256=8UEMnrbuPhQ8_ts_HAF9L6FQCj3Rhm3YFjIQFlI5zwY,1347
 wanghong/opts.py,sha256=T5pwfVsmma7B8OKVycfL5ddsapTpvzpNU4bOCtSccNs,784
 wanghong/test.py,sha256=jCN-cUTttNazLmN1tQb1OquGygddmwrsbZ2Gjpej4y0,1717
@@ -92,12 +93,12 @@
 wanghong/video/prep/wav_split.py,sha256=UJ6iKDszpjRtpxGfE_-h_GAa_uT1dXd0ll_7zJ_2Icc,3312
 wanghong/webscraping/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/items_cover.py,sha256=xt1swF6RCnpR0eLJMsuhEkyLqw9M9GGa4BZfoPI-Egs,4548
 wanghong/webscraping/taobao/taobao_shopinfo_manual.py,sha256=wYjqTHCW4NcU8Qy8eLIi-ZpNgsXsNYeXeP7-eyMtVTw,4874
 wanghong/webscraping/yizhibo/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/yizhibo/ts_downbind.py,sha256=u-VOJl_EAsoA4Ep81XdF0GXeSc3Vr1QkmXnLDBca79o,8389
-cchenutils-0.4.1.dist-info/METADATA,sha256=hNTG-RLxsGDgx60oQkXxxY3IPgKhqc4ehZgHUQp8olk,196
-cchenutils-0.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cchenutils-0.4.1.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
-cchenutils-0.4.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-cchenutils-0.4.1.dist-info/RECORD,,
+cchenutils-0.4.2.dist-info/METADATA,sha256=1LgtaaG2__hxuMyXlIVXlFi611XE_SV0eLBiLywsEqU,196
+cchenutils-0.4.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cchenutils-0.4.2.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
+cchenutils-0.4.2.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+cchenutils-0.4.2.dist-info/RECORD,,
```

