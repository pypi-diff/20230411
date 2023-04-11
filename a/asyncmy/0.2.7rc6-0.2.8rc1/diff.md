# Comparing `tmp/asyncmy-0.2.7rc6.tar.gz` & `tmp/asyncmy-0.2.8rc1-cp37-cp37m-musllinux_1_1_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncmy-0.2.7rc6.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

