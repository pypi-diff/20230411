# Comparing `tmp/tvault-0.3.1-py3-none-any.whl.zip` & `tmp/tvault-0.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 9981 bytes, number of entries: 11
--rw-r--r--  2.0 unx     2815 b- defN 23-Apr-11 07:59 tvault/__init__.py
+-rw-r--r--  2.0 unx     2813 b- defN 23-Apr-11 08:19 tvault/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-03 04:19 tvault/model_diff.py
 -rw-r--r--  2.0 unx     4789 b- defN 23-Apr-03 06:15 tvault/model_log.py
 -rw-r--r--  2.0 unx     8071 b- defN 23-Apr-11 08:17 tvault/parse_utils.py
 -rw-r--r--  2.0 unx    12900 b- defN 23-Apr-11 08:01 tvault/torchvault.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Apr-11 08:18 tvault-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-11 08:18 tvault-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 08:18 tvault-0.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Apr-11 08:18 tvault-0.3.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-11 08:18 tvault-0.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-11 08:18 tvault-0.3.1.dist-info/RECORD
-11 files, 31028 bytes uncompressed, 8541 bytes compressed:  72.5%
+-rw-r--r--  2.0 unx     1067 b- defN 23-Apr-11 08:19 tvault-0.3.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      380 b- defN 23-Apr-11 08:19 tvault-0.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 08:19 tvault-0.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-11 08:19 tvault-0.3.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-11 08:19 tvault-0.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      854 b- defN 23-Apr-11 08:19 tvault-0.3.2.dist-info/RECORD
+11 files, 31026 bytes uncompressed, 8541 bytes compressed:  72.5%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: tvault/parse_utils.py
 Comment: 
 
 Filename: tvault/torchvault.py
 Comment: 
 
-Filename: tvault-0.3.1.dist-info/LICENSE
+Filename: tvault-0.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: tvault-0.3.1.dist-info/METADATA
+Filename: tvault-0.3.2.dist-info/METADATA
 Comment: 
 
-Filename: tvault-0.3.1.dist-info/WHEEL
+Filename: tvault-0.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: tvault-0.3.1.dist-info/entry_points.txt
+Filename: tvault-0.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: tvault-0.3.1.dist-info/top_level.txt
+Filename: tvault-0.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tvault-0.3.1.dist-info/RECORD
+Filename: tvault-0.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tvault/__init__.py

```diff
@@ -73,17 +73,17 @@
 @click.option("--condition", type=str, default="hash")
 @click.option("--hash", type=str, default="")
 @click.option("--tag", type=str, default="")
 @click.option("--min", type=int, default=0)
 @click.option("--max", type=int, default=100)
 # options for diff
 @click.option("--sha1", type=str, default="")
-@click.option("--index1", type=int, default="")
+@click.option("--index1", type=int, default=0)
 @click.option("--sha2", type=str, default="")
-@click.option("--index2", type=int, default="")
+@click.option("--index2", type=int, default=0)
 def cli_main(
     find_flag,
     diff_flag,
     log_dir,
     model_dir,
     condition,
     hash,
```

## Comparing `tvault-0.3.1.dist-info/LICENSE` & `tvault-0.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

