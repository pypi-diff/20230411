# Comparing `tmp/tap_checkly-0.0.2.tar.gz` & `tmp/tap_checkly-0.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_checkly-0.0.2.tar", max compression
+gzip compressed data, was "tap_checkly-0.0.2b1.tar", max compression
```

## Comparing `tap_checkly-0.0.2.tar` & `tap_checkly-0.0.2b1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-04-11 04:37:27.373915 tap_checkly-0.0.2/LICENSE
--rw-r--r--   0        0        0     4559 2023-04-11 04:37:27.373915 tap_checkly-0.0.2/README.md
--rw-r--r--   0        0        0     2107 2023-04-11 04:38:17.343774 tap_checkly-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       82 2023-04-11 04:37:27.373915 tap_checkly-0.0.2/tap_checkly/__init__.py
--rw-r--r--   0        0        0      116 2023-04-11 04:37:27.373915 tap_checkly-0.0.2/tap_checkly/__main__.py
--rw-r--r--   0        0        0     4867 2023-04-11 04:37:27.373915 tap_checkly-0.0.2/tap_checkly/client.py
--rw-r--r--   0        0        0   313417 2023-04-11 04:37:27.373915 tap_checkly-0.0.2/tap_checkly/openapi.json
--rw-r--r--   0        0        0     3263 2023-04-11 04:37:27.373915 tap_checkly-0.0.2/tap_checkly/streams.py
--rw-r--r--   0        0        0     1869 2023-04-11 04:37:27.373915 tap_checkly-0.0.2/tap_checkly/tap.py
--rw-r--r--   0        0        0     5529 1970-01-01 00:00:00.000000 tap_checkly-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 04:33:17.971831 tap_checkly-0.0.2b1/LICENSE
+-rw-r--r--   0        0        0     4559 2023-04-11 04:33:17.971831 tap_checkly-0.0.2b1/README.md
+-rw-r--r--   0        0        0     2109 2023-04-11 04:33:35.056054 tap_checkly-0.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-04-11 04:33:17.975831 tap_checkly-0.0.2b1/tap_checkly/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-11 04:33:17.975831 tap_checkly-0.0.2b1/tap_checkly/__main__.py
+-rw-r--r--   0        0        0     4867 2023-04-11 04:33:17.975831 tap_checkly-0.0.2b1/tap_checkly/client.py
+-rw-r--r--   0        0        0   313417 2023-04-11 04:33:17.975831 tap_checkly-0.0.2b1/tap_checkly/openapi.json
+-rw-r--r--   0        0        0     3263 2023-04-11 04:33:17.975831 tap_checkly-0.0.2b1/tap_checkly/streams.py
+-rw-r--r--   0        0        0     1869 2023-04-11 04:33:17.975831 tap_checkly-0.0.2b1/tap_checkly/tap.py
+-rw-r--r--   0        0        0     5531 1970-01-01 00:00:00.000000 tap_checkly-0.0.2b1/PKG-INFO
```

### Comparing `tap_checkly-0.0.2/LICENSE` & `tap_checkly-0.0.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.2/README.md` & `tap_checkly-0.0.2b1/README.md`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.2/pyproject.toml` & `tap_checkly-0.0.2b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-checkly"
-version = "0.0.2"
+version = "0.0.2b1"
 description = "Singer tap for Checkly, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-checkly"
 repository = "https://github.com/edgarrmondragon/tap-checkly"
```

### Comparing `tap_checkly-0.0.2/tap_checkly/client.py` & `tap_checkly-0.0.2b1/tap_checkly/client.py`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.2/tap_checkly/openapi.json` & `tap_checkly-0.0.2b1/tap_checkly/openapi.json`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.2/tap_checkly/streams.py` & `tap_checkly-0.0.2b1/tap_checkly/streams.py`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.2/tap_checkly/tap.py` & `tap_checkly-0.0.2b1/tap_checkly/tap.py`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.2/PKG-INFO` & `tap_checkly-0.0.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-checkly
-Version: 0.0.2
+Version: 0.0.2b1
 Summary: Singer tap for Checkly, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-checkly
 License: Apache-2.0
 Keywords: ELT,singer.io,Checkly
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: tap-checkly Version: 0.0.2 Summary: Singer tap for
-Checkly, built with the Meltano SDK for Singer Taps. Home-page: https://
+Metadata-Version: 2.1 Name: tap-checkly Version: 0.0.2b1 Summary: Singer tap
+for Checkly, built with the Meltano SDK for Singer Taps. Home-page: https://
 github.com/edgarrmondragon/tap-checkly License: Apache-2.0 Keywords:
 ELT,singer.io,Checkly Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email:
 edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

