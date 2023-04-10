# Comparing `tmp/robotnikmq-0.4.1.tar.gz` & `tmp/robotnikmq-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotnikmq-0.4.1.tar", last modified: Sun Feb 19 20:44:38 2023, max compression
+gzip compressed data, was "robotnikmq-0.5.0.tar", last modified: Mon Apr 10 22:43:32 2023, max compression
```

## Comparing `robotnikmq-0.4.1.tar` & `robotnikmq-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0    34500 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/LICENSE
--rw-r--r--   0        0        0     6369 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/README.md
--rw-r--r--   0        0        0     1165 2023-02-19 20:42:51.432704 robotnikmq-0.4.1/pyproject.toml
--rwxr-xr-x   0        0        0      320 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/__init__.py
--rwxr-xr-x   0        0        0     4899 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/config.py
--rw-r--r--   0        0        0     5675 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/core.py
--rwxr-xr-x   0        0        0      652 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/error.py
--rw-r--r--   0        0        0     1230 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/log.py
--rw-r--r--   0        0        0     2649 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/rpc_client.py
--rw-r--r--   0        0        0    11347 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/rpc_server.py
--rw-r--r--   0        0        0     4304 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/subscriber.py
--rwxr-xr-x   0        0        0     1233 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/topic.py
--rw-r--r--   0        0        0      471 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/robotnikmq/utils.py
--rw-r--r--   0        0        0        0 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/__init__.py
--rwxr-xr-x   0        0        0    16188 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/test_broadcast.py
--rw-r--r--   0        0        0    13648 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/test_rpc.py
--rw-r--r--   0        0        0     2088 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/utils.py
--rw-r--r--   0        0        0    13754 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/library/ca.py
--rw-r--r--   0        0        0    12451 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/library/cert.py
--rw-r--r--   0        0        0      739 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/provision.yaml
--rw-r--r--   0        0        0       84 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/handlers/main.yaml
--rw-r--r--   0        0        0       19 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/meta/main.yaml
--rw-r--r--   0        0        0      102 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/tasks/main.yaml
--rw-r--r--   0        0        0     1609 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml
--rw-r--r--   0        0        0     4907 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml
--rwxr-xr-x   0        0        0      588 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml
--rw-r--r--   0        0        0     1236 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2
--rw-r--r--   0        0        0     1012 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2
--rw-r--r--   0        0        0       29 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/tls/tasks/main.yaml
--rw-r--r--   0        0        0     2522 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/roles/tls/tasks/tls.yaml
--rw-r--r--   0        0        0      172 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/integration/vagrant/testing
--rw-r--r--   0        0        0        0 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     4142 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/unit/test_config.py
--rw-r--r--   0        0        0      261 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/unit/test_error.py
--rw-r--r--   0        0        0     1818 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/unit/test_message.py
--rw-r--r--   0        0        0     1292 2022-12-29 00:46:05.562203 robotnikmq-0.4.1/tests/unit/test_validation.py
--rw-r--r--   0        0        0     6652 1970-01-01 00:00:00.000000 robotnikmq-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6369 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/README.md
+-rw-r--r--   0        0        0     1212 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0      320 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/robotnikmq/__init__.py
+-rwxr-xr-x   0        0        0     5330 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/config.py
+-rw-r--r--   0        0        0     6363 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/core.py
+-rwxr-xr-x   0        0        0      652 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/robotnikmq/error.py
+-rw-r--r--   0        0        0     1230 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/robotnikmq/log.py
+-rw-r--r--   0        0        0     2649 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/robotnikmq/rpc_client.py
+-rw-r--r--   0        0        0    11552 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/rpc_server.py
+-rw-r--r--   0        0        0     4359 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/subscriber.py
+-rwxr-xr-x   0        0        0     1411 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/topic.py
+-rw-r--r--   0        0        0      471 2023-04-10 14:34:22.584553 robotnikmq-0.5.0/robotnikmq/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:18.502194 robotnikmq-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:20.222199 robotnikmq-0.5.0/tests/integration/__init__.py
+-rwxr-xr-x   0        0        0    16298 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/tests/integration/test_broadcast.py
+-rw-r--r--   0        0        0     1632 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/tests/integration/test_disconnects.py
+-rw-r--r--   0        0        0    13648 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/test_rpc.py
+-rw-r--r--   0        0        0     2740 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/tests/integration/utils.py
+-rw-r--r--   0        0        0    13754 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/library/ca.py
+-rw-r--r--   0        0        0    12451 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/library/cert.py
+-rw-r--r--   0        0        0      739 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/provision.yaml
+-rw-r--r--   0        0        0       84 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/handlers/main.yaml
+-rw-r--r--   0        0        0       19 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/meta/main.yaml
+-rw-r--r--   0        0        0      102 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/main.yaml
+-rw-r--r--   0        0        0     1609 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml
+-rw-r--r--   0        0        0     4907 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml
+-rwxr-xr-x   0        0        0      588 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml
+-rw-r--r--   0        0        0     1236 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2
+-rw-r--r--   0        0        0     1012 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2
+-rw-r--r--   0        0        0       29 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/tls/tasks/main.yaml
+-rw-r--r--   0        0        0     2522 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/tls/tasks/tls.yaml
+-rw-r--r--   0        0        0      172 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/testing
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:21.330203 robotnikmq-0.5.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4142 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/unit/test_config.py
+-rw-r--r--   0        0        0      261 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/unit/test_error.py
+-rw-r--r--   0        0        0     1818 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/unit/test_message.py
+-rw-r--r--   0        0        0     1292 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/unit/test_validation.py
+-rw-r--r--   0        0        0     6652 1970-01-01 00:00:00.000000 robotnikmq-0.5.0/PKG-INFO
```

### Comparing `robotnikmq-0.4.1/LICENSE` & `robotnikmq-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/README.md` & `robotnikmq-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/pyproject.toml` & `robotnikmq-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 [project]
 name = "robotnikmq"
-version = "0.4.1"
+version = "0.5.0"
 description = "Utilities for safe, efficient, and scalable infrastructure using RabbitMQ"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
-    "typeguard>=2.13.3",
+    "typeguard>=3.0.2",
     "pyyaml>=6.0",
     "pydantic>=1.0",
     "pika>=1.3.0",
     "funcy>=1.17",
     "arrow>=1.2.3",
     "logzero>=1.7.0",
-    "retry2>=0.9.4",
     "types-pika>=1.2.0b1",
     "types-pyyaml>=6.0.11",
+    "typing-extensions>=4.5.0",
+    "tenacity>=8.2.2",
 ]
 requires-python = ">3.8.2"
 readme = "README.md"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.optional-dependencies]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "pytest<7.0.0,>=6.2.5",
-    "pytest-cov<4.0.0,>=2.0.0",
+    "pytest>=7.3.0",
+    "pytest-cov>=4.0.0",
     "pylint<3.0.0,>=2.12.2",
     "mypy<1.0,>=0.930",
     "flake8<5.0.0,>=3.0.0",
     "mkdocs>=1.0.0",
     "mkdocstrings[python]>=0.10.0",
     "mkdocs-cinder>=1.2.0",
-    "pytest-rabbitmq>=2.0.0",
+    "pytest-rabbitmq>=2.2.1",
     "pudb>=2022.1.2",
+    "types-retry>=0.9.9.3",
 ]
 
 [tool.pdm.scripts.publish-test]
 cmd = "twine upload -r testpypi dist/*"
 
 [tool.pdm.scripts.publish-prod]
 cmd = "twine upload -r pypi dist/*"
```

### Comparing `robotnikmq-0.4.1/robotnikmq/config.py` & `robotnikmq-0.5.0/robotnikmq/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -132,16 +132,32 @@
         )
     else:
         raise InvalidConfiguration(
             "Either all public key encryption fields (cert, key, ca-cert) must be provided, or none of them."
         )
 
 
+class ConnectionConfig(BaseModel):
+    attempts: int = 10
+    wait_random_min_seconds: int = 2
+    wait_random_max_seconds: int = 5
+
+
+@typechecked
+def conn_config(attempts: int, min_wait: int, max_wait: int) -> ConnectionConfig:
+    return ConnectionConfig(
+        attempts=attempts,
+        wait_random_min_seconds=min_wait,
+        wait_random_max_seconds=max_wait,
+    )
+
+
 class RobotnikConfig(BaseModel):
     tiers: List[List[ServerConfig]]
+    connection: ConnectionConfig = ConnectionConfig()
 
     @typechecked
     def tier(self, index: int) -> List[ServerConfig]:
         return self.tiers[index]
 
     @typechecked
     def a_server(self, tier: int) -> ServerConfig:
```

### Comparing `robotnikmq-0.4.1/robotnikmq/core.py` & `robotnikmq-0.5.0/robotnikmq/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from contextlib import contextmanager
 from datetime import datetime
-from json import loads as from_json
+from json import loads as _from_json
 from json.decoder import JSONDecodeError
 from pathlib import Path
+from pprint import pprint
 from random import sample
 from ssl import SSLError
 from threading import current_thread
 from typing import Optional, Callable, Any, Dict, Union, Generator, List
 from uuid import uuid4 as uuid, UUID
 
 from arrow import Arrow, get as to_arrow, now
 from funcy import first
 from pika import BlockingConnection
 from pika.adapters.blocking_connection import BlockingChannel
 from pika.exceptions import AMQPError, AMQPConnectionError
 from pydantic import BaseModel  # pylint: disable=E0611
+from tenacity import (
+    retry_if_exception_type,
+    stop_after_attempt,
+    wait_random,
+    Retrying,
+)
 from typeguard import typechecked
 
 from robotnikmq.config import RobotnikConfig, config_of
 from robotnikmq.error import UnableToConnect, MalformedMessage
-from robotnikmq.utils import to_json
+from robotnikmq.utils import to_json as _to_json
 
 AMQPErrorCallback = Optional[Callable[[AMQPError], None]]
 ConnErrorCallback = Optional[Callable[[AMQPConnectionError], None]]
 
 
 @contextmanager
 def thread_name(name: Union[str, UUID]):
@@ -33,24 +40,24 @@
     yield
     thread.name = original
 
 
 @typechecked
 def jsonable(content: Any) -> bool:
     try:
-        to_json(content)
+        _to_json(content)
         return True
     except (TypeError, OverflowError):
         return False
 
 
 @typechecked
 def valid_json(string: str) -> bool:
     try:
-        from_json(string)
+        _from_json(string)
         return True
     except JSONDecodeError:
         return False
 
 
 class Message:
     @typechecked
@@ -75,21 +82,21 @@
             "contents": self.contents,
             "msg_id": str(self.msg_id),
             "timestamp": self.timestamp.int_timestamp,
         }
 
     @typechecked
     def to_json(self) -> str:
-        return to_json(self.to_dict())
+        return _to_json(self.to_dict())
 
     @staticmethod
     @typechecked
     def of(body: str) -> "Message":  # pylint: disable=C0103
         try:
-            msg = from_json(body)
+            msg = _from_json(body)
             return Message(
                 msg["contents"], msg["routing_key"], msg["timestamp"], msg["msg_id"]
             )
         except (JSONDecodeError, KeyError) as exc:
             raise MalformedMessage(body) from exc
 
     @typechecked
@@ -147,16 +154,28 @@
                         self._on_conn_error(exc)
         raise UnableToConnect(
             f"Cannot connect to any of the configured servers: {errors}"
         )
 
     @property
     def connection(self) -> BlockingConnection:
+        print("Connection...")
+        pprint(self.config)
         if self._connection is None or not self._connection.is_open:
-            self._connection = self._make_connection()
+            for attempt in Retrying(
+                retry=retry_if_exception_type((UnableToConnect, AMQPError, OSError)),
+                stop=stop_after_attempt(self.config.connection.attempts),
+                wait=wait_random(
+                    min=self.config.connection.wait_random_min_seconds,
+                    max=self.config.connection.wait_random_max_seconds,
+                ),
+                reraise=True,
+            ):
+                with attempt:
+                    self._connection = self._make_connection()
         return self._connection
 
     @typechecked
     def _open_channel(self) -> BlockingChannel:
         _channel = self.connection.channel()
         _channel.basic_qos(prefetch_count=1)
         return _channel
```

### Comparing `robotnikmq-0.4.1/robotnikmq/error.py` & `robotnikmq-0.5.0/robotnikmq/error.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/robotnikmq/log.py` & `robotnikmq-0.5.0/robotnikmq/log.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/robotnikmq/rpc_client.py` & `robotnikmq-0.5.0/robotnikmq/rpc_client.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/robotnikmq/rpc_server.py` & `robotnikmq-0.5.0/robotnikmq/rpc_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,245 +1,299 @@
 from inspect import signature, Parameter
-from json import loads as from_json
+from json import loads as _from_json
 from traceback import format_exc
 from socket import gethostname
 from typing import Optional, Callable, Union, Any, Dict, Tuple, List
 from typing import get_type_hints, get_origin, get_args
 from uuid import uuid4 as uuid, UUID
 
 from pika import BasicProperties
 from pika.exceptions import AMQPError, ChannelError, AMQPConnectionError
-from retry import retry
+from tenacity import retry, wait_exponential, retry_if_exception_type
 from typeguard import typechecked
 
 from robotnikmq.config import RobotnikConfig
 from robotnikmq.core import Robotnik, ConnErrorCallback, thread_name, valid_json
 from robotnikmq.log import log
-from robotnikmq.utils import to_json
+from robotnikmq.utils import to_json as _to_json
 
 
 @typechecked
 def _type_hint_str(typ: Any) -> str:
     if get_origin(typ) is Union:
         return f"Union[{','.join([_type_hint_str(t) for t in get_args(typ)])}]"
     return str(typ.__name__)
 
 
-class RpcError():
+class RpcError:
     @typechecked
-    def __init__(self, request_id: Union[str, UUID, None] = None,
-                 details: Union[None, str, Dict[str, Any]] = None):
+    def __init__(
+        self,
+        request_id: Union[str, UUID, None] = None,
+        details: Union[None, str, Dict[str, Any]] = None,
+    ):
         self.request_id = request_id or uuid()
         self.details = details
 
     @typechecked
     def to_json(self) -> str:
-        return to_json(self.to_dict())
+        return _to_json(self.to_dict())
 
     @typechecked
     def to_dict(self) -> Dict[str, Any]:
-        return {'request_id': str(self.request_id),
-                'type': 'error',
-                'details': self.details}
+        return {
+            "request_id": str(self.request_id),
+            "type": "error",
+            "details": self.details,
+        }
 
     @staticmethod
     @typechecked
-    def from_json(json_str: Union[str, bytes]) -> Optional['RpcError']:
+    def from_json(json_str: Union[str, bytes]) -> Optional["RpcError"]:
         json_str = json_str if isinstance(json_str, str) else json_str.decode()
         log.debug(json_str)
         if valid_json(json_str):
-            data = from_json(json_str)
-            if all(k in data for k in {'request_id', 'type', 'details'}):
-                return RpcError(request_id=data['request_id'],
-                                details=data['details'])
+            data = _from_json(json_str)
+            if all(k in data for k in {"request_id", "type", "details"}):
+                return RpcError(request_id=data["request_id"], details=data["details"])
         return None
 
 
-class RpcResponse():
+class RpcResponse:
     @typechecked
-    def __init__(self,
-                 request_id: Union[str, UUID, None] = None,
-                 data: Union[None, str, int, float, Dict[str, Any],
-                             List[Dict[str, Any]]] = None):
+    def __init__(
+        self,
+        request_id: Union[str, UUID, None] = None,
+        data: Union[None, str, int, float, Dict[str, Any], List[Dict[str, Any]]] = None,
+    ):
         self.request_id = request_id or uuid()
         self.data = data
 
     @typechecked
-    def to_json(self) -> str:
-        return to_json(self.to_dict())
+    def to_dict(self) -> Dict[str, Any]:
+        return {
+            "request_id": str(self.request_id),
+            "type": "response",
+            "data": self.data,
+        }
 
     @typechecked
-    def to_dict(self) -> Dict[str, Any]:
-        return {'request_id': str(self.request_id),
-                'type': 'response',
-                'data': self.data}
+    def to_json(self) -> str:
+        return _to_json(self.to_dict())
 
     @staticmethod
     @typechecked
-    def from_json(json_str: Union[str, bytes]) -> Optional['RpcResponse']:
+    def from_json(json_str: Union[str, bytes]) -> Optional["RpcResponse"]:
         json_str = json_str if isinstance(json_str, str) else json_str.decode()
         if valid_json(json_str):
-            data = from_json(json_str)
-            if all(k in data for k in {'request_id', 'type', 'data'}):
-                return RpcResponse(request_id=data['request_id'],
-                                   data=data['data'])
+            data = _from_json(json_str)
+            if all(k in data for k in {"request_id", "type", "data"}):
+                return RpcResponse(request_id=data["request_id"], data=data["data"])
         return None
 
 
 class RpcServer(Robotnik):
     @typechecked
-    def __init__(self, config: Optional[RobotnikConfig] = None,
-                 on_conn_error: ConnErrorCallback = None,
-                 meta_queue_prefix: Optional[str] = None,
-                 docs_queue_suffix: Optional[str] = None,
-                 only_once: bool = False):
+    def __init__(
+        self,
+        config: Optional[RobotnikConfig] = None,
+        on_conn_error: ConnErrorCallback = None,
+        meta_queue_prefix: Optional[str] = None,
+        docs_queue_suffix: Optional[str] = None,
+        only_once: bool = False,
+    ):
         super().__init__(config=config, on_conn_error=on_conn_error)
         self._callbacks: Dict[str, Callable] = {}
         self.meta_queue_prefix = meta_queue_prefix or gethostname()
-        self.docs_queue_suffix = docs_queue_suffix or '.__doc__'
+        self.docs_queue_suffix = docs_queue_suffix or ".__doc__"
         # Typically used for testing, implies server should stop after 1 response
         self.only_once = only_once
 
     @typechecked
     def _register_docs(self, queue: str, callback: Callable) -> None:
-        self.channel.queue_declare(queue=queue + self.docs_queue_suffix, exclusive=False)
+        self.channel.queue_declare(
+            queue=queue + self.docs_queue_suffix, exclusive=False
+        )
 
         @typechecked
         def docs_callback(_, method, props: BasicProperties, __) -> None:
             req_id = props.correlation_id or uuid()
-            response = RpcResponse(req_id,
-                                   data={'rpc_queue': queue,
-                                         'inputs': self._get_input_type_strings(queue),
-                                         'returns': self._get_return_type_str(queue),
-                                         'description': callback.__doc__})
-            self.channel.basic_publish(exchange='',
-                                       routing_key=props.reply_to,
-                                       properties=BasicProperties(
-                                        correlation_id=props.correlation_id),
-                                       body=response.to_json())
+            response = RpcResponse(
+                req_id,
+                data={
+                    "rpc_queue": queue,
+                    "inputs": self._get_input_type_strings(queue),
+                    "returns": self._get_return_type_str(queue),
+                    "description": callback.__doc__,
+                },
+            )
+            self.channel.basic_publish(
+                exchange="",
+                routing_key=props.reply_to,
+                properties=BasicProperties(correlation_id=props.correlation_id),
+                body=response.to_json(),
+            )
             self.channel.basic_ack(delivery_tag=method.delivery_tag)
 
-        self.channel.basic_consume(queue=queue + self.docs_queue_suffix,
-                                   on_message_callback=docs_callback,
-                                   auto_ack=False)
+        self.channel.basic_consume(
+            queue=queue + self.docs_queue_suffix,
+            on_message_callback=docs_callback,
+            auto_ack=False,
+        )
 
     @typechecked
     def _get_defaults(self, queue: str) -> Dict[str, Any]:
         params = signature(self._callbacks[queue]).parameters
-        return {p: params[p].default for p in params if params[p].default is not Parameter.empty}
+        return {
+            p: params[p].default
+            for p in params
+            if params[p].default is not Parameter.empty
+        }
 
     @typechecked
     def _get_input_types(self, queue: str) -> Dict[str, Any]:
-        return {k: v for k, v in get_type_hints(self._callbacks[queue]).items() if k != 'return'}
+        return {
+            k: v
+            for k, v in get_type_hints(self._callbacks[queue]).items()
+            if k != "return"
+        }
 
     @typechecked
     def _get_input_type_strings(self, queue: str) -> Dict[str, Any]:
-        return {k: _type_hint_str(v) for k, v in
-                get_type_hints(self._callbacks[queue]).items() if k != 'return'}
+        return {
+            k: _type_hint_str(v)
+            for k, v in get_type_hints(self._callbacks[queue]).items()
+            if k != "return"
+        }
 
     @typechecked
     def _get_return_type_str(self, queue: str) -> Any:
-        return _type_hint_str(get_type_hints(self._callbacks[queue])['return'])
+        return _type_hint_str(get_type_hints(self._callbacks[queue])["return"])
 
     @staticmethod
     @typechecked
     def _is_optional(arg_type: Any) -> bool:
         return get_origin(arg_type) is Union and type(None) in get_args(arg_type)
 
     @staticmethod
     @typechecked
     def _valid_arg(arg_value: Any, arg_type: Any) -> bool:
         if arg_type is Any:
             return True
         if get_origin(arg_type) is Union:
-            if (type(None) in get_args(arg_type)) and (arg_value is None or arg_value == {}):  # Optional
+            if (type(None) in get_args(arg_type)) and (
+                arg_value is None or arg_value == {}
+            ):  # Optional
                 return True
-            return any(RpcServer._valid_arg(arg_value, typ) for typ in get_args(arg_type))
+            return any(
+                RpcServer._valid_arg(arg_value, typ) for typ in get_args(arg_type)
+            )
         if get_origin(arg_type) is dict:
             key_type, val_type = get_args(arg_type)
-            return all(RpcServer._valid_arg(key, key_type) for key in arg_value.keys()) and \
-                all(RpcServer._valid_arg(val, val_type) for val in arg_value.values())
+            return all(
+                RpcServer._valid_arg(key, key_type) for key in arg_value.keys()
+            ) and all(RpcServer._valid_arg(val, val_type) for val in arg_value.values())
         return isinstance(arg_value, arg_type)
 
     @typechecked
-    def _valid_inputs(self, queue: str, inputs: Dict[str, Any]) -> Tuple[bool, Optional[str]]:
+    def _valid_inputs(
+        self, queue: str, inputs: Dict[str, Any]
+    ) -> Tuple[bool, Optional[str]]:
         inputs_with_defaults = {**self._get_defaults(queue), **inputs}
         for arg_name, arg_type in self._get_input_types(queue).items():
             if arg_name not in inputs_with_defaults and not self._is_optional(arg_type):
-                return False, f'Missing required argument {arg_name}'
-            if arg_name in inputs_with_defaults and not self._valid_arg(inputs_with_defaults[arg_name], arg_type):
-                return False, f'Invalid type for {arg_name}'
+                return False, f"Missing required argument {arg_name}"
+            if arg_name in inputs_with_defaults and not self._valid_arg(
+                inputs_with_defaults[arg_name], arg_type
+            ):
+                return False, f"Invalid type for {arg_name}"
         return True, None
 
     @typechecked
-    def register_rpc(self, queue: str,
-                     callback: Callable,
-                     register_docs: bool = True) -> None:
+    def register_rpc(
+        self, queue: str, callback: Callable, register_docs: bool = True
+    ) -> None:
         self.channel.queue_declare(queue=queue, exclusive=False)
         self._callbacks[queue] = callback
         if register_docs:
             self._register_docs(queue, callback)
         # TODO: servers should have an exclusive Queue for information about themselves
 
         @typechecked
         def meta_callback(_, method, props: BasicProperties, body: bytes):
             req_id = props.correlation_id or uuid()
             with thread_name(req_id):
-                log.debug('Request received')
+                log.debug("Request received")
                 try:
                     try:
                         if valid_json(body.decode()):
-                            input_args: Dict[str, Any] = from_json(body.decode())
-                            log.debug(f'Input JSON is valid: {input_args}')
+                            input_args: Dict[str, Any] = _from_json(body.decode())
+                            log.debug(f"Input JSON is valid: {input_args}")
                             valid_inputs, msg = self._valid_inputs(queue, input_args)
                             if not valid_inputs:
-                                log.debug('Invalid input')
+                                log.debug("Invalid input")
                                 response = RpcError(req_id, msg).to_json()
                             elif not input_args:
-                                log.debug(f'Executing: {callback}')
+                                log.debug(f"Executing: {callback}")
                                 response = RpcResponse(req_id, callback()).to_json()
                             else:
-                                log.debug(f'Executing: {callback} with inputs: {input_args}')
-                                response = RpcResponse(req_id, callback(**input_args)).to_json()
+                                log.debug(
+                                    f"Executing: {callback} with inputs: {input_args}"
+                                )
+                                response = RpcResponse(
+                                    req_id, callback(**input_args)
+                                ).to_json()
                         else:
-                            response = RpcError(req_id,
-                                                'Input could not be decoded as JSON').to_json()
+                            response = RpcError(
+                                req_id, "Input could not be decoded as JSON"
+                            ).to_json()
                     except (AMQPError, ChannelError):
                         raise  # we want this kind of exception to be caught further down
                     except Exception:  # pylint: disable=W0703
-                        log.error("An error has occurred during the execution of the RPC method")
-                        for line in format_exc().split('\n'):
+                        log.error(
+                            "An error has occurred during the execution of the RPC method"
+                        )
+                        for line in format_exc().split("\n"):
                             log.error(line)
-                        response = RpcError(request_id=req_id, details=f'There was an error '
-                                                                       f'while processing the '
-                                                                       f'request, please refer '
-                                                                       f'to server log with '
-                                                                       f'request ID: '
-                                                                       f'{req_id}').to_json()
-                    log.debug(f'Response: {response}')
-                    self.channel.basic_publish(exchange='',
-                                               routing_key=props.reply_to,
-                                               properties=BasicProperties(
-                                                correlation_id=props.correlation_id),
-                                               body=response)
+                        response = RpcError(
+                            request_id=req_id,
+                            details=f"There was an error "
+                            f"while processing the "
+                            f"request, please refer "
+                            f"to server log with "
+                            f"request ID: "
+                            f"{req_id}",
+                        ).to_json()
+                    log.debug(f"Response: {response}")
+                    self.channel.basic_publish(
+                        exchange="",
+                        routing_key=props.reply_to,
+                        properties=BasicProperties(correlation_id=props.correlation_id),
+                        body=response,
+                    )
                     self.channel.basic_ack(delivery_tag=method.delivery_tag)
-                    log.debug('Response sent and ack-ed')
+                    log.debug("Response sent and ack-ed")
                 except (AMQPError, ChannelError):
-                    log.error(f"A RabbitMQ communication error has occurred while processing "
-                              f"Request ID: {req_id}")
-                    for line in format_exc().split('\n'):
+                    log.error(
+                        f"A RabbitMQ communication error has occurred while processing "
+                        f"Request ID: {req_id}"
+                    )
+                    for line in format_exc().split("\n"):
                         log.error(line)
             if self.only_once:
                 self.channel.stop_consuming()
 
-        self.channel.basic_consume(queue=queue,
-                                   on_message_callback=meta_callback,
-                                   auto_ack=False)
-
-    @retry(AMQPConnectionError, delay=2, jitter=1)
+        self.channel.basic_consume(
+            queue=queue, on_message_callback=meta_callback, auto_ack=False
+        )
+
+    @retry(
+        retry=retry_if_exception_type((AMQPConnectionError, OSError)),
+        wait=wait_exponential(multiplier=1, min=3, max=30),
+    )
     @typechecked
     def run(self) -> None:
         try:
             self.channel.start_consuming()
         except KeyboardInterrupt:
             self.channel.stop_consuming()
             log.info("Shutting down server")
```

### Comparing `robotnikmq-0.4.1/robotnikmq/subscriber.py` & `robotnikmq-0.5.0/robotnikmq/subscriber.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,111 @@
 from collections import namedtuple
 from traceback import format_exc
 from typing import Optional, Callable, List, Generator
 
-from pika.exceptions import AMQPConnectionError
-from retry import retry
+from pika.exceptions import AMQPError
+from tenacity import retry, wait_exponential, retry_if_exception_type
 from typeguard import typechecked
 
 from robotnikmq.config import RobotnikConfig
 from robotnikmq.core import Robotnik, ConnErrorCallback, Message
 from robotnikmq.error import MalformedMessage
 from robotnikmq.log import log
 
 OnMessageCallback = Callable[[Message], None]
 
-ExchangeBinding = namedtuple('ExchangeBinding', ['exchange', 'binding_key'])
+ExchangeBinding = namedtuple("ExchangeBinding", ["exchange", "binding_key"])
 
 
 class Subscriber(Robotnik):
     @typechecked
-    def __init__(self,
-                 exchange_bindings: Optional[List[ExchangeBinding]] = None,
-                 config: Optional[RobotnikConfig] = None,
-                 on_conn_error: ConnErrorCallback = None):
+    def __init__(
+        self,
+        exchange_bindings: Optional[List[ExchangeBinding]] = None,
+        config: Optional[RobotnikConfig] = None,
+        on_conn_error: ConnErrorCallback = None,
+    ):
         super().__init__(config=config, on_conn_error=on_conn_error)
         self.exchange_bindings = exchange_bindings or []
         self._halted = True
 
     @typechecked
-    def _bind(self, exchange_binding: ExchangeBinding) -> 'Subscriber':
+    def _bind(self, exchange_binding: ExchangeBinding) -> "Subscriber":
         self.exchange_bindings.append(exchange_binding)
         return self
 
     @typechecked
-    def bind(self, exchange: str, binding_key: str = '#') -> 'Subscriber':
+    def bind(self, exchange: str, binding_key: str = "#") -> "Subscriber":
         return self._bind(ExchangeBinding(exchange, binding_key))
 
     @typechecked
     def stop(self) -> None:
         self._halted = True
 
-    @retry(AMQPConnectionError, delay=2, jitter=1)
-    @typechecked
-    def run(self, callback: OnMessageCallback, inactivity_timeout: Optional[float] = None) -> None:
+    @retry(
+        retry=retry_if_exception_type((AMQPError, OSError)),
+        wait=wait_exponential(multiplier=1, min=3, max=30),
+    )
+    @typechecked
+    def run(
+        self, callback: OnMessageCallback, inactivity_timeout: Optional[float] = None
+    ) -> None:
         self._halted = False
         while not self._halted:
             with self.open_channel() as channel:
-                queue_name = channel.queue_declare(queue='', exclusive=True).method.queue
+                queue_name = channel.queue_declare(
+                    queue="", exclusive=True
+                ).method.queue
                 for ex_b in self.exchange_bindings:
-                    channel.exchange_declare(exchange=ex_b.exchange,
-                                             exchange_type='topic',
-                                             auto_delete=True)
-                    channel.queue_bind(exchange=ex_b.exchange,
-                                       queue=queue_name,
-                                       routing_key=ex_b.binding_key)
-                for method, ___, body in channel.consume(queue=queue_name,  # pragma: no cover
-                                                         auto_ack=False,
-                                                         inactivity_timeout=inactivity_timeout):
+                    channel.exchange_declare(
+                        exchange=ex_b.exchange, exchange_type="topic", auto_delete=True
+                    )
+                    channel.queue_bind(
+                        exchange=ex_b.exchange,
+                        queue=queue_name,
+                        routing_key=ex_b.binding_key,
+                    )
+                for method, ___, body in channel.consume(
+                    queue=queue_name,  # pragma: no cover
+                    auto_ack=False,
+                    inactivity_timeout=inactivity_timeout,
+                ):
                     if method and body:
                         callback(Message.of(body.decode()))
                         channel.basic_ack(delivery_tag=method.delivery_tag)
                     if self._halted:
                         break
                 channel.cancel()
                 self.close_channel(channel)
 
-    @retry(AMQPConnectionError, delay=2, jitter=1)
-    @typechecked
-    def consume(self, inactivity_timeout: Optional[float] = None) -> Generator[Optional[Message],
-                                                                               None, None]:
+    @retry(
+        retry=retry_if_exception_type((AMQPError, OSError)),
+        wait=wait_exponential(multiplier=1, min=3, max=30),
+    )
+    @typechecked
+    def consume(
+        self, inactivity_timeout: Optional[float] = None
+    ) -> Generator[Optional[Message], None, None]:
         with self.open_channel() as channel:
-            queue_name = channel.queue_declare(queue='', exclusive=True).method.queue
+            queue_name = channel.queue_declare(queue="", exclusive=True).method.queue
             for ex_b in self.exchange_bindings:
-                channel.exchange_declare(exchange=ex_b.exchange,
-                                         exchange_type='topic',
-                                         auto_delete=True)
-                channel.queue_bind(exchange=ex_b.exchange,
-                                   queue=queue_name,
-                                   routing_key=ex_b.binding_key)
+                channel.exchange_declare(
+                    exchange=ex_b.exchange, exchange_type="topic", auto_delete=True
+                )
+                channel.queue_bind(
+                    exchange=ex_b.exchange,
+                    queue=queue_name,
+                    routing_key=ex_b.binding_key,
+                )
             try:
-                for method, ___, body in channel.consume(queue=queue_name,  # pragma: no cover
-                                                         auto_ack=False,
-                                                         inactivity_timeout=inactivity_timeout):
+                for method, ___, body in channel.consume(
+                    queue=queue_name,  # pragma: no cover
+                    auto_ack=False,
+                    inactivity_timeout=inactivity_timeout,
+                ):
                     if method and body:
                         channel.basic_ack(delivery_tag=method.delivery_tag)
                         try:
                             yield Message.of(body.decode())
                         except MalformedMessage:
                             log.debug(format_exc())
                     else:
```

### Comparing `robotnikmq-0.4.1/robotnikmq/topic.py` & `robotnikmq-0.5.0/robotnikmq/topic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,44 @@
 import json
 from typing import Optional
 
+from pika.exceptions import AMQPError
+from tenacity import retry, retry_if_exception_type, wait_exponential
 from typeguard import typechecked
 
 from robotnikmq.config import RobotnikConfig
 from robotnikmq.core import Robotnik, Message, ConnErrorCallback, AMQPErrorCallback
 from robotnikmq.log import log
 
 
 class Topic(Robotnik):
     @typechecked
-    def __init__(self, exchange: str,
-                 config: Optional[RobotnikConfig] = None,
-                 on_conn_error: ConnErrorCallback = None):
+    def __init__(
+        self,
+        exchange: str,
+        config: Optional[RobotnikConfig] = None,
+        on_conn_error: ConnErrorCallback = None,
+    ):
         super().__init__(config=config, on_conn_error=on_conn_error)
         self.exchange = exchange
-        self.channel.exchange_declare(exchange=self.exchange,
-                                      exchange_type='topic',
-                                      auto_delete=True)
+        self.channel.exchange_declare(
+            exchange=self.exchange, exchange_type="topic", auto_delete=True
+        )
 
+    @retry(
+        retry=retry_if_exception_type((AMQPError, OSError)),
+        wait=wait_exponential(multiplier=1, min=3, max=30),
+    )
     @typechecked
-    def broadcast(self, msg: Message,
-                  routing_key: Optional[str] = None,
-                  on_msg_error: AMQPErrorCallback = None) -> None:
+    def broadcast(
+        self,
+        msg: Message,
+        routing_key: Optional[str] = None,
+        on_msg_error: AMQPErrorCallback = None,
+    ) -> None:
         msg.routing_key = routing_key or msg.routing_key
-        self.channel.basic_publish(exchange=self.exchange,
-                                   routing_key=(routing_key or msg.routing_key or ''),
-                                   body=json.dumps(msg.to_dict()))
-        log.debug(f'Broadcast: \n{json.dumps(msg.to_dict(), indent=4)}')
+        self.channel.basic_publish(
+            exchange=self.exchange,
+            routing_key=(routing_key or msg.routing_key or ""),
+            body=json.dumps(msg.to_dict()),
+        )
+        log.debug(f"Broadcast: \n{json.dumps(msg.to_dict(), indent=4)}")
```

### Comparing `robotnikmq-0.4.1/tests/integration/test_broadcast.py` & `robotnikmq-0.5.0/tests/integration/test_broadcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 from robotnikmq.core import Message
 from robotnikmq.error import UnableToConnect
 from robotnikmq.log import log
 from robotnikmq.subscriber import Subscriber
 from robotnikmq.topic import Topic
 
 from tests.integration.utils import META_QUEUE
-from tests.integration.utils import robotnikmq_config  # pylint: disable=W0611
+from tests.integration.utils import (
+    conn_config,
+    robotnikmq_config,
+)  # pylint: disable=W0611
 
 
 try:
     from pytest_cov.embed import cleanup_on_sigterm  # type: ignore
 except ImportError:
     pass
 else:
@@ -34,38 +37,40 @@
         on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
     )
     medium.broadcast(Message({"stuff": "Hello world!"}))
 
 
 def test_unable_to_connect():
     config = RobotnikConfig(
+        connection=conn_config(1, 1, 2),
         tiers=[
             [
                 server_config("127.0.0.1", 1, "", "", ""),
                 server_config("127.0.0.2", 1, "1", "1", "1"),
             ]
-        ]
+        ],
     )
     with raises(UnableToConnect):
         medium = Topic(
             META_QUEUE,
             config,
             on_conn_error=lambda a: print(f"Could not connect (callback): {a.args}"),
         )
         medium.broadcast(Message({"stuff": "Hello world!"}))
 
 
 def test_unable_to_connect_without_callback():
     config = RobotnikConfig(
+        connection=conn_config(1, 1, 2),
         tiers=[
             [
                 server_config("127.0.0.1", 1, "", "", ""),
                 server_config("127.0.0.2", 1, "1", "1", "1"),
             ]
-        ]
+        ],
     )
     with raises(UnableToConnect) as exc:
         medium = Topic(META_QUEUE, config)
         medium.broadcast(Message({"stuff": "Hello world!"}))
     log.debug(str(exc))
     log.debug(str(exc.value.__str__()))
```

### Comparing `robotnikmq-0.4.1/tests/integration/test_rpc.py` & `robotnikmq-0.5.0/tests/integration/test_rpc.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/utils.py` & `robotnikmq-0.5.0/tests/integration/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from contextlib import contextmanager
 from multiprocessing import Process
+from pprint import pprint
 from subprocess import run
 from time import sleep
 from typing import Callable, Any, Tuple, Optional
 
+from pytest_rabbitmq import factories
+
 # pylint: disable=E0401
 from pytest_rabbitmq.factories.executor import RabbitMqExecutor  # type: ignore
 
 # pylint: enable=E0401
 from pytest import fixture
 
-from robotnikmq.config import server_config, RobotnikConfig
-
+from robotnikmq.config import server_config, RobotnikConfig, conn_config
 
 USERNAME = "robotnik"
 PASSWORD = "hackme"
 VIRTUAL_HOST = "/robotnik"
 
 META_QUEUE = "skynet.legion"
 
@@ -78,17 +80,36 @@
             ".*",
             ".*",
         ],
         check=False,
     )
 
 
+def config_for(
+    proc: RabbitMqExecutor, attempts: int = 1, min_wait: int = 1, max_wait: int = 2
+) -> RobotnikConfig:
+    print("Configuration fixture...")
+    pprint(
+        RobotnikConfig(
+            connection=conn_config(attempts, min_wait, max_wait),
+            tiers=[
+                [server_config(proc.host, proc.port, USERNAME, PASSWORD, VIRTUAL_HOST)]
+            ],
+        )
+    )
+    return RobotnikConfig(
+        connection=conn_config(attempts, min_wait, max_wait),
+        tiers=[[server_config(proc.host, proc.port, USERNAME, PASSWORD, VIRTUAL_HOST)]],
+    )
+
+
 @fixture(scope="module")
 def robotnikmq_config(rabbitmq_proc):
     initialize_rabbitmq(rabbitmq_proc)
     return config_for(rabbitmq_proc)
 
 
-def config_for(proc: RabbitMqExecutor) -> RobotnikConfig:
-    return RobotnikConfig(
-        tiers=[[server_config(proc.host, proc.port, USERNAME, PASSWORD, VIRTUAL_HOST)]]
-    )
+@fixture(scope="module")
+def robotnikmq():
+    robotnikmq_proc = factories.rabbitmq_proc(port=8888)
+    initialize_rabbitmq(robotnikmq_proc)
+    return robotnikmq_proc
```

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/library/ca.py` & `robotnikmq-0.5.0/tests/integration/vagrant/library/ca.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/library/cert.py` & `robotnikmq-0.5.0/tests/integration/vagrant/library/cert.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/provision.yaml` & `robotnikmq-0.5.0/tests/integration/vagrant/provision.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml` & `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml` & `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml` & `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2` & `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2` & `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/integration/vagrant/roles/tls/tasks/tls.yaml` & `robotnikmq-0.5.0/tests/integration/vagrant/roles/tls/tasks/tls.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/unit/test_config.py` & `robotnikmq-0.5.0/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/unit/test_message.py` & `robotnikmq-0.5.0/tests/unit/test_message.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/tests/unit/test_validation.py` & `robotnikmq-0.5.0/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.4.1/PKG-INFO` & `robotnikmq-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotnikmq
-Version: 0.4.1
+Version: 0.5.0
 Summary: Utilities for safe, efficient, and scalable infrastructure using RabbitMQ
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >3.8.2
 Description-Content-Type: text/markdown
 
 # RobotnikMQ
```

