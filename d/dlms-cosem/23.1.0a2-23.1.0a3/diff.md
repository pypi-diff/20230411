# Comparing `tmp/dlms-cosem-23.1.0a2.tar.gz` & `tmp/dlms_cosem-23.1.0a3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlms-cosem-23.1.0a2.tar", last modified: Mon Mar  6 14:34:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

