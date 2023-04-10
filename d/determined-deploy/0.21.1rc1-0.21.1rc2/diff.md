# Comparing `tmp/determined_deploy-0.21.1rc1-py3-none-any.whl.zip` & `tmp/determined_deploy-0.21.1rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 1828 bytes, number of entries: 6
--rw-r--r--  2.0 unx      235 b- defN 23-Apr-06 00:35 determined_deploy/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-06 00:35 determined_deploy/__version__.py
--rw-r--r--  2.0 unx      436 b- defN 23-Apr-06 00:35 determined_deploy-0.21.1rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 00:35 determined_deploy-0.21.1rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Apr-06 00:35 determined_deploy-0.21.1rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-06 00:35 determined_deploy-0.21.1rc1.dist-info/RECORD
+-rw-r--r--  2.0 unx      235 b- defN 23-Apr-10 23:00 determined_deploy/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-10 23:00 determined_deploy/__version__.py
+-rw-r--r--  2.0 unx      436 b- defN 23-Apr-10 23:00 determined_deploy-0.21.1rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 23:00 determined_deploy-0.21.1rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Apr-10 23:00 determined_deploy-0.21.1rc2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 23-Apr-10 23:00 determined_deploy-0.21.1rc2.dist-info/RECORD
 6 files, 1333 bytes uncompressed, 860 bytes compressed:  35.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_deploy/__init__.py
 Comment: 
 
 Filename: determined_deploy/__version__.py
 Comment: 
 
-Filename: determined_deploy-0.21.1rc1.dist-info/METADATA
+Filename: determined_deploy-0.21.1rc2.dist-info/METADATA
 Comment: 
 
-Filename: determined_deploy-0.21.1rc1.dist-info/WHEEL
+Filename: determined_deploy-0.21.1rc2.dist-info/WHEEL
 Comment: 
 
-Filename: determined_deploy-0.21.1rc1.dist-info/top_level.txt
+Filename: determined_deploy-0.21.1rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_deploy-0.21.1rc1.dist-info/RECORD
+Filename: determined_deploy-0.21.1rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_deploy/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.21.1-rc1"
+__version__ = "0.21.1-rc2"
```

## Comparing `determined_deploy-0.21.1rc1.dist-info/RECORD` & `determined_deploy-0.21.1rc2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 determined_deploy/__init__.py,sha256=e4caLmyNqYzmNjIyNmPBCVCCmZ0BPYY6K_M279HBLeA,235
-determined_deploy/__version__.py,sha256=fGFT1F6PXRbRLKGS6Fc3BOZRJoBH71oa7dWe_k7S2RE,27
-determined_deploy-0.21.1rc1.dist-info/METADATA,sha256=wmJt-UTWOiVhnb01kqvT5mc4VI8yUPc87a1X3riXXZo,436
-determined_deploy-0.21.1rc1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-determined_deploy-0.21.1rc1.dist-info/top_level.txt,sha256=cP5FE7UPh3f1fj49mbwhot5Rs5UcGIZpFFy-tZeaPhg,18
-determined_deploy-0.21.1rc1.dist-info/RECORD,,
+determined_deploy/__version__.py,sha256=6k1kbFOzHQh-YsABJPzuwCFtWRZtqnNyEhDfropiWqY,27
+determined_deploy-0.21.1rc2.dist-info/METADATA,sha256=uvdnn5HolPdgt5kAiXH5OkhLtpbLPuZBff4sHba8FAg,436
+determined_deploy-0.21.1rc2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+determined_deploy-0.21.1rc2.dist-info/top_level.txt,sha256=cP5FE7UPh3f1fj49mbwhot5Rs5UcGIZpFFy-tZeaPhg,18
+determined_deploy-0.21.1rc2.dist-info/RECORD,,
```

