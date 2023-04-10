# Comparing `tmp/yanniszark_common-0.1.73.tar.gz` & `tmp/yanniszark_common-0.1.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanniszark_common-0.1.73.tar", max compression
+gzip compressed data, was "yanniszark_common-0.1.79.tar", max compression
```

## Comparing `yanniszark_common-0.1.73.tar` & `yanniszark_common-0.1.79.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      391 2022-12-30 13:51:03.182264 yanniszark_common-0.1.73/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-30 13:50:39.782029 yanniszark_common-0.1.73/yanniszark_common/__init__.py
--rw-r--r--   0        0        0      272 2022-12-30 13:50:39.782029 yanniszark_common-0.1.73/yanniszark_common/cmdutils.py
--rw-r--r--   0        0        0     1158 2022-12-30 13:50:39.782029 yanniszark_common-0.1.73/yanniszark_common/gitutils.py
--rw-r--r--   0        0        0      194 2022-12-30 13:50:39.782029 yanniszark_common-0.1.73/yanniszark_common/netutils.py
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 yanniszark_common-0.1.73/setup.py
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 yanniszark_common-0.1.73/PKG-INFO
+-rw-r--r--   0        0        0      391 2023-04-10 22:35:38.199517 yanniszark_common-0.1.79/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 22:35:15.071517 yanniszark_common-0.1.79/yanniszark_common/__init__.py
+-rw-r--r--   0        0        0      272 2023-04-10 22:35:15.071517 yanniszark_common-0.1.79/yanniszark_common/cmdutils.py
+-rw-r--r--   0        0        0       96 2023-04-10 22:35:15.071517 yanniszark_common-0.1.79/yanniszark_common/fileutils.py
+-rw-r--r--   0        0        0     1158 2023-04-10 22:35:15.071517 yanniszark_common-0.1.79/yanniszark_common/gitutils.py
+-rw-r--r--   0        0        0     1936 2023-04-10 22:35:15.071517 yanniszark_common-0.1.79/yanniszark_common/installutils.py
+-rw-r--r--   0        0        0      194 2023-04-10 22:35:15.071517 yanniszark_common-0.1.79/yanniszark_common/netutils.py
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 yanniszark_common-0.1.79/PKG-INFO
```

### Comparing `yanniszark_common-0.1.73/yanniszark_common/gitutils.py` & `yanniszark_common-0.1.79/yanniszark_common/gitutils.py`

 * *Files identical despite different names*

### Comparing `yanniszark_common-0.1.73/PKG-INFO` & `yanniszark_common-0.1.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanniszark-common
-Version: 0.1.73
+Version: 0.1.79
 Summary: Idiomatic, reusable code for a bunch of use-cases.
 Author: Yannis Zarkadas
 Author-email: yanniszark@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

