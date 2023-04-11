# Comparing `tmp/tap_shortcut-0.0.1a1.tar.gz` & `tmp/tap_shortcut-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_shortcut-0.0.1a1.tar", max compression
+gzip compressed data, was "tap_shortcut-0.0.2a1.tar", max compression
```

## Comparing `tap_shortcut-0.0.1a1.tar` & `tap_shortcut-0.0.2a1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    11357 2022-12-07 06:05:03.549923 tap_shortcut-0.0.1a1/LICENSE
--rw-r--r--   0        0        0     2571 2022-12-07 06:05:03.549923 tap_shortcut-0.0.1a1/README.md
--rw-r--r--   0        0        0     1669 2022-12-07 06:05:24.086725 tap_shortcut-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0       47 2022-12-07 06:05:03.549923 tap_shortcut-0.0.1a1/tap_shortcut/__init__.py
--rw-r--r--   0        0        0     1004 2022-12-07 06:05:03.549923 tap_shortcut-0.0.1a1/tap_shortcut/client.py
--rw-r--r--   0        0        0     2299 2022-12-07 06:05:03.549923 tap_shortcut-0.0.1a1/tap_shortcut/streams.py
--rw-r--r--   0        0        0     3335 2022-12-07 06:05:03.549923 tap_shortcut-0.0.1a1/tap_shortcut/tap.py
--rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 tap_shortcut-0.0.1a1/setup.py
--rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 tap_shortcut-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 06:41:11.321362 tap_shortcut-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0     2571 2023-04-11 06:41:11.321362 tap_shortcut-0.0.2a1/README.md
+-rw-r--r--   0        0        0     1630 2023-04-11 06:41:29.625494 tap_shortcut-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/__init__.py
+-rw-r--r--   0        0        0     1004 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/client.py
+-rw-r--r--   0        0        0     2299 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/streams.py
+-rw-r--r--   0        0        0     3640 2023-04-11 06:41:11.325362 tap_shortcut-0.0.2a1/tap_shortcut/tap.py
+-rw-r--r--   0        0        0     3519 1970-01-01 00:00:00.000000 tap_shortcut-0.0.2a1/PKG-INFO
```

### Comparing `tap_shortcut-0.0.1a1/LICENSE` & `tap_shortcut-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.1a1/README.md` & `tap_shortcut-0.0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.1a1/pyproject.toml` & `tap_shortcut-0.0.2a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-shortcut"
-version = "0.0.1a1"
+version = "0.0.2a1"
 description = "`tap-shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Shortcut",
 ]
@@ -12,21 +12,19 @@
 readme = "README.md"
 homepage = "https://github.com/edgarrmondragon/tap-shortcut"
 repository = "https://github.com/edgarrmondragon/tap-shortcut"
 documentation = "https://github.com/edgarrmondragon/tap-shortcut#readme"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.7.1"
-singer-sdk = "0.14.0"
+singer-sdk = "0.23.0"
 toolz = "0.12.0"
 
-[tool.poetry.dev-dependencies]
-mypy = ">=0.930"
-pytest = "^7.2.0"
-types-requests = "^2.28.11"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.1"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 # Vertical Hanging Indent
 src_paths = "tap_shortcut"
 
 [tool.pytest.ini_options]
```

### Comparing `tap_shortcut-0.0.1a1/tap_shortcut/client.py` & `tap_shortcut-0.0.2a1/tap_shortcut/client.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.1a1/tap_shortcut/streams.py` & `tap_shortcut-0.0.2a1/tap_shortcut/streams.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.0.1a1/tap_shortcut/tap.py` & `tap_shortcut-0.0.2a1/tap_shortcut/tap.py`

 * *Files 11% similar despite different names*

```diff
@@ -89,16 +89,25 @@
     ).to_dict()
 
     def get_openapi_schema(self) -> dict:
         """Retrieve Swagger/OpenAPI schema for this API.
 
         Returns:
             OpenAPI schema.
+
+        Raises:
+            RuntimeError: If the OpenAPI schema cannot be retrieved.
         """
-        return requests.get(OPENAPI_URL).json()
+        response = requests.get(OPENAPI_URL)
+        try:
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise RuntimeError(f"Error retrieving OpenAPI schema ({err})") from err
+
+        return response.json()
 
     def discover_streams(self) -> List[Stream]:
         """Return a list of discovered streams.
 
         Returns:
             A list of Shortcut streams.
         """
```

### Comparing `tap_shortcut-0.0.1a1/PKG-INFO` & `tap_shortcut-0.0.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tap-shortcut
-Version: 0.0.1a1
+Version: 0.0.2a1
 Summary: `tap-shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-shortcut
 License: Apache-2.0
 Keywords: ELT,singer.io,Shortcut
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (==0.14.0)
+Requires-Dist: singer-sdk (==0.23.0)
 Requires-Dist: toolz (==0.12.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-shortcut#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-shortcut
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: tap-shortcut Version: 0.0.1a1 Summary: `tap-
+Metadata-Version: 2.1 Name: tap-shortcut Version: 0.0.2a1 Summary: `tap-
 shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer
 Taps. Home-page: https://github.com/edgarrmondragon/tap-shortcut License:
 Apache-2.0 Keywords: ELT,singer.io,Shortcut Author: Edgar RamÃ­rez-MondragÃ³n
 Author-email: edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (==0.14.0) Requires-Dist: toolz (==0.12.0) Project-
+Requires-Dist: singer-sdk (==0.23.0) Requires-Dist: toolz (==0.12.0) Project-
 URL: Documentation, https://github.com/edgarrmondragon/tap-shortcut#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-shortcut
 Description-Content-Type: text/markdown
                                 # tap-shortcut
                        [pre-commit.ci_status] [License]
       Singer tap for Shortcut. Built with the [Meltano Tap SDK](https://
                        sdk.meltano.com) for Singer Taps.
```

