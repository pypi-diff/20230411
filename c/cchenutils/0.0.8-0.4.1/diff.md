# Comparing `tmp/cchenutils-0.0.8-py3-none-any.whl.zip` & `tmp/cchenutils-0.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 122800 bytes, number of entries: 103
+Zip file size: 122834 bytes, number of entries: 103
 -rw-rw-rw-  2.0 fat      151 b- defN 23-Apr-11 05:09 cchenutils/__init__.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Mar-31 11:06 cchenutils/dict.py
 -rw-rw-rw-  2.0 fat     1017 b- defN 23-Apr-11 02:40 cchenutils/gmail.py
 -rw-rw-rw-  2.0 fat     1936 b- defN 23-Apr-10 09:39 cchenutils/session.py
--rw-rw-rw-  2.0 fat     3886 b- defN 23-Apr-11 05:59 cchenutils/timer.py
+-rw-rw-rw-  2.0 fat     4375 b- defN 23-Apr-11 06:27 cchenutils/timer.py
 -rw-rw-rw-  2.0 fat      150 b- defN 20-Mar-21 19:46 wanghong/__init__.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 20-Mar-24 05:56 wanghong/async.py
 -rw-rw-rw-  2.0 fat     1347 b- defN 20-Mar-23 22:38 wanghong/dataprep.py
 -rw-rw-rw-  2.0 fat      784 b- defN 20-Apr-06 03:33 wanghong/opts.py
 -rw-rw-rw-  2.0 fat     1717 b- defN 21-Mar-06 19:19 wanghong/test.py
 -rw-rw-rw-  2.0 fat     4258 b- defN 21-Mar-23 02:17 wanghong/utils.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-21 23:45 wanghong/3rdparty/__init__.py
@@ -93,13 +93,13 @@
 -rw-rw-rw-  2.0 fat     3312 b- defN 20-Mar-24 00:35 wanghong/video/prep/wav_split.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/__init__.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/taobao/__init__.py
 -rw-rw-rw-  2.0 fat     4548 b- defN 20-Apr-05 03:47 wanghong/webscraping/taobao/items_cover.py
 -rw-rw-rw-  2.0 fat     4874 b- defN 20-Mar-27 20:44 wanghong/webscraping/taobao/taobao_shopinfo_manual.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/yizhibo/__init__.py
 -rw-rw-rw-  2.0 fat     8389 b- defN 20-Mar-26 19:40 wanghong/webscraping/yizhibo/ts_downbind.py
--rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-11 06:00 cchenutils-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 06:00 cchenutils-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 06:00 cchenutils-0.0.8.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.0.8.dist-info/zip-safe
--rw-rw-r--  2.0 fat     9115 b- defN 23-Apr-11 06:00 cchenutils-0.0.8.dist-info/RECORD
-103 files, 350905 bytes uncompressed, 108288 bytes compressed:  69.1%
+-rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-11 06:28 cchenutils-0.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 06:28 cchenutils-0.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 06:28 cchenutils-0.4.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.4.1.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     9115 b- defN 23-Apr-11 06:28 cchenutils-0.4.1.dist-info/RECORD
+103 files, 351394 bytes uncompressed, 108322 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -288,23 +288,23 @@
 
 Filename: wanghong/webscraping/yizhibo/__init__.py
 Comment: 
 
 Filename: wanghong/webscraping/yizhibo/ts_downbind.py
 Comment: 
 
-Filename: cchenutils-0.0.8.dist-info/METADATA
+Filename: cchenutils-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: cchenutils-0.0.8.dist-info/WHEEL
+Filename: cchenutils-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: cchenutils-0.0.8.dist-info/top_level.txt
+Filename: cchenutils-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: cchenutils-0.0.8.dist-info/zip-safe
+Filename: cchenutils-0.4.1.dist-info/zip-safe
 Comment: 
 
-Filename: cchenutils-0.0.8.dist-info/RECORD
+Filename: cchenutils-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cchenutils/timer.py

```diff
@@ -31,57 +31,68 @@
         sleep_time = self.diff_in_seconds(_now, _next) + 1
         if log:
             print(f'\t{_now.strftime("%Y-%m-%d %H:%M:%S")}, '
                   f'executed {exec_time / 3600:.2f}h: '
                   f'restart in {sleep_time / 3600:.2f}h'
                   , flush=True)
         time.sleep(sleep_time)
+        self.start = self.now()
+        self._last = self.start
+        return self
 
     def calc_next(self, mode, offset=0):
         if mode not in (modes := ['month', 'week', 'day', 'hour', 'minute']):
             raise ValueError(f'Mode must be in {", ".join(modes)}.')
         return eval(f'self._calc_next_{mode}({offset})')
 
     def _calc_next_month(self, offset=0):
         # Offset=0: 1st day of the month
         if not 0 <= offset <= 28:
-            raise ValueError('Offset in range must in [0, 28].')
+            raise ValueError('Offset must be in range [0, 28].')
         next_start = (self.start + relativedelta(months=1)) \
             .replace(microsecond=0, second=0, minute=0, hour=0, day=offset+1)
         next_now = ((self.now()) + relativedelta(months=1)) \
             .replace(microsecond=0, second=0, minute=0, hour=0, day=offset+1)
         if next_now > next_start:
             print('Executed more than 1 month.', flush=True)
         return max([next_start, next_now])
 
     def _calc_next_week(self, offset=0):
         # Offset=0: Monday
+        if not 0 <= offset <= 6:
+            raise ValueError('Offset must be in range [0, 6].')
         next_start = (self.start + timedelta(days=(d := (7 + offset - self.start.weekday()) % 7) + 7 * (d == 0))) \
             .replace(microsecond=0, second=0, minute=0, hour=0)
         next_now = ((now := self.now()) + timedelta(days=(d := (7 + offset - now.weekday()) % 7) + 7 * (d == 0))) \
             .replace(microsecond=0, second=0, minute=0, hour=0)
         if next_now > next_start:
             print('Executed more than 1 week.', flush=True)
         return max([next_start, next_now])
 
     def _calc_next_day(self, offset=0):
+        if not 0 <= offset <= 23:
+            raise ValueError('Offset must be in range [0, 23].')
         next_start = (self.start + timedelta(days=1)).replace(microsecond=0, second=0, minute=0, hour=offset)
         next_now = (self.now() + timedelta(days=1)).replace(microsecond=0, second=0, minute=0, hour=offset)
         if next_now > next_start:
             print('Executed more than 1 day.', flush=True)
         return max([next_start, next_now])
 
     def _calc_next_hour(self, offset=0):
+        if not 0 <= offset <= 59:
+            raise ValueError('Offset must be in range [0, 59].')
         next_start = (self.start + timedelta(hours=1)).replace(microsecond=0, second=0, minute=offset)
         next_now = (self.now() + timedelta(hours=1)).replace(microsecond=0, second=0, minute=offset)
         if next_now > next_start:
             print('Executed more than 1 hour.', flush=True)
         return max([next_start, next_now])
 
     def _calc_next_minute(self, offset=0):
+        if not 0 <= offset <= 59:
+            raise ValueError('Offset must be in range [0, 59].')
         next_start = (self.start + timedelta(minutes=1)).replace(microsecond=0, second=offset)
         next_now = (self.now() + timedelta(minutes=1)).replace(microsecond=0, second=offset)
         if next_now > next_start:
             print('Executed more than 1 minute.', flush=True)
         return max([next_start, next_now])
 
     @staticmethod
```

## Comparing `cchenutils-0.0.8.dist-info/RECORD` & `cchenutils-0.4.1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cchenutils/__init__.py,sha256=NK8fpQKQxgbn5P3wN9Bxi_LPo5A68xczmzBnKKMI1n0,151
 cchenutils/dict.py,sha256=IO_6WLY3xZB8huHpwgKCbYEL3d31TllDWdhoSF8Kz6c,613
 cchenutils/gmail.py,sha256=yRuA6TxNTxYSTnMV23SFsW0I4xpCm6gMoTxe1bqFT68,1017
 cchenutils/session.py,sha256=7k67EyOxZFBhEB4Mr4sj7PS8IZeb5Whiic4de2g540c,1936
-cchenutils/timer.py,sha256=Z0GXkpMkW5RpvsEpKdncJhEs8qhnAQ0Nu6dlysoR43k,3886
+cchenutils/timer.py,sha256=kyeBOyQSoByfevSjpKVFUjU3rGswzYkjG9-hSfs0Ols,4375
 wanghong/__init__.py,sha256=nNr59H3MLTTN-oZoTCUhyOXw0282nv2lzsyom0EbEi0,150
 wanghong/async.py,sha256=5Mb-lTfhRaSYtBHcw4-PT9iV3ohu3aRNaC33okI9Pb8,1372
 wanghong/dataprep.py,sha256=8UEMnrbuPhQ8_ts_HAF9L6FQCj3Rhm3YFjIQFlI5zwY,1347
 wanghong/opts.py,sha256=T5pwfVsmma7B8OKVycfL5ddsapTpvzpNU4bOCtSccNs,784
 wanghong/test.py,sha256=jCN-cUTttNazLmN1tQb1OquGygddmwrsbZ2Gjpej4y0,1717
 wanghong/utils.py,sha256=MgPrC6cJoxon8ooopYx8BvN17GEbAW7TOTPs61RsER0,4258
 wanghong/3rdparty/__init__.py,sha256=7XnItt31RApVDO03DMqxuIVRpnNkhiBmpB8Ue5Nwm-8,152
@@ -92,12 +92,12 @@
 wanghong/video/prep/wav_split.py,sha256=UJ6iKDszpjRtpxGfE_-h_GAa_uT1dXd0ll_7zJ_2Icc,3312
 wanghong/webscraping/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/items_cover.py,sha256=xt1swF6RCnpR0eLJMsuhEkyLqw9M9GGa4BZfoPI-Egs,4548
 wanghong/webscraping/taobao/taobao_shopinfo_manual.py,sha256=wYjqTHCW4NcU8Qy8eLIi-ZpNgsXsNYeXeP7-eyMtVTw,4874
 wanghong/webscraping/yizhibo/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/yizhibo/ts_downbind.py,sha256=u-VOJl_EAsoA4Ep81XdF0GXeSc3Vr1QkmXnLDBca79o,8389
-cchenutils-0.0.8.dist-info/METADATA,sha256=Pt-YWSG-5pAYHFRZX5gbmGG8zOTUhvs-gUaBjB9R_90,196
-cchenutils-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cchenutils-0.0.8.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
-cchenutils-0.0.8.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-cchenutils-0.0.8.dist-info/RECORD,,
+cchenutils-0.4.1.dist-info/METADATA,sha256=hNTG-RLxsGDgx60oQkXxxY3IPgKhqc4ehZgHUQp8olk,196
+cchenutils-0.4.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cchenutils-0.4.1.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
+cchenutils-0.4.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+cchenutils-0.4.1.dist-info/RECORD,,
```

