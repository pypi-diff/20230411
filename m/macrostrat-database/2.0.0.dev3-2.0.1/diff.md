# Comparing `tmp/macrostrat_database-2.0.0.dev3.tar.gz` & `tmp/macrostrat_database-2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_database-2.0.0.dev3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

