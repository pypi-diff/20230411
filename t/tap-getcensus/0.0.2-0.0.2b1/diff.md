# Comparing `tmp/tap_getcensus-0.0.2.tar.gz` & `tmp/tap_getcensus-0.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_getcensus-0.0.2.tar", max compression
+gzip compressed data, was "tap_getcensus-0.0.2b1.tar", max compression
```

## Comparing `tap_getcensus-0.0.2.tar` & `tap_getcensus-0.0.2b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4270 2023-04-11 06:16:20.810403 tap_getcensus-0.0.2/README.md
--rw-r--r--   0        0        0     2034 2023-04-11 06:16:40.614393 tap_getcensus-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       84 2023-04-11 06:16:20.814404 tap_getcensus-0.0.2/tap_getcensus/__init__.py
--rw-r--r--   0        0        0      116 2023-04-11 06:16:20.814404 tap_getcensus-0.0.2/tap_getcensus/__main__.py
--rw-r--r--   0        0        0     2287 2023-04-11 06:16:20.814404 tap_getcensus-0.0.2/tap_getcensus/client.py
--rw-r--r--   0        0        0    20605 2023-04-11 06:16:20.814404 tap_getcensus-0.0.2/tap_getcensus/streams.py
--rw-r--r--   0        0        0      955 2023-04-11 06:16:20.814404 tap_getcensus-0.0.2/tap_getcensus/tap.py
--rw-r--r--   0        0        0     5277 1970-01-01 00:00:00.000000 tap_getcensus-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4270 2023-04-11 06:14:09.011448 tap_getcensus-0.0.2b1/README.md
+-rw-r--r--   0        0        0     2036 2023-04-11 06:14:30.135483 tap_getcensus-0.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/__main__.py
+-rw-r--r--   0        0        0     2287 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/client.py
+-rw-r--r--   0        0        0    20605 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/streams.py
+-rw-r--r--   0        0        0      955 2023-04-11 06:14:09.015448 tap_getcensus-0.0.2b1/tap_getcensus/tap.py
+-rw-r--r--   0        0        0     5279 1970-01-01 00:00:00.000000 tap_getcensus-0.0.2b1/PKG-INFO
```

### Comparing `tap_getcensus-0.0.2/README.md` & `tap_getcensus-0.0.2b1/README.md`

 * *Files identical despite different names*

### Comparing `tap_getcensus-0.0.2/pyproject.toml` & `tap_getcensus-0.0.2b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-getcensus"
-version = "0.0.2"
+version = "0.0.2b1"
 description = "Singer tap for the Census Operational Analytics Platform, built with the Meltano SDK for Singer Taps."
 license = "Apache-2.0"
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 maintainers = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-getcensus"
 repository = "https://github.com/edgarrmondragon/tap-getcensus"
```

### Comparing `tap_getcensus-0.0.2/tap_getcensus/client.py` & `tap_getcensus-0.0.2b1/tap_getcensus/client.py`

 * *Files identical despite different names*

### Comparing `tap_getcensus-0.0.2/tap_getcensus/streams.py` & `tap_getcensus-0.0.2b1/tap_getcensus/streams.py`

 * *Files identical despite different names*

### Comparing `tap_getcensus-0.0.2/tap_getcensus/tap.py` & `tap_getcensus-0.0.2b1/tap_getcensus/tap.py`

 * *Files identical despite different names*

### Comparing `tap_getcensus-0.0.2/PKG-INFO` & `tap_getcensus-0.0.2b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-getcensus
-Version: 0.0.2
+Version: 0.0.2b1
 Summary: Singer tap for the Census Operational Analytics Platform, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-getcensus
 License: Apache-2.0
 Keywords: ELT,singer.io,Census
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tap-getcensus Version: 0.0.2 Summary: Singer tap
+Metadata-Version: 2.1 Name: tap-getcensus Version: 0.0.2b1 Summary: Singer tap
 for the Census Operational Analytics Platform, built with the Meltano SDK for
 Singer Taps. Home-page: https://github.com/edgarrmondragon/tap-getcensus
 License: Apache-2.0 Keywords: ELT,singer.io,Census Author: Edgar RamÃ­rez-
 MondragÃ³n Author-email: edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-
 MondragÃ³n Maintainer-email: edgarrm358@gmail.com Requires-Python:
 >=3.7.1,<3.12 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

