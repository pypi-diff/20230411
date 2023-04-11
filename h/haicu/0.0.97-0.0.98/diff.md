# Comparing `tmp/haicu-0.0.97-py3-none-any.whl.zip` & `tmp/haicu-0.0.98-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 14442 bytes, number of entries: 10
+Zip file size: 14441 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 23-Mar-10 00:08 haicu/__init__.py
 -rw-rw-r--  2.0 unx    28700 b- defN 23-Apr-11 18:22 haicu/__main__.py
 -rw-rw-r--  2.0 unx    12563 b- defN 23-Apr-11 18:21 haicu/format.py
 -rw-rw-r--  2.0 unx    11443 b- defN 23-Apr-11 18:13 haicu/ftdi.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-Apr-11 18:46 haicu-0.0.97.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2671 b- defN 23-Apr-11 18:46 haicu-0.0.97.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-11 18:46 haicu-0.0.97.dist-info/WHEEL
--rw-rw-r--  2.0 unx       50 b- defN 23-Apr-11 18:46 haicu-0.0.97.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-11 18:46 haicu-0.0.97.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      764 b- defN 23-Apr-11 18:46 haicu-0.0.97.dist-info/RECORD
-10 files, 57363 bytes uncompressed, 13150 bytes compressed:  77.1%
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Apr-11 18:48 haicu-0.0.98.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2671 b- defN 23-Apr-11 18:48 haicu-0.0.98.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-11 18:48 haicu-0.0.98.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       50 b- defN 23-Apr-11 18:48 haicu-0.0.98.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 23-Apr-11 18:48 haicu-0.0.98.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      764 b- defN 23-Apr-11 18:48 haicu-0.0.98.dist-info/RECORD
+10 files, 57363 bytes uncompressed, 13149 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: haicu/format.py
 Comment: 
 
 Filename: haicu/ftdi.py
 Comment: 
 
-Filename: haicu-0.0.97.dist-info/LICENSE
+Filename: haicu-0.0.98.dist-info/LICENSE
 Comment: 
 
-Filename: haicu-0.0.97.dist-info/METADATA
+Filename: haicu-0.0.98.dist-info/METADATA
 Comment: 
 
-Filename: haicu-0.0.97.dist-info/WHEEL
+Filename: haicu-0.0.98.dist-info/WHEEL
 Comment: 
 
-Filename: haicu-0.0.97.dist-info/entry_points.txt
+Filename: haicu-0.0.98.dist-info/entry_points.txt
 Comment: 
 
-Filename: haicu-0.0.97.dist-info/top_level.txt
+Filename: haicu-0.0.98.dist-info/top_level.txt
 Comment: 
 
-Filename: haicu-0.0.97.dist-info/RECORD
+Filename: haicu-0.0.98.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `haicu-0.0.97.dist-info/LICENSE` & `haicu-0.0.98.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `haicu-0.0.97.dist-info/METADATA` & `haicu-0.0.98.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.0.97
+Version: 0.0.98
 Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

## Comparing `haicu-0.0.97.dist-info/RECORD` & `haicu-0.0.98.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 haicu/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 haicu/__main__.py,sha256=r9nnlKy_P3P8BoifkikrF1pYUlqCXGzyf27pzJV-jic,28700
 haicu/format.py,sha256=rDwfs72UgS4UipXAp2CsuXlbc8-TIGCw9UXgYKezBjA,12563
 haicu/ftdi.py,sha256=qzZ4AM_NPEBLsrddj57PIgbyn3Z-LhzoRUFGP7iqt4k,11443
-haicu-0.0.97.dist-info/LICENSE,sha256=UxFRHj5WAGUbemGOIhM09tTcnlIXiimQNWtKfb48Auc,1074
-haicu-0.0.97.dist-info/METADATA,sha256=GTOAEeYD1AMhhYMHWR6IeLbTxrNhJUp63TDN2ITCErU,2671
-haicu-0.0.97.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-haicu-0.0.97.dist-info/entry_points.txt,sha256=tvtNJy9RNPTw-BbSnx2KNdG02H6hTimcSC8FnNNLhuY,50
-haicu-0.0.97.dist-info/top_level.txt,sha256=MwlA-feLYqzkHMDPDxcNkrLPFhFYsB-0rip383poUwU,6
-haicu-0.0.97.dist-info/RECORD,,
+haicu-0.0.98.dist-info/LICENSE,sha256=UxFRHj5WAGUbemGOIhM09tTcnlIXiimQNWtKfb48Auc,1074
+haicu-0.0.98.dist-info/METADATA,sha256=IfLhRCZcb9KkYInhP7lk7j4y1XalM1EyPhoXPGp1G4I,2671
+haicu-0.0.98.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+haicu-0.0.98.dist-info/entry_points.txt,sha256=tvtNJy9RNPTw-BbSnx2KNdG02H6hTimcSC8FnNNLhuY,50
+haicu-0.0.98.dist-info/top_level.txt,sha256=MwlA-feLYqzkHMDPDxcNkrLPFhFYsB-0rip383poUwU,6
+haicu-0.0.98.dist-info/RECORD,,
```

