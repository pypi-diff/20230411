# Comparing `tmp/qnabot-0.0.2.tar.gz` & `tmp/qnabot-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qnabot-0.0.2.tar", last modified: Tue Apr 11 20:04:50 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

