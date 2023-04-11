# Comparing `tmp/tap_shortcut-0.0.2.tar.gz` & `tmp/tap_shortcut-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shortcut-0.0.2.tar", max compression
+gzip compressed data, was "tap_shortcut-0.0.2a1.tar", max compression
```

## Comparing `tap_shortcut-0.0.2.tar` & `tap_shortcut-0.0.2a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-04-11 06:42:54.725800 tap_shortcut-0.0.2/LICENSE
--rw-r--r--   0        0        0     2571 2023-04-11 06:42:54.725800 tap_shortcut-0.0.2/README.md
--rw-r--r--   0        0        0     1628 2023-04-11 06:43:22.819530 tap_shortcut-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-11 06:42:54.725800 tap_shortcut-0.0.2/tap_shortcut/__init__.py
--rw-r--r--   0        0        0     1004 2023-04-11 06:42:54.725800 tap_shortcut-0.0.2/tap_shortcut/client.py
--rw-r--r--   0        0        0     2299 2023-04-11 06:42:54.725800 tap_shortcut-0.0.2/tap_shortcut/streams.py
--rw-r--r--   0        0        0     3640 2023-04-11 06:42:54.725800 tap_shortcut-0.0.2/tap_shortcut/tap.py
--rw-r--r--   0        0        0     3517 1970-01-01 00:00:00.000000 tap_shortcut-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 06:41:11.321362 tap_shortcut-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0     2571 2023-04-11 06:41:11.321362 tap_shortcut-0.0.2a1/README.md
+-rw-r--r--   0        0        0     1630 2023-04-11 06:41:29.625494 tap_shortcut-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/__init__.py
+-rw-r--r--   0        0        0     1004 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/client.py
+-rw-r--r--   0        0        0     2299 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/streams.py
+-rw-r--r--   0        0        0     3640 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/tap.py
+-rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 tap_shortcut-0.0.2a1/PKG-INFO
```

### Comparing `tap_shortcut-0.0.2/LICENSE` & `tap_shortcut-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.2/README.md` & `tap_shortcut-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.2/pyproject.toml` & `tap_shortcut-0.0.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-shortcut"
-version = "0.0.2"
+version = "0.0.2a1"
 description = "`tap-shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Shortcut",
 ]
```

### Comparing `tap_shortcut-0.0.2/tap_shortcut/client.py` & `tap_shortcut-0.0.2a1/tap_shortcut/client.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.2/tap_shortcut/streams.py` & `tap_shortcut-0.0.2a1/tap_shortcut/streams.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.2/tap_shortcut/tap.py` & `tap_shortcut-0.0.2a1/tap_shortcut/tap.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.2/PKG-INFO` & `tap_shortcut-0.0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-shortcut
-Version: 0.0.2
+Version: 0.0.2a1
 Summary: `tap-shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-shortcut
 License: Apache-2.0
 Keywords: ELT,singer.io,Shortcut
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: tap-shortcut Version: 0.0.2 Summary: `tap-shortcut`
-is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps. Home-
-page: https://github.com/edgarrmondragon/tap-shortcut License: Apache-2.0
-Keywords: ELT,singer.io,Shortcut Author: Edgar RamÃ­rez-MondragÃ³n Author-
-email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License
-:: OSI Approved :: Apache Software License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
-Dist: singer-sdk (==0.23.0) Requires-Dist: toolz (==0.12.0) Project-URL:
-Documentation, https://github.com/edgarrmondragon/tap-shortcut#readme Project-
-URL: Repository, https://github.com/edgarrmondragon/tap-shortcut Description-
-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: tap-shortcut Version: 0.0.2a1 Summary: `tap-
+shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer
+Taps. Home-page: https://github.com/edgarrmondragon/tap-shortcut License:
+Apache-2.0 Keywords: ELT,singer.io,Shortcut Author: Edgar RamÃ­rez-MondragÃ³n
+Author-email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: singer-sdk (==0.23.0) Requires-Dist: toolz (==0.12.0) Project-
+URL: Documentation, https://github.com/edgarrmondragon/tap-shortcut#readme
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-shortcut
+Description-Content-Type: text/markdown
                                 # tap-shortcut
                        [pre-commit.ci_status] [License]
       Singer tap for Shortcut. Built with the [Meltano Tap SDK](https://
                        sdk.meltano.com) for Singer Taps.
 ## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` ##
 Settings | Setting | Required | Default | Description | |:--------|:--------:|:
 -------:|:---------------| | token | True | None | Shortcut Token | A full list
```

