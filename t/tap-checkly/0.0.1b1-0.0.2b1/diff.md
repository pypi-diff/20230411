# Comparing `tmp/tap_checkly-0.0.1b1.tar.gz` & `tmp/tap_checkly-0.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_checkly-0.0.1b1.tar", max compression
+gzip compressed data, was "tap_checkly-0.0.2b1.tar", max compression
```

## Comparing `tap_checkly-0.0.1b1.tar` & `tap_checkly-0.0.2b1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11357 2022-12-08 04:21:19.977781 tap_checkly-0.0.1b1/LICENSE
--rw-r--r--   0        0        0     4559 2022-12-08 04:21:19.977781 tap_checkly-0.0.1b1/README.md
--rw-r--r--   0        0        0     3071 2022-12-08 04:21:37.526200 tap_checkly-0.0.1b1/pyproject.toml
--rw-r--r--   0        0        0       82 2022-12-08 04:21:19.977781 tap_checkly-0.0.1b1/tap_checkly/__init__.py
--rw-r--r--   0        0        0      116 2022-12-08 04:21:19.977781 tap_checkly-0.0.1b1/tap_checkly/__main__.py
--rw-r--r--   0        0        0     4855 2022-12-08 04:21:19.977781 tap_checkly-0.0.1b1/tap_checkly/client.py
--rw-r--r--   0        0        0   313417 2022-12-08 04:21:19.977781 tap_checkly-0.0.1b1/tap_checkly/openapi.json
--rw-r--r--   0        0        0     3263 2022-12-08 04:21:19.977781 tap_checkly-0.0.1b1/tap_checkly/streams.py
--rw-r--r--   0        0        0     1869 2022-12-08 04:21:19.977781 tap_checkly-0.0.1b1/tap_checkly/tap.py
--rw-r--r--   0        0        0     5597 1970-01-01 00:00:00.000000 tap_checkly-0.0.1b1/setup.py
--rw-r--r--   0        0        0     5554 1970-01-01 00:00:00.000000 tap_checkly-0.0.1b1/PKG-INFO
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

### Comparing `tap_checkly-0.0.1b1/LICENSE` & `tap_checkly-0.0.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.1b1/README.md` & `tap_checkly-0.0.2b1/README.md`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.1b1/tap_checkly/client.py` & `tap_checkly-0.0.2b1/tap_checkly/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             True if response contains at least one item.
         """
         try:
             first(
                 extract_jsonpath(
                     self.records_jsonpath,
                     response.json(),
-                )
+                ),
             )
         except StopIteration:
             return False
 
         return True
 
 
@@ -127,16 +127,16 @@
     def _resolve_openapi_ref(self) -> dict[str, Any]:
         schema = {"$ref": f"#/components/schemas/{self.openapi_ref}"}
         openapi = load_openapi()
         schema["components"] = openapi["components"]
         return resolve_schema_references(schema)
 
     @property
-    @lru_cache(maxsize=None)  # type: ignore # noqa: B019
-    def schema(self) -> dict[str, Any]:
+    @lru_cache(maxsize=None)  # noqa: B019
+    def schema(self) -> dict[str, Any]:  # type: ignore[override]
         """Return the schema for this stream.
 
         Returns:
             The schema for this stream.
         """
         return self._resolve_openapi_ref()
```

### Comparing `tap_checkly-0.0.1b1/tap_checkly/openapi.json` & `tap_checkly-0.0.2b1/tap_checkly/openapi.json`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.1b1/tap_checkly/streams.py` & `tap_checkly-0.0.2b1/tap_checkly/streams.py`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.1b1/tap_checkly/tap.py` & `tap_checkly-0.0.2b1/tap_checkly/tap.py`

 * *Files identical despite different names*

### Comparing `tap_checkly-0.0.1b1/PKG-INFO` & `tap_checkly-0.0.2b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: tap-checkly
-Version: 0.0.1b1
-Summary: `tap-checkly` is a Singer tap for Checkly, built with the Meltano SDK for Singer Taps.
+Version: 0.0.2b1
+Summary: Singer tap for Checkly, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-checkly
 License: Apache-2.0
 Keywords: ELT,singer.io,Checkly
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Maintainer: Edgar Ramírez-Mondragón
 Maintainer-email: edgarrm358@gmail.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: singer-sdk (>=0.14.0,<0.15.0)
+Requires-Dist: singer-sdk (>=0.14,<0.24)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-checkly/#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-checkly
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 # tap-checkly
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: tap-checkly Version: 0.0.1b1 Summary: `tap-checkly`
-is a Singer tap for Checkly, built with the Meltano SDK for Singer Taps. Home-
-page: https://github.com/edgarrmondragon/tap-checkly License: Apache-2.0
-Keywords: ELT,singer.io,Checkly Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
+Metadata-Version: 2.1 Name: tap-checkly Version: 0.0.2b1 Summary: Singer tap
+for Checkly, built with the Meltano SDK for Singer Taps. Home-page: https://
+github.com/edgarrmondragon/tap-checkly License: Apache-2.0 Keywords:
+ELT,singer.io,Checkly Author: Edgar RamÃ­rez-MondragÃ³n Author-email:
 edgarrm358@gmail.com Maintainer: Edgar RamÃ­rez-MondragÃ³n Maintainer-email:
 edgarrm358@gmail.com Requires-Python: >=3.7.1,<3.12 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: singer-sdk
-(>=0.14.0,<0.15.0) Project-URL: Documentation, https://github.com/
-edgarrmondragon/tap-checkly/#readme Project-URL: Repository, https://
-github.com/edgarrmondragon/tap-checkly Description-Content-Type: text/markdown
+(>=0.14,<0.24) Project-URL: Documentation, https://github.com/edgarrmondragon/
+tap-checkly/#readme Project-URL: Repository, https://github.com/
+edgarrmondragon/tap-checkly Description-Content-Type: text/markdown
                                  # tap-checkly
                        [pre-commit.ci_status] [License]
  Singer Tap for [Checkly](https://www.checklyhq.com/). Built with the [Meltano
                      Singer SDK](https://sdk.meltano.com).
 ## Capabilities * `catalog` * `state` * `discover` * `about` * `stream-maps` *
 `schema-flattening` ## Settings | Setting | Required | Default | Description |
 |:--------------------|:--------:|:-------:|:------------| | account_id | True
```

