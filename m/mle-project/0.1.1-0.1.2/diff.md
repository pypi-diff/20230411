# Comparing `tmp/mle_project-0.1.1.tar.gz` & `tmp/mle_project-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mle_project-0.1.1.tar", max compression
+gzip compressed data, was "mle_project-0.1.2.tar", max compression
```

## Comparing `mle_project-0.1.1.tar` & `mle_project-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      375 2023-04-11 02:50:16.443695 mle_project-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3286 2023-04-11 02:44:28.258131 mle_project-0.1.1/README.md
--rw-r--r--   0        0        0      174 2023-04-11 02:12:19.096903 mle_project-0.1.1/src/__init__.py
--rw-r--r--   0        0        0     1436 2023-04-02 00:20:37.236032 mle_project-0.1.1/src/benchmark.py
--rw-r--r--   0        0        0     3156 2023-04-11 02:12:38.253491 mle_project-0.1.1/src/simple_linear_regr.py
--rw-r--r--   0        0        0     1948 2023-04-02 00:20:37.237034 mle_project-0.1.1/src/simple_linear_regr_utils.py
--rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 mle_project-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      375 2023-04-11 02:58:25.297097 mle_project-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4779 2023-04-11 02:57:53.630739 mle_project-0.1.2/README.md
+-rw-r--r--   0        0        0      174 2023-04-11 02:12:19.096903 mle_project-0.1.2/src/__init__.py
+-rw-r--r--   0        0        0     1436 2023-04-02 00:20:37.236032 mle_project-0.1.2/src/benchmark.py
+-rw-r--r--   0        0        0     3156 2023-04-11 02:12:38.253491 mle_project-0.1.2/src/simple_linear_regr.py
+-rw-r--r--   0        0        0     1948 2023-04-02 00:20:37.237034 mle_project-0.1.2/src/simple_linear_regr_utils.py
+-rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 mle_project-0.1.2/PKG-INFO
```

### Comparing `mle_project-0.1.1/src/benchmark.py` & `mle_project-0.1.2/src/benchmark.py`

 * *Files identical despite different names*

### Comparing `mle_project-0.1.1/src/simple_linear_regr.py` & `mle_project-0.1.2/src/simple_linear_regr.py`

 * *Files identical despite different names*

### Comparing `mle_project-0.1.1/src/simple_linear_regr_utils.py` & `mle_project-0.1.2/src/simple_linear_regr_utils.py`

 * *Files identical despite different names*

