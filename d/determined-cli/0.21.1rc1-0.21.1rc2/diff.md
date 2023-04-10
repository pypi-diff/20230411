# Comparing `tmp/determined_cli-0.21.1rc1-py3-none-any.whl.zip` & `tmp/determined_cli-0.21.1rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1778 bytes, number of entries: 6
--rw-r--r--  2.0 unx      226 b- defN 23-Apr-06 00:35 determined_cli/__init__.py
--rw-r--r--  2.0 unx       27 b- defN 23-Apr-06 00:35 determined_cli/__version__.py
--rw-r--r--  2.0 unx      433 b- defN 23-Apr-06 00:35 determined_cli-0.21.1rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 00:35 determined_cli-0.21.1rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-06 00:35 determined_cli-0.21.1rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      507 b- defN 23-Apr-06 00:35 determined_cli-0.21.1rc1.dist-info/RECORD
-6 files, 1300 bytes uncompressed, 846 bytes compressed:  34.9%
+Zip file size: 1780 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      226 b- defN 23-Apr-10 23:00 determined_cli/__init__.py
+-rw-r--r--  2.0 unx       27 b- defN 23-Apr-10 23:00 determined_cli/__version__.py
+-rw-r--r--  2.0 unx      433 b- defN 23-Apr-10 23:00 determined_cli-0.21.1rc2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-10 23:00 determined_cli-0.21.1rc2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-10 23:00 determined_cli-0.21.1rc2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      507 b- defN 23-Apr-10 23:00 determined_cli-0.21.1rc2.dist-info/RECORD
+6 files, 1300 bytes uncompressed, 848 bytes compressed:  34.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: determined_cli/__init__.py
 Comment: 
 
 Filename: determined_cli/__version__.py
 Comment: 
 
-Filename: determined_cli-0.21.1rc1.dist-info/METADATA
+Filename: determined_cli-0.21.1rc2.dist-info/METADATA
 Comment: 
 
-Filename: determined_cli-0.21.1rc1.dist-info/WHEEL
+Filename: determined_cli-0.21.1rc2.dist-info/WHEEL
 Comment: 
 
-Filename: determined_cli-0.21.1rc1.dist-info/top_level.txt
+Filename: determined_cli-0.21.1rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: determined_cli-0.21.1rc1.dist-info/RECORD
+Filename: determined_cli-0.21.1rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## determined_cli/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.21.1-rc1"
+__version__ = "0.21.1-rc2"
```

