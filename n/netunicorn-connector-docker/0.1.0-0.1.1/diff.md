# Comparing `tmp/netunicorn-connector-docker-0.1.0.tar.gz` & `tmp/netunicorn-connector-docker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netunicorn-connector-docker-0.1.0.tar", last modified: Tue Apr 11 07:09:10 2023, max compression
+gzip compressed data, was "netunicorn-connector-docker-0.1.1.tar", last modified: Tue Apr 11 09:45:16 2023, max compression
```

## Comparing `netunicorn-connector-docker-0.1.0.tar` & `netunicorn-connector-docker-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/
--rw-rw-r--   0 kell      (1000) kell      (1000)     1072 2023-04-10 19:20:33.000000 netunicorn-connector-docker-0.1.0/LICENSE
--rw-rw-r--   0 kell      (1000) kell      (1000)      848 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/PKG-INFO
--rw-rw-r--   0 kell      (1000) kell      (1000)      508 2023-04-10 22:31:50.000000 netunicorn-connector-docker-0.1.0/README.md
--rw-rw-r--   0 kell      (1000) kell      (1000)      566 2023-04-10 20:57:14.000000 netunicorn-connector-docker-0.1.0/pyproject.toml
--rw-rw-r--   0 kell      (1000) kell      (1000)       38 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/setup.cfg
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/src/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/src/netunicorn/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/src/netunicorn/director/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/src/netunicorn/director/infrastructure/
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/src/netunicorn/director/infrastructure/connectors/
--rw-rw-r--   0 kell      (1000) kell      (1000)       46 2023-04-11 03:28:32.000000 netunicorn-connector-docker-0.1.0/src/netunicorn/director/infrastructure/connectors/__init__.py
--rw-rw-r--   0 kell      (1000) kell      (1000)     9697 2023-04-11 07:02:30.000000 netunicorn-connector-docker-0.1.0/src/netunicorn/director/infrastructure/connectors/docker_connector.py
-drwxrwxr-x   0 kell      (1000) kell      (1000)        0 2023-04-11 07:09:10.914384 netunicorn-connector-docker-0.1.0/src/netunicorn_connector_docker.egg-info/
--rw-rw-r--   0 kell      (1000) kell      (1000)      848 2023-04-11 07:09:10.000000 netunicorn-connector-docker-0.1.0/src/netunicorn_connector_docker.egg-info/PKG-INFO
--rw-rw-r--   0 kell      (1000) kell      (1000)      438 2023-04-11 07:09:10.000000 netunicorn-connector-docker-0.1.0/src/netunicorn_connector_docker.egg-info/SOURCES.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)        1 2023-04-11 07:09:10.000000 netunicorn-connector-docker-0.1.0/src/netunicorn_connector_docker.egg-info/dependency_links.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)       38 2023-04-11 07:09:10.000000 netunicorn-connector-docker-0.1.0/src/netunicorn_connector_docker.egg-info/requires.txt
--rw-rw-r--   0 kell      (1000) kell      (1000)       11 2023-04-11 07:09:10.000000 netunicorn-connector-docker-0.1.0/src/netunicorn_connector_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.393097 netunicorn-connector-docker-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.393097 netunicorn-connector-docker-0.1.1/src/netunicorn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.393097 netunicorn-connector-docker-0.1.1/src/netunicorn/director/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.393097 netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10782 2023-04-11 09:45:02.000000 netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/connectors/docker_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:45:16.397097 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 09:45:16.000000 netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/top_level.txt
```

### Comparing `netunicorn-connector-docker-0.1.0/LICENSE` & `netunicorn-connector-docker-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netunicorn-connector-docker-0.1.0/PKG-INFO` & `netunicorn-connector-docker-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-docker
-Version: 0.1.0
+Version: 0.1.1
 Summary: Local Docker connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `netunicorn-connector-docker-0.1.0/pyproject.toml` & `netunicorn-connector-docker-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netunicorn-connector-docker"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Roman Beltiukov", email = "rbeltiukov@ucsb.edu"},
 ]
 description = "Local Docker connector for netunicorn"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["netunicorn"]
```

### Comparing `netunicorn-connector-docker-0.1.0/src/netunicorn/director/infrastructure/connectors/docker_connector.py` & `netunicorn-connector-docker-0.1.1/src/netunicorn/director/infrastructure/connectors/docker_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 from netunicorn.base.architecture import Architecture
 from netunicorn.base.deployment import Deployment
 from netunicorn.base.environment_definitions import DockerImage
 from netunicorn.base.nodes import CountableNodePool, Node, Nodes
 from returns.result import Failure, Result, Success
 
-from netunicorn.director.infrastructure.connectors.protocol import (
+from netunicorn.director.base.connectors.protocol import (
     NetunicornConnectorProtocol,
 )
-from netunicorn.director.infrastructure.connectors.types import StopExecutorRequest
+from netunicorn.director.base.connectors.types import StopExecutorRequest
 
 
 class DockerConnector(NetunicornConnectorProtocol):
     def __init__(
             self,
             connector_name: str,
             configuration: str | None,
@@ -204,14 +204,42 @@
                 self.logger.debug(f"Container {request['executor_id']} was not found")
             except Exception as e:
                 result[request['executor_id']] = Failure(str(e))
                 self.logger.exception(e)
 
         return result
 
+    async def cleanup(
+            self,
+            experiment_id: str,
+            deployments: list[Deployment],
+            *args: Any,
+            **kwargs: Any
+    ) -> None:
+        # stop containers if they are still working
+        for deployment in deployments:
+            try:
+                container = self.client.containers.get(deployment.executor_id)
+                container.stop()
+                self.logger.debug(f"Stopped container {deployment.executor_id}")
+            except docker.errors.NotFound:
+                pass
+            except Exception as e:
+                self.logger.exception(e)
+
+        # remove images
+        for deployment in deployments:
+            try:
+                self.client.images.remove(deployment.environment_definition.image)
+                self.logger.debug(f"Removed image {deployment.environment_definition.image}")
+            except docker.errors.ImageNotFound:
+                self.logger.debug(f"Image {deployment.environment_definition.image} was not found")
+            except Exception as e:
+                self.logger.exception(e)
+
 
 async def test_main():
     from netunicorn.base.pipeline import Pipeline
     import uuid
 
     logger = logging.getLogger('test-logger')
     logger.setLevel(logging.DEBUG)
```

### Comparing `netunicorn-connector-docker-0.1.0/src/netunicorn_connector_docker.egg-info/PKG-INFO` & `netunicorn-connector-docker-0.1.1/src/netunicorn_connector_docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netunicorn-connector-docker
-Version: 0.1.0
+Version: 0.1.1
 Summary: Local Docker connector for netunicorn
 Author-email: Roman Beltiukov <rbeltiukov@ucsb.edu>
 License: MIT
 Keywords: netunicorn
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

