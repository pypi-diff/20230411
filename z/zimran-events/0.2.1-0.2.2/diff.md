# Comparing `tmp/zimran-events-0.2.1.tar.gz` & `tmp/zimran-events-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.2.1.tar", last modified: Tue Apr 11 17:39:15 2023, max compression
+gzip compressed data, was "zimran-events-0.2.2.tar", last modified: Tue Apr 11 18:07:34 2023, max compression
```

## Comparing `zimran-events-0.2.1.tar` & `zimran-events-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.165491 zimran-events-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-11 17:39:06.000000 zimran-events-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 17:39:06.000000 zimran-events-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 17:39:15.165491 zimran-events-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 17:39:06.000000 zimran-events-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 17:39:06.000000 zimran-events-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 17:39:06.000000 zimran-events-0.2.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 17:39:15.165491 zimran-events-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.161491 zimran-events-0.2.1/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-11 17:39:06.000000 zimran-events-0.2.1/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 17:39:15.165491 zimran-events-0.2.1/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 17:39:15.000000 zimran-events-0.2.1/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.635647 zimran-events-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-11 18:07:26.000000 zimran-events-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 18:07:26.000000 zimran-events-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 18:07:34.639647 zimran-events-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-11 18:07:26.000000 zimran-events-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 18:07:26.000000 zimran-events-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-11 18:07:26.000000 zimran-events-0.2.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 18:07:34.639647 zimran-events-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.635647 zimran-events-0.2.2/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-11 18:07:26.000000 zimran-events-0.2.2/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:07:34.639647 zimran-events-0.2.2/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 18:07:34.000000 zimran-events-0.2.2/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.2.1/.github/scripts/release.py` & `zimran-events-0.2.2/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.1/.gitignore` & `zimran-events-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.1/.pre-commit-config.yaml` & `zimran-events-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.1/LICENSE` & `zimran-events-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.1/PKG-INFO` & `zimran-events-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.1
+Version: 0.2.2
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.1/README.md` & `zimran-events-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.1/pyproject.toml` & `zimran-events-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.2.1/zimran/events/connection.py` & `zimran-events-0.2.2/zimran/events/connection.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.1/zimran/events/consumer.py` & `zimran-events-0.2.2/zimran/events/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         }
 
 
 class Consumer(Connection, ConsumerMixin):
     def __init__(self, *, service_name: str, broker_url: str, channel_number: int = 1, prefetch_count: int = 10):
         super().__init__(broker_url=broker_url, channel_number=channel_number)
 
-        self._service_name = service_name
+        self._service_name = service_name.replace('-', '_').lower()
         self._prefetch_count = prefetch_count
 
         self._event_handlers = {}
 
     def run(self):
         try:
             self.channel.basic_qos(prefetch_count=self._prefetch_count)
@@ -102,15 +102,15 @@
         broker_url: str,
         channel_number: int = 1,
         prefetch_count: int = 10,
         loop=None,
     ):
         super().__init__(broker_url=broker_url, loop=loop, channel_number=channel_number)
 
-        self._service_name = service_name
+        self._service_name = service_name.replace('-', '_').lower()
         self._prefetch_count = prefetch_count
 
         self._event_handlers = {}
 
     @retry(retry_policy)
     async def run(self):
         try:
```

### Comparing `zimran-events-0.2.1/zimran/events/producer.py` & `zimran-events-0.2.2/zimran/events/producer.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.1/zimran/events/schemas.py` & `zimran-events-0.2.2/zimran/events/schemas.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.1/zimran/events/utils.py` & `zimran-events-0.2.2/zimran/events/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from aiormq.exceptions import AMQPChannelError, AMQPConnectionError
-from loguru import logger
+
+
+try:
+    from loguru import logger
+except ImportError:
+    import logging
+
+    logger = logging.getLogger(__name__)
 
 from .exceptions import ContextTypeError, ExchangeTypeError
 from .schemas import ContextScheme, ExchangeScheme
 
 
 def validate_exchange(exchange: ExchangeScheme):
     if not isinstance(exchange, ExchangeScheme):
@@ -26,11 +33,11 @@
         queue_name = queue_name[:-1]
 
     return f'{queue_name}_q'
 
 
 def retry_policy(info):
     if isinstance(info.exception, (AMQPConnectionError, AMQPChannelError)):
-        logger.warning(f'Retrying connection... | attempt_amount: {info.fails}')
+        logger.warning(f'Retrying connection... | attempt amount: {info.fails}')
         return info.fails > 3, (info.fails - 1) * 2
 
     return True, 0
```

### Comparing `zimran-events-0.2.1/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.2.2/zimran_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.1
+Version: 0.2.2
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.1/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.2.2/zimran_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

