# Comparing `tmp/polyaxon-sdk-2.0.0rc5.tar.gz` & `tmp/polyaxon_sdk-2.0.0rc6-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyaxon-sdk-2.0.0rc5.tar", last modified: Tue Apr 11 15:38:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

