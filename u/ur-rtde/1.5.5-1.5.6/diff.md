# Comparing `tmp/ur_rtde-1.5.5.tar.gz` & `tmp/ur_rtde-1.5.6-pp37-pypy37_pp73-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ur_rtde-1.5.5.tar", last modified: Mon Oct 31 10:53:00 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

