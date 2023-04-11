# Comparing `tmp/cchenutils-0.0.7-py3-none-any.whl.zip` & `tmp/cchenutils-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 121571 bytes, number of entries: 102
--rw-rw-rw-  2.0 fat      117 b- defN 23-Apr-11 02:10 cchenutils/__init__.py
+Zip file size: 122800 bytes, number of entries: 103
+-rw-rw-rw-  2.0 fat      151 b- defN 23-Apr-11 05:09 cchenutils/__init__.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Mar-31 11:06 cchenutils/dict.py
--rw-rw-rw-  2.0 fat      728 b- defN 23-Apr-11 02:08 cchenutils/gmail.py
+-rw-rw-rw-  2.0 fat     1017 b- defN 23-Apr-11 02:40 cchenutils/gmail.py
 -rw-rw-rw-  2.0 fat     1936 b- defN 23-Apr-10 09:39 cchenutils/session.py
+-rw-rw-rw-  2.0 fat     3886 b- defN 23-Apr-11 05:59 cchenutils/timer.py
 -rw-rw-rw-  2.0 fat      150 b- defN 20-Mar-21 19:46 wanghong/__init__.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 20-Mar-24 05:56 wanghong/async.py
 -rw-rw-rw-  2.0 fat     1347 b- defN 20-Mar-23 22:38 wanghong/dataprep.py
 -rw-rw-rw-  2.0 fat      784 b- defN 20-Apr-06 03:33 wanghong/opts.py
 -rw-rw-rw-  2.0 fat     1717 b- defN 21-Mar-06 19:19 wanghong/test.py
 -rw-rw-rw-  2.0 fat     4258 b- defN 21-Mar-23 02:17 wanghong/utils.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-21 23:45 wanghong/3rdparty/__init__.py
@@ -92,13 +93,13 @@
 -rw-rw-rw-  2.0 fat     3312 b- defN 20-Mar-24 00:35 wanghong/video/prep/wav_split.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/__init__.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/taobao/__init__.py
 -rw-rw-rw-  2.0 fat     4548 b- defN 20-Apr-05 03:47 wanghong/webscraping/taobao/items_cover.py
 -rw-rw-rw-  2.0 fat     4874 b- defN 20-Mar-27 20:44 wanghong/webscraping/taobao/taobao_shopinfo_manual.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/yizhibo/__init__.py
 -rw-rw-rw-  2.0 fat     8389 b- defN 20-Mar-26 19:40 wanghong/webscraping/yizhibo/ts_downbind.py
--rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-11 02:10 cchenutils-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 02:10 cchenutils-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 02:10 cchenutils-0.0.7.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.0.7.dist-info/zip-safe
--rw-rw-r--  2.0 fat     9038 b- defN 23-Apr-11 02:10 cchenutils-0.0.7.dist-info/RECORD
-102 files, 346619 bytes uncompressed, 107173 bytes compressed:  69.1%
+-rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-11 06:00 cchenutils-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 06:00 cchenutils-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 06:00 cchenutils-0.0.8.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.0.8.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     9115 b- defN 23-Apr-11 06:00 cchenutils-0.0.8.dist-info/RECORD
+103 files, 350905 bytes uncompressed, 108288 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: cchenutils/gmail.py
 Comment: 
 
 Filename: cchenutils/session.py
 Comment: 
 
+Filename: cchenutils/timer.py
+Comment: 
+
 Filename: wanghong/__init__.py
 Comment: 
 
 Filename: wanghong/async.py
 Comment: 
 
 Filename: wanghong/dataprep.py
@@ -285,23 +288,23 @@
 
 Filename: wanghong/webscraping/yizhibo/__init__.py
 Comment: 
 
 Filename: wanghong/webscraping/yizhibo/ts_downbind.py
 Comment: 
 
-Filename: cchenutils-0.0.7.dist-info/METADATA
+Filename: cchenutils-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: cchenutils-0.0.7.dist-info/WHEEL
+Filename: cchenutils-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: cchenutils-0.0.7.dist-info/top_level.txt
+Filename: cchenutils-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: cchenutils-0.0.7.dist-info/zip-safe
+Filename: cchenutils-0.0.8.dist-info/zip-safe
 Comment: 
 
-Filename: cchenutils-0.0.7.dist-info/RECORD
+Filename: cchenutils-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cchenutils/__init__.py

```diff
@@ -1,5 +1,6 @@
 from .dict import dict
-from .session import Session
 from .gmail import Gmail
+from .session import Session
+from .timer import Timer
 
-__all__ = ['dict', 'Session', 'Gmail']
+__all__ = ['dict', 'Session', 'Gmail', 'Timer']
```

## cchenutils/gmail.py

```diff
@@ -1,12 +1,20 @@
 import smtplib
 
 
 class Gmail:
     def __init__(self, account, app_password):
+        """App password can be obtained:
+        1. https://myaccount.google.com/
+        2. Security
+        3. under `How you sign in to Google`, click 2-Step Verification
+        4. App passwords
+
+        Reference: https://support.google.com/accounts/answer/185833
+        """
         self.account = account if '@' in account else f'{account}@gmail.com'
         self.server = smtplib.SMTP('smtp.gmail.com', 587)
         self.server.starttls()
         self.server.login(self.account, app_password)
 
     def send(self, to=None, subject=None, body=None):
         to = self.account if to is None else (to if '@' in to else f'{to}@gmail.com')
```

## Comparing `cchenutils-0.0.7.dist-info/RECORD` & `cchenutils-0.0.8.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-cchenutils/__init__.py,sha256=dDFPG7cpBX8XURd78db3uqjQ7sQ0xWiSSiFErfM5_fo,117
+cchenutils/__init__.py,sha256=NK8fpQKQxgbn5P3wN9Bxi_LPo5A68xczmzBnKKMI1n0,151
 cchenutils/dict.py,sha256=IO_6WLY3xZB8huHpwgKCbYEL3d31TllDWdhoSF8Kz6c,613
-cchenutils/gmail.py,sha256=LzfzotqhFR_Q97Lp2TNmaILrW47O94Wi3gjhA2MSe4Q,728
+cchenutils/gmail.py,sha256=yRuA6TxNTxYSTnMV23SFsW0I4xpCm6gMoTxe1bqFT68,1017
 cchenutils/session.py,sha256=7k67EyOxZFBhEB4Mr4sj7PS8IZeb5Whiic4de2g540c,1936
+cchenutils/timer.py,sha256=Z0GXkpMkW5RpvsEpKdncJhEs8qhnAQ0Nu6dlysoR43k,3886
 wanghong/__init__.py,sha256=nNr59H3MLTTN-oZoTCUhyOXw0282nv2lzsyom0EbEi0,150
 wanghong/async.py,sha256=5Mb-lTfhRaSYtBHcw4-PT9iV3ohu3aRNaC33okI9Pb8,1372
 wanghong/dataprep.py,sha256=8UEMnrbuPhQ8_ts_HAF9L6FQCj3Rhm3YFjIQFlI5zwY,1347
 wanghong/opts.py,sha256=T5pwfVsmma7B8OKVycfL5ddsapTpvzpNU4bOCtSccNs,784
 wanghong/test.py,sha256=jCN-cUTttNazLmN1tQb1OquGygddmwrsbZ2Gjpej4y0,1717
 wanghong/utils.py,sha256=MgPrC6cJoxon8ooopYx8BvN17GEbAW7TOTPs61RsER0,4258
 wanghong/3rdparty/__init__.py,sha256=7XnItt31RApVDO03DMqxuIVRpnNkhiBmpB8Ue5Nwm-8,152
@@ -91,12 +92,12 @@
 wanghong/video/prep/wav_split.py,sha256=UJ6iKDszpjRtpxGfE_-h_GAa_uT1dXd0ll_7zJ_2Icc,3312
 wanghong/webscraping/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/items_cover.py,sha256=xt1swF6RCnpR0eLJMsuhEkyLqw9M9GGa4BZfoPI-Egs,4548
 wanghong/webscraping/taobao/taobao_shopinfo_manual.py,sha256=wYjqTHCW4NcU8Qy8eLIi-ZpNgsXsNYeXeP7-eyMtVTw,4874
 wanghong/webscraping/yizhibo/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/yizhibo/ts_downbind.py,sha256=u-VOJl_EAsoA4Ep81XdF0GXeSc3Vr1QkmXnLDBca79o,8389
-cchenutils-0.0.7.dist-info/METADATA,sha256=bY-g0KPYJygWaKD68CxBFWMejQ3Rsc0IBFOXP5OOhW0,196
-cchenutils-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cchenutils-0.0.7.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
-cchenutils-0.0.7.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-cchenutils-0.0.7.dist-info/RECORD,,
+cchenutils-0.0.8.dist-info/METADATA,sha256=Pt-YWSG-5pAYHFRZX5gbmGG8zOTUhvs-gUaBjB9R_90,196
+cchenutils-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cchenutils-0.0.8.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
+cchenutils-0.0.8.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+cchenutils-0.0.8.dist-info/RECORD,,
```

