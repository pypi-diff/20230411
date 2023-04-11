# Comparing `tmp/fastapi_poe-0.0.5.tar.gz` & `tmp/fastapi_poe-0.0.6.tar.gz`

## Comparing `fastapi_poe-0.0.5.tar` & `fastapi_poe-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/src/fastapi_poe/__init__.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/src/fastapi_poe/__main__.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/src/fastapi_poe/base.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/src/fastapi_poe/types.py
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/src/fastapi_poe/samples/catbot.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/src/fastapi_poe/samples/echo.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/.gitignore
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 fastapi_poe-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/__main__.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/base.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/types.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/samples/catbot.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/src/fastapi_poe/samples/echo.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 fastapi_poe-0.0.6/PKG-INFO
```

### Comparing `fastapi_poe-0.0.5/src/fastapi_poe/base.py` & `fastapi_poe-0.0.6/src/fastapi_poe/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-from __future__ import annotations
-
 import argparse
 import copy
 import json
 import logging
 import os
-from typing import Any, AsyncIterable
+from typing import Any, AsyncIterable, Dict, Optional, Union
 
 from fastapi import Depends, FastAPI, HTTPException, Request, Response
 from fastapi.exceptions import RequestValidationError
 from fastapi.responses import HTMLResponse, JSONResponse
 from fastapi.security import HTTPBearer
 from sse_starlette.sse import EventSourceResponse, ServerSentEvent
 from starlette.middleware.base import BaseHTTPMiddleware
@@ -130,17 +128,17 @@
                 }
             ),
             event="meta",
         )
 
     @staticmethod
     def error_event(
-        text: str | None = None, *, allow_retry: bool = True
+        text: Optional[str] = None, *, allow_retry: bool = True
     ) -> ServerSentEvent:
-        data: dict[str, bool | str] = {"allow_retry": allow_retry}
+        data: Dict[str, Union[bool, str]] = {"allow_retry": allow_retry}
         if text is not None:
             data["text"] = text
         return ServerSentEvent(data=json.dumps(data), event="error")
 
     # Internal handlers
 
     async def handle_report_feedback(
@@ -194,15 +192,15 @@
         return HTMLResponse(
             "<html><body><h1>FastAPI Poe bot server</h1><p>Congratulations! Your server"
             " is running. To connect it to Poe, create a bot at <a"
             f' href="{url}">{url}</a>.</p></body></html>'
         )
 
     @app.post("/")
-    async def poe_post(request: dict[str, Any], dict=Depends(auth_user)) -> Response:
+    async def poe_post(request: Dict[str, Any], dict=Depends(auth_user)) -> Response:
         if request["type"] == "query":
             return EventSourceResponse(
                 handler.handle_query(QueryRequest.parse_obj(request))
             )
         elif request["type"] == "settings":
             return await handler.handle_settings(SettingsRequest.parse_obj(request))
         elif request["type"] == "report_feedback":
```

### Comparing `fastapi_poe-0.0.5/src/fastapi_poe/types.py` & `fastapi_poe-0.0.6/src/fastapi_poe/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.5/src/fastapi_poe/samples/catbot.py` & `fastapi_poe-0.0.6/src/fastapi_poe/samples/catbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             yield self.text_event("\n")
             yield self.text_event("A table:\n\n")
             yield self.text_event("| animal | cuteness |\n")
             yield self.text_event("|--------|----------|\n")
             yield self.text_event("| cat    | 10       |\n")
             yield self.text_event("| dog    | 1        |\n")
             yield self.text_event("\n")
-        if "cardbord" in last_message:
+        if "cardboard" in last_message:
             yield self.text_event("crunch ")
             yield self.text_event("crunch")
         elif (
             "kitchen" in last_message
             or "meal" in last_message
             or "food" in last_message
         ):
```

### Comparing `fastapi_poe-0.0.5/src/fastapi_poe/samples/echo.py` & `fastapi_poe-0.0.6/src/fastapi_poe/samples/echo.py`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.5/README.md` & `fastapi_poe-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_poe-0.0.5/pyproject.toml` & `fastapi_poe-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_poe"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Lida Li", email="lli@quora.com" },
 ]
 description = "A demonstration of the Poe protocol using FastAPI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `fastapi_poe-0.0.5/PKG-INFO` & `fastapi_poe-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_poe
-Version: 0.0.5
+Version: 0.0.6
 Summary: A demonstration of the Poe protocol using FastAPI
 Project-URL: Homepage, https://github.com/quora/poe-protocol
 Author-email: Lida Li <lli@quora.com>
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

