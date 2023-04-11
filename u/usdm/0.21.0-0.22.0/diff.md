# Comparing `tmp/usdm-0.21.0.tar.gz` & `tmp/usdm-0.22.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usdm-0.21.0.tar", last modified: Wed Apr  5 16:56:37 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

