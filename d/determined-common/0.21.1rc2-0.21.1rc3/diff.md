# Comparing `tmp/determined_common-0.21.1rc2-py3-none-any.whl.zip` & `tmp/determined_common-0.21.1rc3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1829 bytes, number of entries: 6
--rw-r--r--  2.0 unx      235 b- defN 23-Apr-10 23:00 determined_common/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-10 23:00 determined_common/__version__.py
--rw-r--r--  2.0 unx      436 b- defN 23-Apr-10 23:00 determined_common-0.21.1rc2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 23:00 determined_common-0.21.1rc2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-10 23:00 determined_common-0.21.1rc2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-10 23:00 determined_common-0.21.1rc2.dist-info/RECORD
-6 files, 1333 bytes uncompressed, 861 bytes compressed:  35.4%
+Zip file size: 1814 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      235 b- defN 23-Apr-11 20:19 determined_common/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-11 20:19 determined_common/__version__.py
+-rw-r--r--  2.0 unx      417 b- defN 23-Apr-11 20:19 determined_common-0.21.1rc3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 20:19 determined_common-0.21.1rc3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-11 20:19 determined_common-0.21.1rc3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-11 20:19 determined_common-0.21.1rc3.dist-info/RECORD
+6 files, 1314 bytes uncompressed, 846 bytes compressed:  35.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_common/__init__.py
 Comment: 
 
 Filename: determined_common/__version__.py
 Comment: 
 
-Filename: determined_common-0.21.1rc2.dist-info/METADATA
+Filename: determined_common-0.21.1rc3.dist-info/METADATA
 Comment: 
 
-Filename: determined_common-0.21.1rc2.dist-info/WHEEL
+Filename: determined_common-0.21.1rc3.dist-info/WHEEL
 Comment: 
 
-Filename: determined_common-0.21.1rc2.dist-info/top_level.txt
+Filename: determined_common-0.21.1rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_common-0.21.1rc2.dist-info/RECORD
+Filename: determined_common-0.21.1rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_common/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.21.1-rc2"
+__version__ = "0.21.1-rc3"
```

## Comparing `determined_common-0.21.1rc2.dist-info/RECORD` & `determined_common-0.21.1rc3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 determined_common/__init__.py,sha256=cHo0m87BOaQx-d4abum7tAeKV_ukSvs3xkABM7R76OM,235
-determined_common/__version__.py,sha256=6k1kbFOzHQh-YsABJPzuwCFtWRZtqnNyEhDfropiWqY,27
-determined_common-0.21.1rc2.dist-info/METADATA,sha256=MUUTTGl1EJGObXl2zqI8olIEywTYIpfDml57a_lFreE,436
-determined_common-0.21.1rc2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-determined_common-0.21.1rc2.dist-info/top_level.txt,sha256=CD1pq4FvMD2KEVXd1cFj6S6gCC-Th-FtDLBZojRsg98,18
-determined_common-0.21.1rc2.dist-info/RECORD,,
+determined_common/__version__.py,sha256=o3Mw2i5FQl98c8cXwSrVM2sHvV_sTby7-HJzRNNnxGc,27
+determined_common-0.21.1rc3.dist-info/METADATA,sha256=4i52n-_YgQE31VIvPp9F7Tcf51yaz_yQrABTWnc0MjI,417
+determined_common-0.21.1rc3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+determined_common-0.21.1rc3.dist-info/top_level.txt,sha256=CD1pq4FvMD2KEVXd1cFj6S6gCC-Th-FtDLBZojRsg98,18
+determined_common-0.21.1rc3.dist-info/RECORD,,
```

