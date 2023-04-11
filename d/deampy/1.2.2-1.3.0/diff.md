# Comparing `tmp/deampy-1.2.2.tar.gz` & `tmp/deampy-1.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deampy-1.2.2.tar", last modified: Tue Mar  7 14:37:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

