# Comparing `tmp/tap_jotform-0.0.5.tar.gz` & `tmp/tap_jotform-0.0.5b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_jotform-0.0.5.tar", max compression
+gzip compressed data, was "tap_jotform-0.0.5b1.tar", max compression
```

## Comparing `tap_jotform-0.0.5.tar` & `tap_jotform-0.0.5b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11355 2023-04-11 04:29:43.843201 tap_jotform-0.0.5/LICENSE
--rw-r--r--   0        0        0     3508 2023-04-11 04:29:43.843201 tap_jotform-0.0.5/README.md
--rw-r--r--   0        0        0     1836 2023-04-11 04:29:58.455351 tap_jotform-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       30 2023-04-11 04:29:43.847201 tap_jotform-0.0.5/tap_jotform/__init__.py
--rw-r--r--   0        0        0      116 2023-04-11 04:29:43.847201 tap_jotform-0.0.5/tap_jotform/__main__.py
--rw-r--r--   0        0        0     5305 2023-04-11 04:29:43.847201 tap_jotform-0.0.5/tap_jotform/client.py
--rw-r--r--   0        0        0     8419 2023-04-11 04:29:43.847201 tap_jotform-0.0.5/tap_jotform/streams.py
--rw-r--r--   0        0        0     2738 2023-04-11 04:29:43.847201 tap_jotform-0.0.5/tap_jotform/tap.py
--rw-r--r--   0        0        0     4642 1970-01-01 00:00:00.000000 tap_jotform-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11355 2023-04-11 04:26:25.288194 tap_jotform-0.0.5b1/LICENSE
+-rw-r--r--   0        0        0     3508 2023-04-11 04:26:25.288194 tap_jotform-0.0.5b1/README.md
+-rw-r--r--   0        0        0     1838 2023-04-11 04:26:46.052260 tap_jotform-0.0.5b1/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/__main__.py
+-rw-r--r--   0        0        0     5305 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/client.py
+-rw-r--r--   0        0        0     8419 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/streams.py
+-rw-r--r--   0        0        0     2738 2023-04-11 04:26:25.292194 tap_jotform-0.0.5b1/tap_jotform/tap.py
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 tap_jotform-0.0.5b1/PKG-INFO
```

### Comparing `tap_jotform-0.0.5/LICENSE` & `tap_jotform-0.0.5b1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5/README.md` & `tap_jotform-0.0.5b1/README.md`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5/pyproject.toml` & `tap_jotform-0.0.5b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.black]
 line-length = 88
 
 [tool.poetry]
 name = "tap-jotform"
-version = "0.0.5"
+version = "0.0.5b1"
 description = "Singer tap for Jotform, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-jotform"
 repository = "https://github.com/edgarrmondragon/tap-jotform"
```

### Comparing `tap_jotform-0.0.5/tap_jotform/client.py` & `tap_jotform-0.0.5b1/tap_jotform/client.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5/tap_jotform/streams.py` & `tap_jotform-0.0.5b1/tap_jotform/streams.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5/tap_jotform/tap.py` & `tap_jotform-0.0.5b1/tap_jotform/tap.py`

 * *Files identical despite different names*

### Comparing `tap_jotform-0.0.5/PKG-INFO` & `tap_jotform-0.0.5b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-jotform
-Version: 0.0.5
+Version: 0.0.5b1
 Summary: Singer tap for Jotform, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-jotform
 License: Apache-2.0
 Keywords: ELT,Jotform
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tap-jotform Version: 0.0.5 Summary: Singer tap for
-Jotform, built with the Meltano SDK for Singer Taps. Home-page: https://
+Metadata-Version: 2.1 Name: tap-jotform Version: 0.0.5b1 Summary: Singer tap
+for Jotform, built with the Meltano SDK for Singer Taps. Home-page: https://
 github.com/edgarrmondragon/tap-jotform License: Apache-2.0 Keywords:
 ELT,Jotform Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email:
 edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

