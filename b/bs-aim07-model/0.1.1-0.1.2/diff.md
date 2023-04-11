# Comparing `tmp/bs_aim07_model-0.1.1-py3-none-any.whl.zip` & `tmp/bs_aim07_model-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 4570 bytes, number of entries: 7
+Zip file size: 5386 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       28 b- defN 23-Apr-08 08:55 bs_aim07_model/__init__.py
 -rw-rw-r--  2.0 unx    10593 b- defN 23-Apr-08 08:55 bs_aim07_model/model.py
 -rw-rw-r--  2.0 unx     3648 b- defN 23-Apr-07 16:50 bs_aim07_model/resnet.py
--rw-rw-r--  2.0 unx       59 b- defN 23-Apr-08 09:00 bs_aim07_model-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-08 09:00 bs_aim07_model-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-08 09:00 bs_aim07_model-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      567 b- defN 23-Apr-08 09:00 bs_aim07_model-0.1.1.dist-info/RECORD
-7 files, 15002 bytes uncompressed, 3558 bytes compressed:  76.3%
+-rw-rw-r--  2.0 unx     1900 b- defN 23-Apr-11 06:13 bs_aim07_model/yunet.py
+-rw-rw-r--  2.0 unx       59 b- defN 23-Apr-11 06:21 bs_aim07_model-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-11 06:21 bs_aim07_model-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-11 06:21 bs_aim07_model-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      647 b- defN 23-Apr-11 06:21 bs_aim07_model-0.1.2.dist-info/RECORD
+8 files, 16982 bytes uncompressed, 4252 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -3,20 +3,23 @@
 
 Filename: bs_aim07_model/model.py
 Comment: 
 
 Filename: bs_aim07_model/resnet.py
 Comment: 
 
-Filename: bs_aim07_model-0.1.1.dist-info/METADATA
+Filename: bs_aim07_model/yunet.py
 Comment: 
 
-Filename: bs_aim07_model-0.1.1.dist-info/WHEEL
+Filename: bs_aim07_model-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: bs_aim07_model-0.1.1.dist-info/top_level.txt
+Filename: bs_aim07_model-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: bs_aim07_model-0.1.1.dist-info/RECORD
+Filename: bs_aim07_model-0.1.2.dist-info/top_level.txt
+Comment: 
+
+Filename: bs_aim07_model-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bs_aim07_model-0.1.1.dist-info/RECORD` & `bs_aim07_model-0.1.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 bs_aim07_model/__init__.py,sha256=F0OgTfDoMF87X3lfq-IWSWUhHnvTuxrbh6G7YW5BWWs,28
 bs_aim07_model/model.py,sha256=vh8bmggcqDa1xj96tHQ4uIM11iptQOCj6XytCVpimgo,10593
 bs_aim07_model/resnet.py,sha256=PDOyEqKM3P8bPxq0qp9ZJHvxfmuma9xQYFbyv4kwrZU,3648
-bs_aim07_model-0.1.1.dist-info/METADATA,sha256=noRMTfn9h5SCov0PREH3EOojRwVcbRTS_zy6OCu63pY,59
-bs_aim07_model-0.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bs_aim07_model-0.1.1.dist-info/top_level.txt,sha256=37YAu3o1pG90uuHaGHn3Qs6ye-0zTPGCDbEkFkqiLyM,15
-bs_aim07_model-0.1.1.dist-info/RECORD,,
+bs_aim07_model/yunet.py,sha256=-wyemaarG5qSFCO95HdTPjhZ1DWlKBGgStygx7V8mAc,1900
+bs_aim07_model-0.1.2.dist-info/METADATA,sha256=xQYZkNrP92S-KLt91oinnArnXdKBCY8baMNsWtUybcA,59
+bs_aim07_model-0.1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bs_aim07_model-0.1.2.dist-info/top_level.txt,sha256=37YAu3o1pG90uuHaGHn3Qs6ye-0zTPGCDbEkFkqiLyM,15
+bs_aim07_model-0.1.2.dist-info/RECORD,,
```

