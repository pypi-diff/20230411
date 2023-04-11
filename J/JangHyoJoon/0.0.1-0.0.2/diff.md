# Comparing `tmp/JangHyoJoon-0.0.1-py3-none-any.whl.zip` & `tmp/JangHyoJoon-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1308 bytes, number of entries: 5
--rw-r--r--  2.0 unx       62 b- defN 23-Apr-11 01:54 mycalc/calculator.py
--rw-r--r--  2.0 unx      235 b- defN 23-Apr-11 02:14 JangHyoJoon-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 02:14 JangHyoJoon-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-11 02:14 JangHyoJoon-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      387 b- defN 23-Apr-11 02:14 JangHyoJoon-0.0.1.dist-info/RECORD
-5 files, 783 bytes uncompressed, 578 bytes compressed:  26.2%
+Zip file size: 1307 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       64 b- defN 23-Apr-11 02:26 mycalc/calculator.py
+-rw-r--r--  2.0 unx      235 b- defN 23-Apr-11 02:27 JangHyoJoon-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 02:27 JangHyoJoon-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-11 02:27 JangHyoJoon-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      387 b- defN 23-Apr-11 02:27 JangHyoJoon-0.0.2.dist-info/RECORD
+5 files, 785 bytes uncompressed, 577 bytes compressed:  26.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: mycalc/calculator.py
 Comment: 
 
-Filename: JangHyoJoon-0.0.1.dist-info/METADATA
+Filename: JangHyoJoon-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: JangHyoJoon-0.0.1.dist-info/WHEEL
+Filename: JangHyoJoon-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: JangHyoJoon-0.0.1.dist-info/top_level.txt
+Filename: JangHyoJoon-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: JangHyoJoon-0.0.1.dist-info/RECORD
+Filename: JangHyoJoon-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mycalc/calculator.py

```diff
@@ -1,6 +1,7 @@
 def add(a,b):
   return a+b
 
+
 def sub(a,b):
   return a-b
```

