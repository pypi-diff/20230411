# Comparing `tmp/web3toolz-0.7.tar.gz` & `tmp/web3toolz-0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\web3toolz-0.7.tar", last modified: Fri Apr  7 03:57:28 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

