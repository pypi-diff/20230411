# Comparing `tmp/cchenutils-0.5.7-py3-none-any.whl.zip` & `tmp/cchenutils-0.5.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 124145 bytes, number of entries: 106
+Zip file size: 124146 bytes, number of entries: 106
 -rw-rw-rw-  2.0 fat      199 b- defN 23-Apr-11 10:14 cchenutils/__init__.py
 -rw-rw-rw-  2.0 fat      394 b- defN 23-Apr-11 21:38 cchenutils/__setup__.py
 -rw-rw-rw-  2.0 fat     1162 b- defN 23-Apr-11 07:30 cchenutils/_monitor.py
 -rw-rw-rw-  2.0 fat       84 b- defN 23-Apr-11 21:08 cchenutils/call.py
 -rw-rw-rw-  2.0 fat      613 b- defN 23-Mar-31 11:06 cchenutils/dict.py
 -rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-11 07:18 cchenutils/gmail.py
 -rw-rw-rw-  2.0 fat     2125 b- defN 23-Apr-11 20:40 cchenutils/session.py
@@ -96,13 +96,13 @@
 -rw-rw-rw-  2.0 fat     3312 b- defN 20-Mar-24 00:35 wanghong/video/prep/wav_split.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/__init__.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/taobao/__init__.py
 -rw-rw-rw-  2.0 fat     4548 b- defN 20-Apr-05 03:47 wanghong/webscraping/taobao/items_cover.py
 -rw-rw-rw-  2.0 fat     4874 b- defN 20-Mar-27 20:44 wanghong/webscraping/taobao/taobao_shopinfo_manual.py
 -rw-rw-rw-  2.0 fat      152 b- defN 20-Mar-26 19:39 wanghong/webscraping/yizhibo/__init__.py
 -rw-rw-rw-  2.0 fat     8389 b- defN 20-Mar-26 19:40 wanghong/webscraping/yizhibo/ts_downbind.py
--rw-rw-rw-  2.0 fat      195 b- defN 23-Apr-11 21:38 cchenutils-0.5.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 21:38 cchenutils-0.5.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 21:38 cchenutils-0.5.7.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-11 21:38 cchenutils-0.5.7.dist-info/zip-safe
--rw-rw-r--  2.0 fat     9346 b- defN 23-Apr-11 21:38 cchenutils-0.5.7.dist-info/RECORD
-106 files, 352315 bytes uncompressed, 109279 bytes compressed:  69.0%
+-rw-rw-rw-  2.0 fat      195 b- defN 23-Apr-11 21:38 cchenutils-0.5.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 21:38 cchenutils-0.5.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Apr-11 21:38 cchenutils-0.5.8.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-11 21:38 cchenutils-0.5.8.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     9346 b- defN 23-Apr-11 21:38 cchenutils-0.5.8.dist-info/RECORD
+106 files, 352315 bytes uncompressed, 109280 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -297,23 +297,23 @@
 
 Filename: wanghong/webscraping/yizhibo/__init__.py
 Comment: 
 
 Filename: wanghong/webscraping/yizhibo/ts_downbind.py
 Comment: 
 
-Filename: cchenutils-0.5.7.dist-info/METADATA
+Filename: cchenutils-0.5.8.dist-info/METADATA
 Comment: 
 
-Filename: cchenutils-0.5.7.dist-info/WHEEL
+Filename: cchenutils-0.5.8.dist-info/WHEEL
 Comment: 
 
-Filename: cchenutils-0.5.7.dist-info/top_level.txt
+Filename: cchenutils-0.5.8.dist-info/top_level.txt
 Comment: 
 
-Filename: cchenutils-0.5.7.dist-info/zip-safe
+Filename: cchenutils-0.5.8.dist-info/zip-safe
 Comment: 
 
-Filename: cchenutils-0.5.7.dist-info/RECORD
+Filename: cchenutils-0.5.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cchenutils/__setup__.py

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cchenutils',
-    version='0.5.7',
+    version='0.5.8',
     keywords=('utils'),
     description='cc personal use',
     license='MIT License',
     install_requires=[],
     include_package_data=True,
     zip_safe=True,
```

## Comparing `cchenutils-0.5.7.dist-info/RECORD` & `cchenutils-0.5.8.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cchenutils/__init__.py,sha256=X3gsgabX2tWQ7oE3aAtRAwh2b4sHBfbYVA7hzMAIEJ0,199
-cchenutils/__setup__.py,sha256=hULtnFi5al17lmluPtaXDKGoBMXxfnZvMMsMFZ9wnWI,394
+cchenutils/__setup__.py,sha256=yvRFJ3tYR_-SYNk72gg71E3nSBcIShxoGG7iFlk2E7U,394
 cchenutils/_monitor.py,sha256=drOt6YBZGcbb2ZqMqGEslQlZWcCJW3GeN6T-XpHJ5R0,1162
 cchenutils/call.py,sha256=1y6rVCa7EqAxB1tfTLXG1KsTP25nTBYiixlepp5WNrI,84
 cchenutils/dict.py,sha256=IO_6WLY3xZB8huHpwgKCbYEL3d31TllDWdhoSF8Kz6c,613
 cchenutils/gmail.py,sha256=5VIF9-OyzpjWbB0waR1hogtbT66ZqXwFeaCPdrIcMko,1064
 cchenutils/session.py,sha256=tSXmvmGWALiF4f1ab09x13ySSkdLfyDIwMy_brZ2EvY,2125
 cchenutils/timer.py,sha256=2GqTOG98RzpF00CaHj1FvlHnvBk42rxbcqFDB3KIahM,3142
 wanghong/__init__.py,sha256=nNr59H3MLTTN-oZoTCUhyOXw0282nv2lzsyom0EbEi0,150
@@ -95,12 +95,12 @@
 wanghong/video/prep/wav_split.py,sha256=UJ6iKDszpjRtpxGfE_-h_GAa_uT1dXd0ll_7zJ_2Icc,3312
 wanghong/webscraping/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/taobao/items_cover.py,sha256=xt1swF6RCnpR0eLJMsuhEkyLqw9M9GGa4BZfoPI-Egs,4548
 wanghong/webscraping/taobao/taobao_shopinfo_manual.py,sha256=wYjqTHCW4NcU8Qy8eLIi-ZpNgsXsNYeXeP7-eyMtVTw,4874
 wanghong/webscraping/yizhibo/__init__.py,sha256=Zx53GK5f04rgk2G04neuZcLGRhYHCNKBWtimzB1dwIQ,152
 wanghong/webscraping/yizhibo/ts_downbind.py,sha256=u-VOJl_EAsoA4Ep81XdF0GXeSc3Vr1QkmXnLDBca79o,8389
-cchenutils-0.5.7.dist-info/METADATA,sha256=UaeMsgaGo6963yrHMphUXmXnqT71ZdkFtQ6oZQPkNQk,195
-cchenutils-0.5.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cchenutils-0.5.7.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
-cchenutils-0.5.7.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-cchenutils-0.5.7.dist-info/RECORD,,
+cchenutils-0.5.8.dist-info/METADATA,sha256=eAletqa4xmvf86Cx9TKy6lsyLX7Uw7basyIWIRDu_SE,195
+cchenutils-0.5.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cchenutils-0.5.8.dist-info/top_level.txt,sha256=xLXRttimPVQEG1OBK3Vhwo65HZYG6DovfViIUG2CNRw,20
+cchenutils-0.5.8.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+cchenutils-0.5.8.dist-info/RECORD,,
```

