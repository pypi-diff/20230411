# Comparing `tmp/netunicorn-connector-salt-0.3.2.tar.gz` & `tmp/netunicorn-connector-salt-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-salt-0.3.2.tar", last modified: Fri Apr  7 21:58:19 2023, max compression
+gzip compressed data, was "netunicorn-connector-salt-0.3.3.tar", last modified: Tue Apr 11 10:09:21 2023, max compression
```

## Comparing `netunicorn-connector-salt-0.3.2.tar` & `netunicorn-connector-salt-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.019979 netunicorn-connector-salt-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-07 21:58:19.019979 netunicorn-connector-salt-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 21:58:19.019979 netunicorn-connector-salt-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/netunicorn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/netunicorn/director/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.015979 netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19878 2023-04-07 21:58:08.000000 netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/connectors/salt_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 21:58:19.019979 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 21:58:19.000000 netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.408581 netunicorn-connector-salt-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-11 10:09:21.408581 netunicorn-connector-salt-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:09:21.408581 netunicorn-connector-salt-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.404580 netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22173 2023-04-11 10:09:02.000000 netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/connectors/salt_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:09:21.408581 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 10:09:21.000000 netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-salt-0.3.2/LICENSE` & `netunicorn-connector-salt-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.2/PKG-INFO` & `netunicorn-connector-salt-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.2
+Version: 0.3.3
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-salt-0.3.2/README.md` & `netunicorn-connector-salt-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-salt-0.3.2/pyproject.toml` & `netunicorn-connector-salt-0.3.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "netunicorn-connector-salt"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "SaltStack connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "netunicorn-base >= 0.2.0",
+    "netunicorn-base >= 0.2.6",
     "pyyaml",
     "returns",
     "aiohttp"
 ]
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `netunicorn-connector-salt-0.3.2/src/netunicorn/director/infrastructure/connectors/salt_connector.py` & `netunicorn-connector-salt-0.3.3/src/netunicorn/director/infrastructure/connectors/salt_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 from collections import defaultdict
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Any
 
 import aiohttp
 import yaml
 from netunicorn.base.architecture import Architecture
 from netunicorn.base.deployment import Deployment
 from netunicorn.base.environment_definitions import DockerImage, ShellExecution
 from netunicorn.base.nodes import CountableNodePool, Node
 from returns.result import Failure, Result, Success
 
-from netunicorn.director.infrastructure.connectors.protocol import (
+from netunicorn.director.base.connectors.protocol import (
     NetunicornConnectorProtocol,
 )
-from netunicorn.director.infrastructure.connectors.types import StopExecutorRequest
+from netunicorn.director.base.connectors.types import StopExecutorRequest
 
 
 class SaltConnector(NetunicornConnectorProtocol):
     def __init__(
         self,
         connector_name: str,
         config_file: str | None,
@@ -61,15 +61,21 @@
     async def health(self) -> Tuple[bool, str]:
         return True, "OK"
 
     async def shutdown(self) -> None:
         await self.session.close()
         return
 
-    async def get_nodes(self, username: str, *args, **kwargs) -> CountableNodePool:
+    async def get_nodes(
+            self,
+            username: str,
+            authentication_context: Optional[dict[str, str]] = None,
+            *args: Any,
+            **kwargs: Any,
+    ) -> CountableNodePool:
         try:
             (
                 await self.session.post(
                     self.runpoint,
                     json={
                         "client": "local",
                         "tgt": "*",
@@ -244,16 +250,18 @@
         pass
 
     async def deploy(
         self,
         username: str,
         experiment_id: str,
         deployments: list[Deployment],
-        *args,
-        **kwargs,
+        deployment_context: Optional[dict[str, str]] = None,
+        authentication_context: Optional[dict[str, str]] = None,
+        *args: Any,
+        **kwargs: Any,
     ) -> dict[str, Result[None, str]]:
         docker_deployments = []
         shell_deployments = []
         for deployment in deployments:
             if isinstance(deployment.environment_definition, DockerImage):
                 docker_deployments.append(deployment)
             elif isinstance(deployment.environment_definition, ShellExecution):
@@ -431,16 +439,18 @@
         return Success(None)
 
     async def execute(
         self,
         username: str,
         experiment_id: str,
         deployments: list[Deployment],
-        *args,
-        **kwargs,
+        execution_context: Optional[dict[str, str]] = None,
+        authentication_context: Optional[dict[str, str]] = None,
+        *args: Any,
+        **kwargs: Any,
     ) -> dict[str, Result[None, str]]:
 
         keys = [deployment.executor_id for deployment in deployments]
         # Start all deployments
         answers: tuple[Exception | Result[None, str]] = await asyncio.gather(  # type: ignore
             *(
                 self._start_single_execution(experiment_id, deployment)
@@ -453,15 +463,21 @@
             if isinstance(answer, Exception):
                 answer = Failure(str(answer))
             results[key] = answer
 
         return results
 
     async def stop_executors(
-        self, username: str, requests_list: list[StopExecutorRequest], *args, **kwargs
+        self,
+        username: str,
+        requests_list: list[StopExecutorRequest],
+        cancellation_context: Optional[dict[str, str]],
+        authentication_context: Optional[dict[str, str]] = None,
+        *args: Any,
+        **kwargs: Any,
     ) -> dict[str, Result[None, str]]:
 
         try:
             for request in requests_list:
                 self.logger.debug(
                     f"Stopping executor {request['executor_id']} on node {request['node_name']}"
                 )
@@ -481,14 +497,59 @@
                 ).raise_for_status()
         except Exception as e:
             self.logger.error(f"Error stopping executors: {e}")
             return {request["node_name"]: Failure(str(e)) for request in requests_list}
 
         return {request["node_name"]: Success(None) for request in requests_list}
 
+    async def cleanup(
+            self,
+            experiment_id: str,
+            deployments: list[Deployment],
+            *args: Any,
+            **kwargs: Any
+    ) -> None:
+        deployments = [deployment for deployment in deployments if isinstance(deployment.environment_definition, DockerImage)]
+
+        # stop containers
+        for deployment in deployments:
+            try:
+                await self.session.post(
+                    self.runpoint,
+                    json={
+                        "client": "local",
+                        "tgt": deployment.node.name,
+                        "fun": "cmd.run",
+                        "arg": [f"docker stop {deployment.executor_id}; docker rm {deployment.executor_id}"],
+                        "username": self.username,
+                        "password": self.password,
+                        "eauth": self.eauth,
+                    },
+                )
+            except Exception as e:
+                self.logger.exception(f"Error stopping container: {e}")
+
+        # remove images
+        for deployment in deployments:
+            try:
+                await self.session.post(
+                    self.runpoint,
+                    json={
+                        "client": "local",
+                        "tgt": deployment.node.name,
+                        "fun": "cmd.run",
+                        "arg": [f"docker rmi {deployment.environment_definition.image}"],
+                        "username": self.username,
+                        "password": self.password,
+                        "eauth": self.eauth,
+                    },
+                )
+            except Exception as e:
+                self.logger.exception(f"Error removing image: {e}")
+
 
 async def debug():
     from netunicorn.base import Pipeline, Experiment, Task
 
     class DummyTask(Task):
         def run(self):
             return 0
```

### Comparing `netunicorn-connector-salt-0.3.2/src/netunicorn_connector_salt.egg-info/PKG-INFO` & `netunicorn-connector-salt-0.3.3/src/netunicorn_connector_salt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-salt
-Version: 0.3.2
+Version: 0.3.3
 Summary: SaltStack connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

