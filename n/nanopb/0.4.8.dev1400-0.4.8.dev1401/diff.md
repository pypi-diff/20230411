# Comparing `tmp/nanopb-0.4.8.dev1400.tar.gz` & `tmp/nanopb-0.4.8.dev1401-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanopb-0.4.8.dev1400.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

