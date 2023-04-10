# Comparing `tmp/robotnikmq-0.5.0.tar.gz` & `tmp/robotnikmq-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotnikmq-0.5.0.tar", last modified: Mon Apr 10 22:43:32 2023, max compression
+gzip compressed data, was "robotnikmq-0.5.1.tar", last modified: Mon Apr 10 23:01:26 2023, max compression
```

## Comparing `robotnikmq-0.5.0.tar` & `robotnikmq-0.5.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    34500 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/LICENSE
--rw-r--r--   0        0        0     6369 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/README.md
--rw-r--r--   0        0        0     1212 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0      320 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/robotnikmq/__init__.py
--rwxr-xr-x   0        0        0     5330 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/config.py
--rw-r--r--   0        0        0     6363 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/core.py
--rwxr-xr-x   0        0        0      652 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/robotnikmq/error.py
--rw-r--r--   0        0        0     1230 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/robotnikmq/log.py
--rw-r--r--   0        0        0     2649 2022-11-16 02:41:34.714029 robotnikmq-0.5.0/robotnikmq/rpc_client.py
--rw-r--r--   0        0        0    11552 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/rpc_server.py
--rw-r--r--   0        0        0     4359 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/subscriber.py
--rwxr-xr-x   0        0        0     1411 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/robotnikmq/topic.py
--rw-r--r--   0        0        0      471 2023-04-10 14:34:22.584553 robotnikmq-0.5.0/robotnikmq/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 14:11:18.502194 robotnikmq-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 14:11:20.222199 robotnikmq-0.5.0/tests/integration/__init__.py
--rwxr-xr-x   0        0        0    16298 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/tests/integration/test_broadcast.py
--rw-r--r--   0        0        0     1632 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/tests/integration/test_disconnects.py
--rw-r--r--   0        0        0    13648 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/test_rpc.py
--rw-r--r--   0        0        0     2740 2023-04-10 22:43:27.085734 robotnikmq-0.5.0/tests/integration/utils.py
--rw-r--r--   0        0        0    13754 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/library/ca.py
--rw-r--r--   0        0        0    12451 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/library/cert.py
--rw-r--r--   0        0        0      739 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/provision.yaml
--rw-r--r--   0        0        0       84 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/handlers/main.yaml
--rw-r--r--   0        0        0       19 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/meta/main.yaml
--rw-r--r--   0        0        0      102 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/main.yaml
--rw-r--r--   0        0        0     1609 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml
--rw-r--r--   0        0        0     4907 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml
--rwxr-xr-x   0        0        0      588 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml
--rw-r--r--   0        0        0     1236 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2
--rw-r--r--   0        0        0     1012 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2
--rw-r--r--   0        0        0       29 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/tls/tasks/main.yaml
--rw-r--r--   0        0        0     2522 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/roles/tls/tasks/tls.yaml
--rw-r--r--   0        0        0      172 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/integration/vagrant/testing
--rw-r--r--   0        0        0        0 2023-04-10 14:11:21.330203 robotnikmq-0.5.0/tests/unit/__init__.py
--rw-r--r--   0        0        0     4142 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/unit/test_config.py
--rw-r--r--   0        0        0      261 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/unit/test_error.py
--rw-r--r--   0        0        0     1818 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/unit/test_message.py
--rw-r--r--   0        0        0     1292 2022-11-16 02:41:34.718029 robotnikmq-0.5.0/tests/unit/test_validation.py
--rw-r--r--   0        0        0     6652 1970-01-01 00:00:00.000000 robotnikmq-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/LICENSE
+-rw-r--r--   0        0        0     6369 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/README.md
+-rw-r--r--   0        0        0     1217 2023-04-10 22:57:32.564447 robotnikmq-0.5.1/pyproject.toml
+-rwxr-xr-x   0        0        0      320 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/robotnikmq/__init__.py
+-rwxr-xr-x   0        0        0     5330 2023-04-10 22:43:27.085734 robotnikmq-0.5.1/robotnikmq/config.py
+-rw-r--r--   0        0        0     6278 2023-04-10 22:59:06.907684 robotnikmq-0.5.1/robotnikmq/core.py
+-rwxr-xr-x   0        0        0      652 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/robotnikmq/error.py
+-rw-r--r--   0        0        0     1230 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/robotnikmq/log.py
+-rw-r--r--   0        0        0     2649 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/robotnikmq/rpc_client.py
+-rw-r--r--   0        0        0    11552 2023-04-10 22:43:27.085734 robotnikmq-0.5.1/robotnikmq/rpc_server.py
+-rw-r--r--   0        0        0     4359 2023-04-10 23:00:12.499144 robotnikmq-0.5.1/robotnikmq/subscriber.py
+-rwxr-xr-x   0        0        0     1411 2023-04-10 22:43:27.085734 robotnikmq-0.5.1/robotnikmq/topic.py
+-rw-r--r--   0        0        0      471 2023-04-10 14:34:22.584553 robotnikmq-0.5.1/robotnikmq/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:18.502194 robotnikmq-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:20.222199 robotnikmq-0.5.1/tests/integration/__init__.py
+-rwxr-xr-x   0        0        0    16298 2023-04-10 23:00:46.078865 robotnikmq-0.5.1/tests/integration/test_broadcast.py
+-rw-r--r--   0        0        0     1632 2023-04-10 22:43:27.085734 robotnikmq-0.5.1/tests/integration/test_disconnects.py
+-rw-r--r--   0        0        0    13648 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/test_rpc.py
+-rw-r--r--   0        0        0     2435 2023-04-10 23:00:31.458987 robotnikmq-0.5.1/tests/integration/utils.py
+-rw-r--r--   0        0        0    13754 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/library/ca.py
+-rw-r--r--   0        0        0    12451 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/library/cert.py
+-rw-r--r--   0        0        0      739 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/provision.yaml
+-rw-r--r--   0        0        0       84 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/handlers/main.yaml
+-rw-r--r--   0        0        0       19 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/meta/main.yaml
+-rw-r--r--   0        0        0      102 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/main.yaml
+-rw-r--r--   0        0        0     1609 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml
+-rw-r--r--   0        0        0     4907 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml
+-rwxr-xr-x   0        0        0      588 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml
+-rw-r--r--   0        0        0     1236 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2
+-rw-r--r--   0        0        0     1012 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2
+-rw-r--r--   0        0        0       29 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/tls/tasks/main.yaml
+-rw-r--r--   0        0        0     2522 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/tls/tasks/tls.yaml
+-rw-r--r--   0        0        0      172 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/testing
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:21.330203 robotnikmq-0.5.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4142 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/unit/test_config.py
+-rw-r--r--   0        0        0      261 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/unit/test_error.py
+-rw-r--r--   0        0        0     1818 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/unit/test_message.py
+-rw-r--r--   0        0        0     1292 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/unit/test_validation.py
+-rw-r--r--   0        0        0     6657 1970-01-01 00:00:00.000000 robotnikmq-0.5.1/PKG-INFO
```

### Comparing `robotnikmq-0.5.0/LICENSE` & `robotnikmq-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/README.md` & `robotnikmq-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/pyproject.toml` & `robotnikmq-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "robotnikmq"
-version = "0.5.0"
+version = "0.5.1"
 description = "Utilities for safe, efficient, and scalable infrastructure using RabbitMQ"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
     "typeguard>=3.0.2",
     "pyyaml>=6.0",
@@ -14,15 +14,15 @@
     "arrow>=1.2.3",
     "logzero>=1.7.0",
     "types-pika>=1.2.0b1",
     "types-pyyaml>=6.0.11",
     "typing-extensions>=4.5.0",
     "tenacity>=8.2.2",
 ]
-requires-python = ">3.8.2"
+requires-python = ">3.8.2,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.optional-dependencies]
```

### Comparing `robotnikmq-0.5.0/robotnikmq/config.py` & `robotnikmq-0.5.1/robotnikmq/config.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/robotnikmq/core.py` & `robotnikmq-0.5.1/robotnikmq/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from contextlib import contextmanager
 from datetime import datetime
 from json import loads as _from_json
 from json.decoder import JSONDecodeError
 from pathlib import Path
-from pprint import pprint
 from random import sample
 from ssl import SSLError
 from threading import current_thread
 from typing import Optional, Callable, Any, Dict, Union, Generator, List
 from uuid import uuid4 as uuid, UUID
 
 from arrow import Arrow, get as to_arrow, now
@@ -154,16 +153,14 @@
                         self._on_conn_error(exc)
         raise UnableToConnect(
             f"Cannot connect to any of the configured servers: {errors}"
         )
 
     @property
     def connection(self) -> BlockingConnection:
-        print("Connection...")
-        pprint(self.config)
         if self._connection is None or not self._connection.is_open:
             for attempt in Retrying(
                 retry=retry_if_exception_type((UnableToConnect, AMQPError, OSError)),
                 stop=stop_after_attempt(self.config.connection.attempts),
                 wait=wait_random(
                     min=self.config.connection.wait_random_min_seconds,
                     max=self.config.connection.wait_random_max_seconds,
```

### Comparing `robotnikmq-0.5.0/robotnikmq/error.py` & `robotnikmq-0.5.1/robotnikmq/error.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/robotnikmq/log.py` & `robotnikmq-0.5.1/robotnikmq/log.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/robotnikmq/rpc_client.py` & `robotnikmq-0.5.1/robotnikmq/rpc_client.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/robotnikmq/rpc_server.py` & `robotnikmq-0.5.1/robotnikmq/rpc_server.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/robotnikmq/subscriber.py` & `robotnikmq-0.5.1/robotnikmq/subscriber.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/robotnikmq/topic.py` & `robotnikmq-0.5.1/robotnikmq/topic.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/test_broadcast.py` & `robotnikmq-0.5.1/tests/integration/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/test_disconnects.py` & `robotnikmq-0.5.1/tests/integration/test_disconnects.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/test_rpc.py` & `robotnikmq-0.5.1/tests/integration/test_rpc.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/utils.py` & `robotnikmq-0.5.1/tests/integration/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from contextlib import contextmanager
 from multiprocessing import Process
-from pprint import pprint
 from subprocess import run
 from time import sleep
 from typing import Callable, Any, Tuple, Optional
 
 from pytest_rabbitmq import factories
 
 # pylint: disable=E0401
@@ -83,23 +82,14 @@
         check=False,
     )
 
 
 def config_for(
     proc: RabbitMqExecutor, attempts: int = 1, min_wait: int = 1, max_wait: int = 2
 ) -> RobotnikConfig:
-    print("Configuration fixture...")
-    pprint(
-        RobotnikConfig(
-            connection=conn_config(attempts, min_wait, max_wait),
-            tiers=[
-                [server_config(proc.host, proc.port, USERNAME, PASSWORD, VIRTUAL_HOST)]
-            ],
-        )
-    )
     return RobotnikConfig(
         connection=conn_config(attempts, min_wait, max_wait),
         tiers=[[server_config(proc.host, proc.port, USERNAME, PASSWORD, VIRTUAL_HOST)]],
     )
 
 
 @fixture(scope="module")
```

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/library/ca.py` & `robotnikmq-0.5.1/tests/integration/vagrant/library/ca.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/library/cert.py` & `robotnikmq-0.5.1/tests/integration/vagrant/library/cert.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/provision.yaml` & `robotnikmq-0.5.1/tests/integration/vagrant/provision.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml` & `robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml` & `robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml` & `robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2` & `robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2` & `robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/integration/vagrant/roles/tls/tasks/tls.yaml` & `robotnikmq-0.5.1/tests/integration/vagrant/roles/tls/tasks/tls.yaml`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/unit/test_config.py` & `robotnikmq-0.5.1/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/unit/test_message.py` & `robotnikmq-0.5.1/tests/unit/test_message.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/tests/unit/test_validation.py` & `robotnikmq-0.5.1/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.0/PKG-INFO` & `robotnikmq-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: robotnikmq
-Version: 0.5.0
+Version: 0.5.1
 Summary: Utilities for safe, efficient, and scalable infrastructure using RabbitMQ
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
-Requires-Python: >3.8.2
+Requires-Python: >3.8.2,<4.0
 Description-Content-Type: text/markdown
 
 # RobotnikMQ
 
 Utilities for safe, efficient, and scalable infrastructure using RabbitMQ
 
 ## Usage
```

