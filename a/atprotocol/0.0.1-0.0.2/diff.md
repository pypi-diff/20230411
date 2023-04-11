# Comparing `tmp/atprotocol-0.0.1.tar.gz` & `tmp/atprotocol-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atprotocol-0.0.1.tar", max compression
+gzip compressed data, was "atprotocol-0.0.2.tar", max compression
```

## Comparing `atprotocol-0.0.1.tar` & `atprotocol-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      272 2023-04-11 01:02:38.106059 atprotocol-0.0.1/README.md
--rw-r--r--   0        0        0       88 2023-04-09 16:43:58.835762 atprotocol-0.0.1/protopy/README.md
--rw-r--r--   0        0        0       40 2023-04-11 00:44:52.475414 atprotocol-0.0.1/protopy/__init__.py
--rw-r--r--   0        0        0     1146 2023-04-11 00:32:23.768748 atprotocol-0.0.1/protopy/agent.py
--rw-r--r--   0        0        0       42 2023-04-11 00:35:08.917599 atprotocol-0.0.1/protopy/bsky/__init__.py
--rw-r--r--   0        0        0     3639 2023-04-11 00:38:11.350283 atprotocol-0.0.1/protopy/bsky/agent.py
--rw-r--r--   0        0        0     3875 2023-04-11 00:38:42.032263 atprotocol-0.0.1/protopy/bsky/types.py
--rw-r--r--   0        0        0      142 2023-04-11 00:35:23.767002 atprotocol-0.0.1/protopy/types.py
--rw-r--r--   0        0        0      955 2023-04-11 01:02:24.361499 atprotocol-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 atprotocol-0.0.1/setup.py
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 atprotocol-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    57417 2023-04-11 01:12:48.876068 atprotocol-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1502 2023-04-11 01:36:01.127112 atprotocol-0.0.2/README.md
+-rw-r--r--   0        0        0       40 2023-04-11 00:44:52.475414 atprotocol-0.0.2/atprotocol/__init__.py
+-rw-r--r--   0        0        0     1304 2023-04-11 01:25:22.314683 atprotocol-0.0.2/atprotocol/agent.py
+-rw-r--r--   0        0        0       42 2023-04-11 00:35:08.917599 atprotocol-0.0.2/atprotocol/bsky/__init__.py
+-rw-r--r--   0        0        0     3645 2023-04-11 01:17:54.354039 atprotocol-0.0.2/atprotocol/bsky/agent.py
+-rw-r--r--   0        0        0     3875 2023-04-11 01:05:01.009471 atprotocol-0.0.2/atprotocol/bsky/types.py
+-rw-r--r--   0        0        0      142 2023-04-11 00:35:23.767002 atprotocol-0.0.2/atprotocol/types.py
+-rw-r--r--   0        0        0      958 2023-04-11 01:52:22.908052 atprotocol-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2263 1970-01-01 00:00:00.000000 atprotocol-0.0.2/setup.py
+-rw-r--r--   0        0        0     1970 1970-01-01 00:00:00.000000 atprotocol-0.0.2/PKG-INFO
```

### Comparing `atprotocol-0.0.1/protopy/agent.py` & `atprotocol-0.0.2/atprotocol/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-from protopy.types import Session
+from atprotocol.types import Session
 
 
 class AtpAgent:
     """Generic agent for interacting with any ATP app."""
 
     def __init__(
         self,
@@ -20,21 +20,26 @@
             raise Exception("Not logged in.")
 
         return {"Authorization": f"Bearer {self.session.accessJwt}"}
 
     def login(self, identifier: str, password: str) -> None:
         """Create ATP session for specified host URL."""
 
+        # TODO: Clean this up
         res = requests.post(
             url=f"{self.service}/xrpc/com.atproto.server.createSession",
             json={"identifier": identifier, "password": password},
         )
 
-        if res.history[0].status_code == 301:
-            redirect_url = res.history[0].headers["Location"]
+        try:
+            self.session = Session.parse_obj(res.json())
 
-            res = requests.post(
-                url=redirect_url,
-                json={"identifier": identifier, "password": password},
-            )
+        except Exception:
+            if res.history[0].status_code == 301:
+                redirect_url = res.history[0].headers["Location"]
+
+                res = requests.post(
+                    url=redirect_url,
+                    json={"identifier": identifier, "password": password},
+                )
 
-        self.session = Session.parse_obj(res.json())
+            self.session = Session.parse_obj(res.json())
```

### Comparing `atprotocol-0.0.1/protopy/bsky/agent.py` & `atprotocol-0.0.2/atprotocol/bsky/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
-from protopy import AtpAgent
-from protopy.bsky.types import (
+from atprotocol import AtpAgent
+from atprotocol.bsky.types import (
     ActorResults,
     Feed,
     Followers,
     Likes,
     Profile,
     Profiles,
     Reposts,
```

### Comparing `atprotocol-0.0.1/protopy/bsky/types.py` & `atprotocol-0.0.2/atprotocol/bsky/types.py`

 * *Files identical despite different names*

### Comparing `atprotocol-0.0.1/pyproject.toml` & `atprotocol-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "atprotocol"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python wrapper for the ATProtocol API"
 authors = ["Jett Hollister <jett.hollister@proton.me>"]
 readme = "README.md"
-packages = [{include = 'protopy'}]
+packages = [{include = 'atprotocol'}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-python-dotenv = "^1.0.0"
 requests = "^2.28.2"
 pydantic = "^1.10.7"
-pre-commit = "^3.2.2"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 ruff = "^0.0.261"
 black = "^23.3.0"
 isort = "^5.12.0"
 ipykernel = "^6.22.0"
 types-requests = "^2.28.11.17"
+pre-commit = "^3.2.2"
+python-dotenv = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
```

