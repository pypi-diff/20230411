# Comparing `tmp/drill4snap-0.2.0.tar.gz` & `tmp/drill4snap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drill4snap-0.2.0.tar", max compression
+gzip compressed data, was "drill4snap-0.3.0.tar", max compression
```

## Comparing `drill4snap-0.2.0.tar` & `drill4snap-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     7651 2023-04-10 13:42:06.746487 drill4snap-0.2.0/LICENSE
--rw-r--r--   0        0        0     2997 2023-04-11 13:34:53.661106 drill4snap-0.2.0/README.md
--rw-r--r--   0        0        0       21 2023-04-10 14:07:12.271506 drill4snap-0.2.0/drill4snap/__init__.py
--rwxr-xr-x   0        0        0     1899 2023-04-11 12:20:30.196491 drill4snap-0.2.0/drill4snap/cli.py
--rw-r--r--   0        0        0      482 2023-04-11 07:51:33.373595 drill4snap-0.2.0/drill4snap/devices.py
--rw-r--r--   0        0        0     9412 2023-04-11 08:48:07.713290 drill4snap-0.2.0/drill4snap/drill_pict.png
--rw-r--r--   0        0        0      542 2023-04-11 10:16:54.449059 drill4snap-0.2.0/drill4snap/jobs.py
--rw-r--r--   0        0        0     5123 2023-04-11 10:18:45.062407 drill4snap-0.2.0/drill4snap/parser.py
--rw-r--r--   0        0        0     1171 2023-04-11 12:22:12.864748 drill4snap-0.2.0/drill4snap/templates.py
--rw-r--r--   0        0        0     6675 2023-04-11 12:16:49.446798 drill4snap-0.2.0/drill4snap/writer.py
--rw-r--r--   0        0        0      515 2023-04-11 13:35:13.141362 drill4snap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 drill4snap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     7651 2023-04-10 13:42:06.746487 drill4snap-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2997 2023-04-11 13:34:53.661106 drill4snap-0.3.0/README.md
+-rw-r--r--   0        0        0       21 2023-04-10 14:07:12.271506 drill4snap-0.3.0/drill4snap/__init__.py
+-rwxr-xr-x   0        0        0     1899 2023-04-11 12:20:30.196491 drill4snap-0.3.0/drill4snap/cli.py
+-rw-r--r--   0        0        0      482 2023-04-11 07:51:33.373595 drill4snap-0.3.0/drill4snap/devices.py
+-rw-r--r--   0        0        0     9412 2023-04-11 08:48:07.713290 drill4snap-0.3.0/drill4snap/drill_pict.png
+-rw-r--r--   0        0        0      542 2023-04-11 10:16:54.449059 drill4snap-0.3.0/drill4snap/jobs.py
+-rw-r--r--   0        0        0     5123 2023-04-11 10:18:45.062407 drill4snap-0.3.0/drill4snap/parser.py
+-rw-r--r--   0        0        0     1171 2023-04-11 12:22:12.864748 drill4snap-0.3.0/drill4snap/templates.py
+-rw-r--r--   0        0        0     6675 2023-04-11 12:16:49.446798 drill4snap-0.3.0/drill4snap/writer.py
+-rw-r--r--   0        0        0      566 2023-04-11 13:37:41.615305 drill4snap-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3639 1970-01-01 00:00:00.000000 drill4snap-0.3.0/PKG-INFO
```

### Comparing `drill4snap-0.2.0/LICENSE` & `drill4snap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drill4snap-0.2.0/README.md` & `drill4snap-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `drill4snap-0.2.0/drill4snap/cli.py` & `drill4snap-0.3.0/drill4snap/cli.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.2.0/drill4snap/drill_pict.png` & `drill4snap-0.3.0/drill4snap/drill_pict.png`

 * *Files identical despite different names*

### Comparing `drill4snap-0.2.0/drill4snap/jobs.py` & `drill4snap-0.3.0/drill4snap/jobs.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.2.0/drill4snap/parser.py` & `drill4snap-0.3.0/drill4snap/parser.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.2.0/drill4snap/templates.py` & `drill4snap-0.3.0/drill4snap/templates.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.2.0/drill4snap/writer.py` & `drill4snap-0.3.0/drill4snap/writer.py`

 * *Files identical despite different names*

### Comparing `drill4snap-0.2.0/PKG-INFO` & `drill4snap-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: drill4snap
-Version: 0.2.0
+Version: 0.3.0
 Summary: Convert Excellion drill files (such as those produced by KiCad) into G-Code for SnapMaker CNC usage
+Home-page: https://github.com/mjleehh/drill4snap
 License: LGPL
 Author: Michael Jonathan Lee
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

