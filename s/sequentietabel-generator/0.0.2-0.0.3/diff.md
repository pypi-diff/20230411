# Comparing `tmp/sequentietabel_generator-0.0.2.tar.gz` & `tmp/sequentietabel_generator-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequentietabel_generator-0.0.2.tar", last modified: Fri Apr  7 21:30:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

