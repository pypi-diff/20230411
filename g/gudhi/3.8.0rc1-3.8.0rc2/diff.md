# Comparing `tmp/gudhi-3.8.0rc1.tar.gz` & `tmp/gudhi-3.8.0rc2-cp38-cp38-macosx_10_15_universal2.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\a\gudhi-devel\gudhi-devel\build\src\python\dist\tmp_t8pkuz8\gudhi-3.8.0rc1.tar", last modified: Tue Apr 11 08:46:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

