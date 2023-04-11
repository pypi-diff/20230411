# Comparing `tmp/zimran-events-0.2.0.tar.gz` & `tmp/zimran-events-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.2.0.tar", last modified: Tue Apr 11 11:22:24 2023, max compression
+gzip compressed data, was "zimran-events-0.2.1.tar", last modified: Tue Apr 11 17:39:15 2023, max compression
```

## Comparing `zimran-events-0.2.0.tar` & `zimran-events-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:22:24.946443 zimran-events-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:22:24.942443 zimran-events-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:22:24.942443 zimran-events-0.2.0/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:22:24.942443 zimran-events-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-11 11:22:15.000000 zimran-events-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 11:22:15.000000 zimran-events-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 11:22:24.946443 zimran-events-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 11:22:15.000000 zimran-events-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-11 11:22:15.000000 zimran-events-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 11:22:15.000000 zimran-events-0.2.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 11:22:24.946443 zimran-events-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:22:24.942443 zimran-events-0.2.0/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:22:24.946443 zimran-events-0.2.0/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 11:22:15.000000 zimran-events-0.2.0/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-11 11:22:15.000000 zimran-events-0.2.0/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 11:22:15.000000 zimran-events-0.2.0/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5077 2023-04-11 11:22:15.000000 zimran-events-0.2.0/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 11:22:15.000000 zimran-events-0.2.0/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-11 11:22:15.000000 zimran-events-0.2.0/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-11 11:22:15.000000 zimran-events-0.2.0/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-11 11:22:15.000000 zimran-events-0.2.0/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 11:22:24.946443 zimran-events-0.2.0/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 11:22:24.000000 zimran-events-0.2.0/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 11:22:24.000000 zimran-events-0.2.0/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 11:22:24.000000 zimran-events-0.2.0/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-11 11:22:24.000000 zimran-events-0.2.0/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 11:22:24.000000 zimran-events-0.2.0/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.165491 zimran-events-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 17:39:06.000000 zimran-events-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 17:39:15.165491 zimran-events-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 17:39:06.000000 zimran-events-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 17:39:06.000000 zimran-events-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 17:39:06.000000 zimran-events-0.2.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:39:15.165491 zimran-events-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.165491 zimran-events-0.2.1/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.2.0/.github/scripts/release.py` & `zimran-events-0.2.1/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.0/.gitignore` & `zimran-events-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.0/.pre-commit-config.yaml` & `zimran-events-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.0/LICENSE` & `zimran-events-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.0/PKG-INFO` & `zimran-events-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.0
+Version: 0.2.1
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.0/README.md` & `zimran-events-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.0/pyproject.toml` & `zimran-events-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
 
-dependencies = ["pika>=1.3.1", "aio-pika>=9.0.5"]
+dependencies = ["pika>=1.3.1", "aio-pika>=9.0.5", "aioretry>=5.0.2"]
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
```

### Comparing `zimran-events-0.2.0/zimran/events/connection.py` & `zimran-events-0.2.1/zimran/events/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import asyncio
 
 import aio_pika
 import pika
+from aioretry import retry
+
+from zimran.events.utils import retry_policy
 
 
 try:
     from loguru import logger
 except ImportError:
     import logging
 
@@ -85,14 +88,15 @@
     async def channel(self):
         if self._channel is None or self._channel.is_closed:
             self._channel = await (await self.connection).channel(channel_number=self._channel_number)
             logger.info('Channel connection established')
 
         return self._channel
 
+    @retry(retry_policy)
     async def connect(self):
         self._channel = await (await self.connection).channel(channel_number=self._channel_number)
         logger.info('Channel connection established')
 
     async def disconnect(self):
         if self._channel is not None and not self._channel.is_closed:
             await self._channel.close()
```

### Comparing `zimran-events-0.2.0/zimran/events/consumer.py` & `zimran-events-0.2.1/zimran/events/consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import asyncio
 
 import aio_pika
+from aioretry import retry
 
 
 try:
     from loguru import logger
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
 
 from zimran.events.connection import AsyncConnection, Connection
 from zimran.events.constants import UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
 from zimran.events.schemas import ExchangeScheme
-from zimran.events.utils import validate_exchange
+from zimran.events.utils import cleanup_and_normalize_queue_name, retry_policy, validate_exchange
 
 
 class ConsumerMixin:
     def handle_event(self, name: str, *, exchange: ExchangeScheme | None = None):
         if exchange is not None:
             validate_exchange(exchange)
 
@@ -59,16 +60,16 @@
         try:
             self.channel.basic_qos(prefetch_count=self._prefetch_count)
 
             self._declare_unroutable_exchange()
 
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
-                queue_result = self.channel.queue_declare(f'{self._service_name}_{event_name}_q')
-                queue_name = queue_result.method.queue
+                queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
+                self.channel.queue_declare(queue_name, durable=True)
 
                 if exchange := data['exchange']:
                     self.channel.exchange_declare(
                         exchange=exchange.name,
                         exchange_type=exchange.type,
                         **exchange.as_dict(exclude=['name', 'type', 'timeout']),
                     )
@@ -77,15 +78,15 @@
                 self.channel.basic_consume(queue_name, data['handler'])
                 logger.info(f'Registering consumer | queue: {queue_name} | routing_key: {event_name}')
                 consumer_amount += 1
 
             logger.info(f'Registered {consumer_amount} consumers')
             self.channel.start_consuming()
         except Exception as exc:
-            logger.error(f'Exception occured | error: {exc}')
+            logger.error(f'Exception occured | error: {exc} | type: {type(exc)}')
         finally:
             self.disconnect()
 
     def _declare_unroutable_exchange(self):
         self.channel.exchange_declare(exchange=UNROUTABLE_EXCHANGE_NAME, exchange_type='fanout', durable=True)
         self.channel.queue_declare(queue=UNROUTABLE_QUEUE_NAME, durable=True)
         self.channel.queue_bind(queue=UNROUTABLE_QUEUE_NAME, exchange=UNROUTABLE_EXCHANGE_NAME, routing_key='')
@@ -106,36 +107,39 @@
         super().__init__(broker_url=broker_url, loop=loop, channel_number=channel_number)
 
         self._service_name = service_name
         self._prefetch_count = prefetch_count
 
         self._event_handlers = {}
 
+    @retry(retry_policy)
     async def run(self):
         try:
             channel = await self.channel
-            tasks = [self._declare_unroutable_queue(), channel.set_qos(prefetch_count=self._prefetch_count)]
+            tasks = [self._declare_unroutable_queue(channel), channel.set_qos(prefetch_count=self._prefetch_count)]
             await asyncio.gather(*tasks)
 
             consumer_amount = 0
             for event_name, data in self._event_handlers.items():
-                queue = await channel.declare_queue(f'{self._service_name}_{event_name}_q', exclusive=True)
+                queue_name = cleanup_and_normalize_queue_name(f'{self._service_name}.{event_name}')
+                queue = await channel.declare_queue(queue_name, durable=True)
                 if _exchange := data['exchange']:
                     exchange = await channel.declare_exchange(**_exchange.as_dict(exclude_none=True))
                     await queue.bind(exchange=exchange, routing_key=event_name)
 
                 await queue.consume(data['handler'])
 
-                logger.info(f'Registering consumer | queue: {queue.name} | routing_key: {event_name}')
+                logger.info(f'Registering consumer | queue: {queue_name} | routing_key: {event_name}')
                 consumer_amount += 1
 
             logger.info(f'Registered {consumer_amount} consumers')
             await asyncio.Future()
         except Exception as exc:
             logger.error(f'Exception occured | error: {exc}')
+            raise exc
         finally:
             await self.disconnect()
 
     async def _declare_unroutable_queue(self, channel: aio_pika.abc.AbstractRobustChannel):
         exchange = await channel.declare_exchange(name=UNROUTABLE_EXCHANGE_NAME, type='fanout', durable=True)
         queue = await channel.declare_queue(name=UNROUTABLE_QUEUE_NAME, durable=True)
         await queue.bind(exchange=exchange, routing_key='')
```

### Comparing `zimran-events-0.2.0/zimran/events/producer.py` & `zimran-events-0.2.1/zimran/events/producer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import json
 
 import aio_pika
+from aioretry import retry
 
 
 try:
     from loguru import logger
 except ImportError:
     import logging
 
     logger = logging.getLogger(__name__)
 
 
-from zimran.events.connection import AsyncConnection, Connection
-from zimran.events.constants import UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
-from zimran.events.schemas import ContextScheme
-from zimran.events.utils import validate_context, validate_exchange
+from .connection import AsyncConnection, Connection
+from .constants import UNROUTABLE_EXCHANGE_NAME, UNROUTABLE_QUEUE_NAME
+from .schemas import ContextScheme
+from .utils import retry_policy, validate_context, validate_exchange
 
 
 class Producer(Connection):
     def __init__(self, *, broker_url: str, channel_number: int = 1):
         super().__init__(broker_url=broker_url, channel_number=channel_number)
 
     def publish(self, routing_key: str, *, payload: dict, context: ContextScheme | None = None):
@@ -51,14 +52,15 @@
         self.channel.queue_bind(queue=UNROUTABLE_QUEUE_NAME, exchange=UNROUTABLE_EXCHANGE_NAME, routing_key='')
 
 
 class AsyncProducer(AsyncConnection):
     def __init__(self, *, broker_url: str, channel_number: int = 1):
         super().__init__(broker_url=broker_url, channel_number=channel_number)
 
+    @retry(retry_policy)
     async def publish(self, routing_key: str, *, payload: dict, context: ContextScheme | None = None):
         if context is None:
             context = ContextScheme()
         else:
             validate_context(context)
 
         message = self._get_message(context=context, payload=payload)
```

### Comparing `zimran-events-0.2.0/zimran/events/schemas.py` & `zimran-events-0.2.1/zimran/events/schemas.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.0/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.2.1/zimran_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.0
+Version: 0.2.1
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.0/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.2.1/zimran_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

