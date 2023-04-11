# Comparing `tmp/alfred5-1.1.0.tar.gz` & `tmp/alfred5-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred5-1.1.0.tar", last modified: Mon Apr 10 14:03:39 2023, max compression
+gzip compressed data, was "alfred5-1.1.1.tar", last modified: Tue Apr 11 01:04:37 2023, max compression
```

## Comparing `alfred5-1.1.0.tar` & `alfred5-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-10 14:03:28.000000 alfred5-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-10 14:03:28.000000 alfred5-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-10 14:03:39.031641 alfred5-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.027641 alfred5-1.1.0/alfred5/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/alfred5/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/icons/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-10 14:03:28.000000 alfred5-1.1.0/alfred5/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/alfred5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:03:38.000000 alfred5-1.1.0/alfred5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 14:03:39.000000 alfred5-1.1.0/alfred5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-10 14:03:28.000000 alfred5-1.1.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 14:03:39.031641 alfred5-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-10 14:03:28.000000 alfred5-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:39.031641 alfred5-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 14:03:28.000000 alfred5-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-10 14:03:28.000000 alfred5-1.1.0/tests/test_snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-11 01:04:28.000000 alfred5-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 01:04:28.000000 alfred5-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-11 01:04:37.079642 alfred5-1.1.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/alfred5/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9878 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/alfred5/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/icons/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-11 01:04:28.000000 alfred5-1.1.1/alfred5/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/alfred5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 01:04:36.000000 alfred5-1.1.1/alfred5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 01:04:37.000000 alfred5-1.1.1/alfred5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-11 01:04:28.000000 alfred5-1.1.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 01:04:37.079642 alfred5-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-11 01:04:28.000000 alfred5-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:37.079642 alfred5-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 01:04:28.000000 alfred5-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-11 01:04:28.000000 alfred5-1.1.1/tests/test_snippets.py
```

### Comparing `alfred5-1.1.0/LICENSE` & `alfred5-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.0/PKG-INFO` & `alfred5-1.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,81 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.0
-Summary: Simple python wrapper for alfred workflow / snippets
+Version: 1.1.1
+Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
-Project-URL: Documentation, https://github.com/yedhrab/alfred5/wiki
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
 Project-URL: Issue Tracker, https://github.com/yedhrab/alfred5/issues
 Keywords: alfred,alfred5,workflow,snippets,alfred-workflows,alfred-snippets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 #  🎩 AlfredClient
 
 Simplest Alfred Client that I use my own projects.
 
 ```bash
 pip install alfred5
 ```
 
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
+    - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
+    - To install `from requirements.txt` do all import packages inside `main`
+            - Use `global` keyword to access imported packages globally
+        - `client.query` is the query string
+        - `client.page_count` is the page count for pagination results
+    - Dont need to add `alfred5` to `requirements.txt`
 - Use `WorkflowClient.log` to log your message to alfred debugger 
     - [debugging alfred workflow](https://www.alfredapp.com/help/workflows/utilities/debug/)
     - [why this project use stderr for all logging operation](https://www.alfredforum.com/topic/14721-get-the-python-output-back-to-alfred/?do=findComment&comment=75303)
 - Use `client.load_cached_response` and `client.cache_response` method to use caching system
     - Just do it for static response (not timebased response)
     - Db path is `db/results.yml` also you can see it from workflow debug panel
 
 ## Example Db Format
 
-![example-db](https://i.imgur.com/EW4KSq0.png)
+![example-db](https://i.imgur.com/r2whZsi.png)
 
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
 
 from alfred5 import WorkflowClient
 
 
 async def main(client: WorkflowClient):
+    # To auto install requirements all import operation must be in here
+    global get
+    from requests import get
+
     query = client.query
     client.log(f"my query: {query}")  # use it to see your log in workflow debug panel
 
-    # Use cache system to quick response
-    if client.load_cached_response():
-        return
+    # (use cache=True) Use cache system to quick response
+    # if client.load_cached_response():
+    #     return
 
     char_count = str(len( query))
     word_count = str(len(query.split(" ")))
     line_count = str(len(query.split("\n")))
 
     encoded_string = quote_plus(query)
     remove_dublication = " ".join(dict.fromkeys(query.split(" ")))
@@ -83,15 +91,16 @@
     client.add_result(lower_case, "Lower Case", arg=lower_case)
     client.add_result(capitalized, "Capitalized", arg=capitalized)
     client.add_result(template, "Template", arg=template)
     client.add_result(char_count, "Characters", arg=char_count)
     client.add_result(word_count, "Words", arg=word_count)
     client.add_result(line_count, "Lines", arg=line_count)
     
-    client.cache_response()  # to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # (use cache=True) to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # client.cache_response()  
 
 if __name__ == "__main__":
     WorkflowClient.run(main)
 
 ```
```

### Comparing `alfred5-1.1.0/alfred5/client.py` & `alfred5-1.1.1/alfred5/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 from logging import Logger, StreamHandler
 import json
+import pkg_resources
 from .models import Result
 from traceback import format_exc
 import sys
 from asyncio import run
 from collections.abc import Callable, Coroutine
 from pathlib import Path
 from shutil import copy2, move
@@ -53,14 +54,15 @@
                     zipfile.write(snippet_iconpath, snippet_iconpath.name)
 
             destination = (Path(dst) if dst else Path.cwd()) / f"{name}.alfredsnippets"
             move(snippet_path, destination)
 
 
 class WorkflowClient:
+    bare_query: str
     query: str
     page_count: int
     bundleid: str
 
     icondir: Path
 
     datadir: Path
@@ -71,16 +73,17 @@
     logger: Logger
 
     def __init__(self) -> None:
         self.logger = Logger("alfred5")
         self.logger.addHandler(StreamHandler(sys.stderr))
         self.log(f"logger initted")
 
-        self.page_count = sys.argv[1].count("+") + 1
-        self.query = sys.argv[1].replace("+", "")
+        self.bare_query = sys.argv[1]
+        self.page_count = self.bare_query.count("+") + 1
+        self.query = self.bare_query.replace("+", "")
 
         self.log(
             f"sys.argv: {sys.argv} page_count: {self.page_count} query: {self.query}"
         )
 
         self.icondir = Path(__file__).parent / "icons"
 
@@ -105,19 +108,18 @@
     def install_requirements(self) -> None:
         """Check if requirements are met"""
         self.log(f"checking requirements...")
         req_file = Path("requirements.txt")
         if req_file.exists():
             packages = req_file.read_text().splitlines()
             self.log(f"found requirements.txt: {packages}")
-            try:
-                import pkg_resources
 
+            try:
                 pkg_resources.require(packages)
-            except Exception:
+            except pkg_resources.DistributionNotFound:
                 import subprocess
 
                 command = ["python3", "-m", "pip", "install", "--target=.", *packages]
                 subprocess.Popen(
                     command,
                     start_new_session=True,
                     stdout=subprocess.DEVNULL,
@@ -136,69 +138,88 @@
     def cache_response(self) -> None:
         """Cache response to workflow db_results"""
         if not self.db_results.exists():
             self.db_results.parent.mkdir(parents=True, exist_ok=True)
             self.db_results.touch()
         with self.db_results.open("r") as f:
             data = yaml_load(f) or {}
-        data[self.query] = [
+        data[self.bare_query] = [
             {
                 "title": result.title,
                 "subtitle": result.subtitle,
                 "icon_path": result.icon.path if result.icon else None,
             }
             for result in self.results
         ]
         with self.db_results.open("w") as f:
             yaml_dump(data, f)
             self.log(f"cached response to {self.db_results}")
 
     def load_cached_response(self) -> bool:
         """Load cached result from alfred"""
-        self.log(f"checking if `{self.query}` exists in `{self.db_results}`")
+        self.log(f"checking if `{self.bare_query}` exists in `{self.db_results}`")
         if self.db_results.exists():
             with self.db_results.open("r") as f:
                 data: dict[str, list[dict[str, str]]] = self.yaml.load(f)
                 self.log(f"loaded data from {self.db_results} {len(data.keys())}")
-                if self.query in data:
+                if self.bare_query in data:
                     self.results = [
                         Result(
                             title=result["title"],
                             subtitle=result["subtitle"],
                             icon=Result.Icon(result["icon_path"])
                             if result["icon_path"]
                             else None,
                         )
-                        for result in data[self.query]
+                        for result in data[self.bare_query]
                     ]
-                    self.log(f"found: {self.query} in {self.db_results}")
+                    self.log(f"found: {self.bare_query} in {self.db_results}")
                     return True
-        self.log(f"not found `{self.query}` in `{self.db_results}`")
+        self.log(f"not found `{self.bare_query}` in `{self.db_results}`")
         return False
 
     @classmethod
     def run(
-        cls, func: Callable[[WorkflowClient], Coroutine[None, None, None]]
+        cls,
+        func: Callable[[WorkflowClient], Coroutine[None, None, None]],
+        cache: bool = False,
     ) -> NoReturn:
         """Give async main function, no need to call `client.response` method
 
-        ```
-        from alfred import AlfredWorkflowClient
-
-        async def main(alfred_client: AlfredWorkflowClient):
-            pass
-
-        if __name__ == "__main__":
-            AlfredWorkflowClient.run(main)
-        ```
+        Args:
+            `func`: async main function that takes `client` as argument
+            `cache`: cache response to workflow db_results, if cache exists, it will be loaded instead of executing `func`
+
+        - To install `from requirements.txt` do all import packages inside it
+            - Use `global` keyword to access imported packages globally
+        - `client.bare_query` is the bare query string
+        - `client.query` is the query string without `+` (page count)
+        - `client.page_count` is the page count for pagination results
+
+        Example:
+            ```
+            from alfred import WorkflowClient
+
+            async def main(client: WorkflowClient, cache=True):
+                global get
+                from requests import get
+                pass
+
+            if __name__ == "__main__":
+                WorkflowClient.run(main)
+            ```
         """
         client = cls()
+        if cache and client.load_cached_response():
+            client.response()
         try:
             client.install_requirements()
             run(func(client))
+            if cache:
+                client.cache_response()
             client.response()
         except Exception as e:
             if isinstance(e, WorkflowError):
                 client.error_response(
                     title=e.title,
                     subtitle=e.subtitle,
                     arg=e.arg,
```

### Comparing `alfred5-1.1.0/alfred5/icons/download.png` & `alfred5-1.1.1/alfred5/icons/download.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.0/alfred5/icons/error.png` & `alfred5-1.1.1/alfred5/icons/error.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.0/alfred5/models.py` & `alfred5-1.1.1/alfred5/models.py`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.0/alfred5.egg-info/PKG-INFO` & `alfred5-1.1.1/alfred5.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,81 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.0
-Summary: Simple python wrapper for alfred workflow / snippets
+Version: 1.1.1
+Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
-Project-URL: Documentation, https://github.com/yedhrab/alfred5/wiki
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
 Project-URL: Issue Tracker, https://github.com/yedhrab/alfred5/issues
 Keywords: alfred,alfred5,workflow,snippets,alfred-workflows,alfred-snippets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9.6
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 #  🎩 AlfredClient
 
 Simplest Alfred Client that I use my own projects.
 
 ```bash
 pip install alfred5
 ```
 
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
+    - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
+    - To install `from requirements.txt` do all import packages inside `main`
+            - Use `global` keyword to access imported packages globally
+        - `client.query` is the query string
+        - `client.page_count` is the page count for pagination results
+    - Dont need to add `alfred5` to `requirements.txt`
 - Use `WorkflowClient.log` to log your message to alfred debugger 
     - [debugging alfred workflow](https://www.alfredapp.com/help/workflows/utilities/debug/)
     - [why this project use stderr for all logging operation](https://www.alfredforum.com/topic/14721-get-the-python-output-back-to-alfred/?do=findComment&comment=75303)
 - Use `client.load_cached_response` and `client.cache_response` method to use caching system
     - Just do it for static response (not timebased response)
     - Db path is `db/results.yml` also you can see it from workflow debug panel
 
 ## Example Db Format
 
-![example-db](https://i.imgur.com/EW4KSq0.png)
+![example-db](https://i.imgur.com/r2whZsi.png)
 
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
 
 from alfred5 import WorkflowClient
 
 
 async def main(client: WorkflowClient):
+    # To auto install requirements all import operation must be in here
+    global get
+    from requests import get
+
     query = client.query
     client.log(f"my query: {query}")  # use it to see your log in workflow debug panel
 
-    # Use cache system to quick response
-    if client.load_cached_response():
-        return
+    # (use cache=True) Use cache system to quick response
+    # if client.load_cached_response():
+    #     return
 
     char_count = str(len( query))
     word_count = str(len(query.split(" ")))
     line_count = str(len(query.split("\n")))
 
     encoded_string = quote_plus(query)
     remove_dublication = " ".join(dict.fromkeys(query.split(" ")))
@@ -83,15 +91,16 @@
     client.add_result(lower_case, "Lower Case", arg=lower_case)
     client.add_result(capitalized, "Capitalized", arg=capitalized)
     client.add_result(template, "Template", arg=template)
     client.add_result(char_count, "Characters", arg=char_count)
     client.add_result(word_count, "Words", arg=word_count)
     client.add_result(line_count, "Lines", arg=line_count)
     
-    client.cache_response()  # to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # (use cache=True) to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # client.cache_response()  
 
 if __name__ == "__main__":
     WorkflowClient.run(main)
 
 ```
```

### Comparing `alfred5-1.1.0/docs/README.md` & `alfred5-1.1.1/docs/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,43 +4,53 @@
 
 ```bash
 pip install alfred5
 ```
 
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
+    - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
+    - To install `from requirements.txt` do all import packages inside `main`
+            - Use `global` keyword to access imported packages globally
+        - `client.query` is the query string
+        - `client.page_count` is the page count for pagination results
+    - Dont need to add `alfred5` to `requirements.txt`
 - Use `WorkflowClient.log` to log your message to alfred debugger 
     - [debugging alfred workflow](https://www.alfredapp.com/help/workflows/utilities/debug/)
     - [why this project use stderr for all logging operation](https://www.alfredforum.com/topic/14721-get-the-python-output-back-to-alfred/?do=findComment&comment=75303)
 - Use `client.load_cached_response` and `client.cache_response` method to use caching system
     - Just do it for static response (not timebased response)
     - Db path is `db/results.yml` also you can see it from workflow debug panel
 
 ## Example Db Format
 
-![example-db](https://i.imgur.com/EW4KSq0.png)
+![example-db](https://i.imgur.com/r2whZsi.png)
 
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
 
 from alfred5 import WorkflowClient
 
 
 async def main(client: WorkflowClient):
+    # To auto install requirements all import operation must be in here
+    global get
+    from requests import get
+
     query = client.query
     client.log(f"my query: {query}")  # use it to see your log in workflow debug panel
 
-    # Use cache system to quick response
-    if client.load_cached_response():
-        return
+    # (use cache=True) Use cache system to quick response
+    # if client.load_cached_response():
+    #     return
 
     char_count = str(len( query))
     word_count = str(len(query.split(" ")))
     line_count = str(len(query.split("\n")))
 
     encoded_string = quote_plus(query)
     remove_dublication = " ".join(dict.fromkeys(query.split(" ")))
@@ -56,15 +66,16 @@
     client.add_result(lower_case, "Lower Case", arg=lower_case)
     client.add_result(capitalized, "Capitalized", arg=capitalized)
     client.add_result(template, "Template", arg=template)
     client.add_result(char_count, "Characters", arg=char_count)
     client.add_result(word_count, "Words", arg=word_count)
     client.add_result(line_count, "Lines", arg=line_count)
     
-    client.cache_response()  # to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # (use cache=True) to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # client.cache_response()  
 
 if __name__ == "__main__":
     WorkflowClient.run(main)
 
 ```
```

### Comparing `alfred5-1.1.0/setup.py` & `alfred5-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,70 @@
+"""Setup script for package
+
+References: 
+    - https://github.com/openai/openai-python/blob/main/setup.cfg
+"""
+
 from glob import glob
 from os.path import basename, splitext
 from setuptools import find_packages, setup
 from pathlib import Path
 
-VERSION = "1.1.0"
+VERSION = "1.1.1"
+DESCRIPTION = "Simple python wrapper for alfred5 workflow / snippets"
 README_PATH = "docs/README.md"
 USERNAME = "yedhrab"
 REPOSITORY = "alfred5"
+KEYWORDS = [
+    "alfred",
+    "alfred5",
+    "workflow",
+    "snippets",
+    "alfred-workflows",
+    "alfred-snippets",
+]
+INSTALL_REQUIRES = ["aiohttp==3.8.4", "ruamel.yaml==0.17.21"]
+EXSTRAS_REQUIRE = {
+    "dev": [
+        "black==23.3.0",
+        "autoflake==2.0.2",
+        "pytest==7.3.0",
+        "pytest-asyncio==0.21.0",
+    ]
+}
 
 setup(
     name=REPOSITORY,
     version=VERSION,
     license="Apache Software License 2.0",
-    description="Simple python wrapper for alfred workflow / snippets",
+    description=DESCRIPTION,
     long_description=Path(README_PATH).read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     author="Yunus Emre Ak",
     author_email="yemreak.com@gmail.com",
     url=f"https://github.com/{USERNAME}/{REPOSITORY}",
     packages=find_packages(),
     py_modules=[splitext(basename(path))[0] for path in glob(f"*.py")],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
-        "Operating System :: Unix",
-        "Operating System :: POSIX",
-        "Operating System :: Microsoft :: Windows",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
     ],
     project_urls={
         "Source": f"https://github.com/{USERNAME}/{REPOSITORY}/",
-        "Documentation": f"https://github.com/{USERNAME}/{REPOSITORY}/wiki",
         "Changelog": f"https://github.com/{USERNAME}/{REPOSITORY}/releases",
         "Issue Tracker": f"https://github.com/{USERNAME}/{REPOSITORY}/issues",
     },
-    keywords=[
-        "alfred",
-        "alfred5",
-        "workflow",
-        "snippets",
-        "alfred-workflows",
-        "alfred-snippets",
-    ],
+    keywords=KEYWORDS,
     python_requires=">=3.9.6",
-    install_requires=["aiohttp==3.8.3", "ruamel.yaml==0.17.21"],
-    extras_require={},
+    install_requires=INSTALL_REQUIRES,
+    extras_require=EXSTRAS_REQUIRE,
     setup_requires=[],
     entry_points={},
 )
```

