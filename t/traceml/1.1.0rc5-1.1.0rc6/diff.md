# Comparing `tmp/traceml-1.1.0rc5.tar.gz` & `tmp/traceml-1.1.0rc6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceml-1.1.0rc5.tar", last modified: Tue Apr 11 15:35:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

