# Comparing `tmp/pynurex-1.5-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/pynurex-1.9.0-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,11 @@
-Zip file size: 806749 bytes, number of entries: 5
--rwxr-xr-x  2.0 unx  2923088 b- defN 22-Oct-11 11:00 pynurex.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      148 b- defN 22-Oct-11 11:03 pynurex-1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 22-Oct-11 11:00 pynurex-1.5.dist-info/top_level.txt
--rw-r--r--  2.0 unx     1807 b- defN 22-Oct-11 11:00 pynurex-1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx      393 b- defN 22-Oct-11 11:03 pynurex-1.5.dist-info/RECORD
-5 files, 2925444 bytes uncompressed, 806031 bytes compressed:  72.5%
+Zip file size: 717903 bytes, number of entries: 9
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 20:54 pynurex.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 20:54 pynurex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 20:54 pynurex-1.9.0.dist-info/
+-rwxr-xr-x  2.0 unx  2253064 b- defN 23-Apr-10 20:54 pynurex/_pynurex.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx       24 b- defN 23-Apr-10 20:54 pynurex/__init__.py
+-rw-rw-r--  2.0 unx      155 b- defN 23-Apr-10 20:54 pynurex-1.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-10 20:54 pynurex-1.9.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx      488 b- defN 23-Apr-10 20:54 pynurex-1.9.0.dist-info/RECORD
+-rw-rw-r--  2.0 unx      173 b- defN 23-Apr-10 20:54 pynurex-1.9.0.dist-info/METADATA
+9 files, 2253904 bytes uncompressed, 716711 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -1,16 +1,28 @@
-Filename: pynurex.cpython-39-x86_64-linux-gnu.so
+Filename: pynurex.libs/
 Comment: 
 
-Filename: pynurex-1.5.dist-info/WHEEL
+Filename: pynurex/
 Comment: 
 
-Filename: pynurex-1.5.dist-info/top_level.txt
+Filename: pynurex-1.9.0.dist-info/
 Comment: 
 
-Filename: pynurex-1.5.dist-info/METADATA
+Filename: pynurex/_pynurex.cpython-311-x86_64-linux-gnu.so
 Comment: 
 
-Filename: pynurex-1.5.dist-info/RECORD
+Filename: pynurex/__init__.py
+Comment: 
+
+Filename: pynurex-1.9.0.dist-info/WHEEL
+Comment: 
+
+Filename: pynurex-1.9.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: pynurex-1.9.0.dist-info/RECORD
+Comment: 
+
+Filename: pynurex-1.9.0.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

