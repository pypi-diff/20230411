# Comparing `tmp/cchenutils-0.4.3-py3-none-any.whl.zip` & `tmp/cchenutils-0.4.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 123463 bytes, number of entries: 104
+Zip file size: 123467 bytes, number of entries: 104
 -rw-rw-rw-  2.0 fat      199 b- defN 23-Apr-11 10:14 cchenutils/__init__.py
 -rw-rw-rw-  2.0 fat     1162 b- defN 23-Apr-11 07:30 cchenutils/_monitor.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Mar-31 11:06 cchenutils/dict.py
 -rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-11 07:18 cchenutils/gmail.py
--rw-rw-rw-  2.0 fat     1936 b- defN 23-Apr-10 09:39 cchenutils/session.py
+-rw-rw-rw-  2.0 fat     1975 b- defN 23-Apr-11 12:25 cchenutils/session.py
 -rw-rw-rw-  2.0 fat     3142 b- defN 23-Apr-11 12:12 cchenutils/timer.py
 -rw-rw-rw-  2.0 fat      150 b- defN 20-Mar-21 19:46 wanghong/__init__.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 20-Mar-24 05:56 wanghong/async.py
 -rw-rw-rw-  2.0 fat     1347 b- defN 20-Mar-23 22:38 wanghong/dataprep.py
 -rw-rw-rw-  2.0 fat      784 b- defN 20-Apr-06 03:33 wanghong/opts.py
 -rw-rw-rw-  2.0 fat     1717 b- defN 21-Mar-06 19:19 wanghong/test.py
 -rw-rw-rw-  2.0 fat     4258 b- defN 21-Mar-23 02:17 wanghong/utils.py
@@ -94,13 +94,13 @@
 -rw-rw-rw-  2.0 fat     3312 b- defN 20-Mar-24 00:35 wanghong/video/prep/wav_split.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/__init__.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/taobao/__init__.py
 -rw-rw-rw-  2.0 fat     4548 b- defN 20-Apr-05 03:47 wanghong/webscraping/taobao/items_cover.py
 -rw-rw-rw-  2.0 fat     4874 b- defN 20-Mar-27 20:44 wanghong/webscraping/taobao/taobao_shopinfo_manual.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/yizhibo/__init__.py
 -rw-rw-rw-  2.0 fat     8389 b- defN 20-Mar-26 19:40 wanghong/webscraping/yizhibo/ts_downbind.py
--rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-11 12:13 cchenutils-0.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 12:13 cchenutils-0.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 12:13 cchenutils-0.4.3.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.4.3.dist-info/zip-safe
--rw-rw-r--  2.0 fat     9194 b- defN 23-Apr-11 12:13 cchenutils-0.4.3.dist-info/RECORD
-104 files, 351497 bytes uncompressed, 108831 bytes compressed:  69.0%
+-rw-rw-rw-  2.0 fat      196 b- defN 23-Apr-11 12:26 cchenutils-0.4.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 12:26 cchenutils-0.4.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 12:26 cchenutils-0.4.4.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-31 09:42 cchenutils-0.4.4.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     9194 b- defN 23-Apr-11 12:26 cchenutils-0.4.4.dist-info/RECORD
+104 files, 351536 bytes uncompressed, 108835 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -291,23 +291,23 @@
 
 Filename: wanghong/webscraping/yizhibo/__init__.py
 Comment: 
 
 Filename: wanghong/webscraping/yizhibo/ts_downbind.py
 Comment: 
 
-Filename: cchenutils-0.4.3.dist-info/METADATA
+Filename: cchenutils-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: cchenutils-0.4.3.dist-info/WHEEL
+Filename: cchenutils-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: cchenutils-0.4.3.dist-info/top_level.txt
+Filename: cchenutils-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: cchenutils-0.4.3.dist-info/zip-safe
+Filename: cchenutils-0.4.4.dist-info/zip-safe
 Comment: 
 
-Filename: cchenutils-0.4.3.dist-info/RECORD
+Filename: cchenutils-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cchenutils/session.py

```diff
@@ -24,23 +24,24 @@
     def get(self, url, **kwargs):
         r"""Sends a GET request. Returns :class:`Response` object.
         :param url: URL for the new :class:`Request` object.
         :param \*\*kwargs: Optional arguments that ``request`` takes.
         :rtype: requests.Response
         """
         kwargs.setdefault('allow_redirects', True)
-
+        kwargs.setdefault('_retry', 0)
+        _retry = kwargs.pop('_retry')
         try:
             r = self.request("GET", url, **kwargs)
-            if r.status_code == 200 or kwargs.get('_retry') == self.max_retries:
+            if r.status_code == 200 or _retry == self.max_retries:
                 return r
         except (ProxyError, ConnectionError):
             pass
         time.sleep(self.sleep)
-        kwargs['_retry'] = kwargs.setdefault('_retry', 0) + 1
+        kwargs['_retry'] = _retry + 1
         return self.get(url, **kwargs)
 
     def get_json(self, url, **kwargs):
         return dict(self.get(url, **kwargs).json())
 
     def get_soup(self, url, **kwargs):
         return BeautifulSoup(self.get(url, **kwargs).text, features='lxml')
```

## Comparing `cchenutils-0.4.3.dist-info/RECORD` & `cchenutils-0.4.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 cchenutils/__init__.py,sha256=X3gsgabX2tWQ7oE3aAtRAwh2b4sHBfbYVA7hzMAIEJ0,199
 cchenutils/_monitor.py,sha256=drOt6YBZGcbb2ZqMqGEslQlZWcCJW3GeN6T-XpHJ5R0,1162
 cchenutils/dict.py,sha256=IO_6WLY3xZB8huHpwgKCbYEL3d31TllDWdhoSF8Kz6c,613
 cchenutils/gmail.py,sha256=5VIF9-OyzpjWbB0waR1hogtbT66ZqXwFeaCPdrIcMko,1064
-cchenutils/session.py,sha256=7k67EyOxZFBhEB4Mr4sj7PS8IZeb5Whiic4de2g540c,1936
+cchenutils/session.py,sha256=jAotIeXms4R-b--h_QsF5MsXJWC0dMMCc_6Mij6j-u8,1975
 cchenutils/timer.py,sha256=2GqTOG98RzpF00CaHj1FvlHnvBk42rxbcqFDB3KIahM,3142
 wanghong/__init__.py,sha256=nNr59H3MLTTN-oZoTCUhyOXw0282nv2lzsyom0EbEi0,150
 wanghong/async.py,sha256=5Mb-lTfhRaSYtBHcw4-PT9iV3ohu3aRNaC33okI9Pb8,1372
 wanghong/dataprep.py,sha256=8UEMnrbuPhQ8_ts_HAF9L6FQCj3Rhm3YFjIQFlI5zwY,1347
 wanghong/opts.py,sha256=T5pwfVsmma7B8OKVycfL5ddsapTpvzpNU4bOCtSccNs,784
 wanghong/test.py,sha256=jCN-cUTttNazLmN1tQb1OquGygddmwrsbZ2Gjpej4y0,1717
 wanghong/utils.py,sha256=MgPrC6cJoxon8ooopYx8BvN17GEbAW7TOTPs61RsER0,4258
@@ -93,12 +93,12 @@
 wanghong/video/prep/wav_split.py,sha256=UJ6iKDszpjRtpxGfE_-h_GAa_uT1dXd0ll_7zJ_2Icc,3312
 wanghong/webscraping/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/items_cover.py,sha256=xt1swF6RCnpR0eLJMsuhEkyLqw9M9GGa4BZfoPI-Egs,4548
 wanghong/webscraping/taobao/taobao_shopinfo_manual.py,sha256=wYjqTHCW4NcU8Qy8eLIi-ZpNgsXsNYeXeP7-eyMtVTw,4874
 wanghong/webscraping/yizhibo/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/yizhibo/ts_downbind.py,sha256=u-VOJl_EAsoA4Ep81XdF0GXeSc3Vr1QkmXnLDBca79o,8389
-cchenutils-0.4.3.dist-info/METADATA,sha256=7opiFSwEabneGCR63AZgUz3RCc-EjLxdpcnQl8VCOxE,196
-cchenutils-0.4.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cchenutils-0.4.3.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
-cchenutils-0.4.3.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-cchenutils-0.4.3.dist-info/RECORD,,
+cchenutils-0.4.4.dist-info/METADATA,sha256=vGsXqQe71yTHjnI_iDLGWvi0-IBo2fVg90NaVCPMUVw,196
+cchenutils-0.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cchenutils-0.4.4.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
+cchenutils-0.4.4.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+cchenutils-0.4.4.dist-info/RECORD,,
```

