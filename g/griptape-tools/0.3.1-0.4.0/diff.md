# Comparing `tmp/griptape_tools-0.3.1.tar.gz` & `tmp/griptape_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.3.1.tar", max compression
+gzip compressed data, was "griptape_tools-0.4.0.tar", max compression
```

## Comparing `griptape_tools-0.3.1.tar` & `griptape_tools-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.3.1/LICENSE
--rw-r--r--   0        0        0      940 2023-04-06 20:56:04.343666 griptape_tools-0.3.1/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.3.1/griptape/__init__.py
--rw-r--r--   0        0        0      137 2023-04-07 15:29:21.691602 griptape_tools-0.3.1/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.3.1/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.3.1/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       20 2023-04-09 16:57:04.925786 griptape_tools-0.3.1/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0     1513 2023-04-09 16:48:43.512439 griptape_tools-0.3.1/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.3.1/griptape/tools/google_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.3.1/griptape/tools/google_search/manifest.yml
--rw-r--r--   0        0        0       20 2023-04-09 16:57:04.927625 griptape_tools-0.3.1/griptape/tools/google_search/requirements.txt
--rw-r--r--   0        0        0     2436 2023-04-09 16:48:43.509967 griptape_tools-0.3.1/griptape/tools/google_search/tool.py
--rw-r--r--   0        0        0      525 2023-04-09 16:57:59.445954 griptape_tools-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 griptape_tools-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.4.0/LICENSE
+-rw-r--r--   0        0        0      940 2023-04-06 20:56:04.343666 griptape_tools-0.4.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.4.0/griptape/__init__.py
+-rw-r--r--   0        0        0      137 2023-04-07 15:29:21.691602 griptape_tools-0.4.0/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.4.0/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.4.0/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       20 2023-04-11 20:40:54.042137 griptape_tools-0.4.0/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0     1466 2023-04-11 17:42:54.149645 griptape_tools-0.4.0/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.4.0/griptape/tools/google_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.4.0/griptape/tools/google_search/manifest.yml
+-rw-r--r--   0        0        0       20 2023-04-11 20:40:54.044431 griptape_tools-0.4.0/griptape/tools/google_search/requirements.txt
+-rw-r--r--   0        0        0     2389 2023-04-11 17:42:54.155798 griptape_tools-0.4.0/griptape/tools/google_search/tool.py
+-rw-r--r--   0        0        0      525 2023-04-11 20:40:54.038520 griptape_tools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 griptape_tools-0.4.0/PKG-INFO
```

### Comparing `griptape_tools-0.3.1/LICENSE` & `griptape_tools-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.3.1/README.md` & `griptape_tools-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.3.1/griptape/tools/calculator/tool.py` & `griptape_tools-0.4.0/griptape/tools/calculator/tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 
 
 class Calculator(BaseTool):
     configs = {
         "calculate": {
             "name": "calculate",
             "description": "Used for making simple calculations in Python.",
-            "input_schema": Schema({
+            "value_schema": Schema({
                 Literal(
-                    "action_input",
+                    "value",
                     description="Arithmetic expression parsable in pure Python. Single line only. Don't use any "
                                 "imports or external libraries."
                 ): str
-            }),
-            "foo": "bar"
+            })
         }
     }
 
     @action(config=configs["calculate"])
-    def calculate(self, action_input: bytes) -> str:
+    def calculate(self, value: bytes) -> str:
         try:
-            return self._exec_python(action_input.decode())
+            return self._exec_python(value.decode())
         except Exception as e:
             return f"error calculating: {e}"
 
     def _exec_python(self, code: str, libs: dict[str, str] = {}) -> str:
         global_stdout = sys.stdout
         sys.stdout = local_stdout = StringIO()
```

### Comparing `griptape_tools-0.3.1/griptape/tools/google_search/tool.py` & `griptape_tools-0.4.0/griptape/tools/google_search/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,35 +7,34 @@
 
 @define
 class GoogleSearch(BaseTool):
     configs = {
         "search": {
             "name": "search",
             "description": "Used for searching Google.",
-            "input_schema": Schema({
+            "value_schema": Schema({
                 Literal(
-                    "action_input",
+                    "value",
                     description="Google search request that returns a list of pages with titles, descriptions, and URLs"
                 ): str
-            }),
-            "foo": "bar"
+            })
         }
     }
 
     results_count: int = field(default=5, kw_only=True, metadata={"env": "GOOGLE_RESULTS_COUNT"})
     lang: str = field(default="lang_en", kw_only=True, metadata={"env": "GOOGLE_LANG"})
     api_search_key: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_SEARCH_KEY"})
     api_search_id: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_SEARCH_ID"})
     api_country: str = field(default="us", kw_only=True, metadata={"env": "GOOGLE_API_COUNTRY"})
 
     @action(config=configs["search"])
-    def search(self, action_input: bytes) -> dict:
+    def search(self, value: bytes) -> dict:
         try:
             return {
-                "results": self._search_api(action_input.decode())
+                "results": self._search_api(value.decode())
             }
         except Exception as e:
             return {
                 "error": f"error searching Google: {e}"
             }
 
     def _search_api(self, query: str) -> list[dict]:
```

### Comparing `griptape_tools-0.3.1/pyproject.toml` & `griptape_tools-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.3.1"
+version = "0.4.0"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-griptape-core = ">=0.3.0"
+griptape-core = ">=0.4.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-mock = "*"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `griptape_tools-0.3.1/PKG-INFO` & `griptape_tools-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.3.1
+Version: 0.4.0
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape-core (>=0.3.0)
+Requires-Dist: griptape-core (>=0.4.0)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
 # Griptape Tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
```

