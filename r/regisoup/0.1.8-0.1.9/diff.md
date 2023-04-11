# Comparing `tmp/regisoup-0.1.8.tar.gz` & `tmp/regisoup-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regisoup-0.1.8.tar", max compression
+gzip compressed data, was "regisoup-0.1.9.tar", max compression
```

## Comparing `regisoup-0.1.8.tar` & `regisoup-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      276 2023-03-31 15:45:19.984515 regisoup-0.1.8/README.md
--rw-r--r--   0        0        0      504 2023-04-11 09:18:28.469575 regisoup-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-31 15:36:16.680509 regisoup-0.1.8/regisoup/__init__.py
--rw-r--r--   0        0        0       47 2023-04-11 09:16:28.020368 regisoup-0.1.8/regisoup/__main__.py
--rw-r--r--   0        0        0    12079 2023-04-07 15:33:11.175948 regisoup-0.1.8/regisoup/main.py
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 regisoup-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2191 2023-04-11 16:00:52.190072 regisoup-0.1.9/README.md
+-rw-r--r--   0        0        0      504 2023-04-11 16:01:16.397179 regisoup-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-31 15:36:16.680509 regisoup-0.1.9/regisoup/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-11 09:16:28.020368 regisoup-0.1.9/regisoup/__main__.py
+-rw-r--r--   0        0        0    12079 2023-04-07 15:33:11.175948 regisoup-0.1.9/regisoup/main.py
+-rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 regisoup-0.1.9/PKG-INFO
```

### Comparing `regisoup-0.1.8/regisoup/main.py` & `regisoup-0.1.9/regisoup/main.py`

 * *Files identical despite different names*

