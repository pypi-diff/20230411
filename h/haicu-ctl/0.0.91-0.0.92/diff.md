# Comparing `tmp/haicu-ctl-0.0.91.tar.gz` & `tmp/haicu_ctl-0.0.92-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-ctl-0.0.91.tar", last modified: Tue Apr 11 17:58:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

