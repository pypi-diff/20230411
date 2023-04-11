# Comparing `tmp/async_sqs_consumer-0.3.5.tar.gz` & `tmp/async_sqs_consumer-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_sqs_consumer-0.3.5.tar", max compression
+gzip compressed data, was "async_sqs_consumer-0.3.6.tar", max compression
```

## Comparing `async_sqs_consumer-0.3.5.tar` & `async_sqs_consumer-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     2410 2023-03-31 13:48:41.692048 async_sqs_consumer-0.3.5/README.md
--rw-r--r--   0        0        0        0 2023-03-31 14:08:47.294687 async_sqs_consumer-0.3.5/async_sqs_consumer/__init__.py
--rw-r--r--   0        0        0     4158 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/queue.py
--rw-r--r--   0        0        0     2254 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/resources.py
--rw-r--r--   0        0        0        0 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/test/__init__.py
--rw-r--r--   0        0        0      542 2023-04-02 17:24:04.634142 async_sqs_consumer-0.3.5/async_sqs_consumer/test/send_message.py
--rw-r--r--   0        0        0      517 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/test/server.py
--rw-r--r--   0        0        0      753 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/types.py
--rw-r--r--   0        0        0      486 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/utils/__init__.py
--rw-r--r--   0        0        0     3803 2023-04-11 12:49:23.872046 async_sqs_consumer-0.3.5/async_sqs_consumer/utils/retry.py
--rw-r--r--   0        0        0     9445 2023-04-11 14:17:02.626204 async_sqs_consumer-0.3.5/async_sqs_consumer/worker.py
--rw-r--r--   0        0        0      647 2023-04-11 14:19:07.227046 async_sqs_consumer-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.5/setup.py
--rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     2410 2023-03-31 13:48:41.692048 async_sqs_consumer-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2023-03-31 14:08:47.294687 async_sqs_consumer-0.3.6/async_sqs_consumer/__init__.py
+-rw-r--r--   0        0        0     4682 2023-04-11 18:06:55.645770 async_sqs_consumer-0.3.6/async_sqs_consumer/queue.py
+-rw-r--r--   0        0        0     2254 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.6/async_sqs_consumer/resources.py
+-rw-r--r--   0        0        0        0 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.6/async_sqs_consumer/test/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-02 17:24:04.634142 async_sqs_consumer-0.3.6/async_sqs_consumer/test/send_message.py
+-rw-r--r--   0        0        0      543 2023-04-11 18:44:09.667026 async_sqs_consumer-0.3.6/async_sqs_consumer/test/server.py
+-rw-r--r--   0        0        0      753 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.6/async_sqs_consumer/types.py
+-rw-r--r--   0        0        0      486 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.6/async_sqs_consumer/utils/__init__.py
+-rw-r--r--   0        0        0     1365 2023-03-31 15:12:56.460833 async_sqs_consumer-0.3.6/async_sqs_consumer/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5522 2023-04-11 14:12:54.911336 async_sqs_consumer-0.3.6/async_sqs_consumer/utils/__pycache__/retry.cpython-311.pyc
+-rw-r--r--   0        0        0     3803 2023-04-11 12:49:23.872046 async_sqs_consumer-0.3.6/async_sqs_consumer/utils/retry.py
+-rw-r--r--   0        0        0    10106 2023-04-11 18:43:37.009724 async_sqs_consumer-0.3.6/async_sqs_consumer/worker.py
+-rw-r--r--   0        0        0      647 2023-04-11 19:40:19.723405 async_sqs_consumer-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.6/setup.py
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.6/PKG-INFO
```

### Comparing `async_sqs_consumer-0.3.5/README.md` & `async_sqs_consumer-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.5/async_sqs_consumer/queue.py` & `async_sqs_consumer-0.3.6/async_sqs_consumer/queue.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,20 +49,22 @@
 
 @retry(exceptions=NETWORK_ERRORS, tries=3, delay=0.2)
 async def get_queue_messages(
     queue_url: str,
     credentials: Optional[AwsCredentials] = None,
     client: Optional[BaseClient] = None,
     visibility_timeout: Optional[int] = None,
+    wait_time_seconds: Optional[int] = None,
 ) -> list[dict[str, Any]]:
     client = await get_sqs_client(credentials)
     response = await client.receive_message(
         QueueUrl=queue_url,
         MaxNumberOfMessages=10,
         VisibilityTimeout=visibility_timeout or 60,
+        WaitTimeSeconds=wait_time_seconds or 0,
     )
     return response.get("Messages", [])
 
 
 @retry(exceptions=NETWORK_ERRORS, tries=3, delay=0.2)
 async def delete_messages(
     queue_url: str,
@@ -76,26 +78,38 @@
     )
 
 
 class Queue:
     def __init__(  # pytlint: disable=too-many-arguments,too-many-arguments
         self,
         url: str,
+        priority: Optional[int] = None,
         authentication: Optional[AwsCredentials] = None,
         polling_interval: Optional[float] = None,
         visibility_timeout: Optional[int] = None,
         max_queue_parallel_messages: Optional[int] = None,
     ) -> None:
         self.url = url
+        self.priority = priority or 1
         self.authentication = authentication
         self.polling_interval = polling_interval or 1.0
         self.visibility_timeout = visibility_timeout or 60
         self._max_queue_parallel_messages = max_queue_parallel_messages
         self._polling = False
 
+    async def get_messages(self, sqs_client: Any) -> list[dict[str, Any]]:
+        with suppress(asyncio.CancelledError):
+            messages = await get_queue_messages(
+                self.url,
+                client=sqs_client,
+                visibility_timeout=self.visibility_timeout,
+            )
+            return messages
+        return []
+
     async def start_polling(
         self,
         callback: Callable[[dict[str, Any], str], Coroutine[Any, Any, None]],
         queue_alias: str,
         max_parallel_messages: Optional[int] = None,
     ) -> None:
         self._polling = self._polling or True
```

### Comparing `async_sqs_consumer-0.3.5/async_sqs_consumer/resources.py` & `async_sqs_consumer-0.3.6/async_sqs_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.5/async_sqs_consumer/test/send_message.py` & `async_sqs_consumer-0.3.6/async_sqs_consumer/test/send_message.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.5/async_sqs_consumer/test/server.py` & `async_sqs_consumer-0.3.6/async_sqs_consumer/test/server.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from asyncio import (
     sleep,
 )
 
 worker = Worker(
     queues={
         "default": Queue(
-            url="https://sqs.us-east-1.amazonaws.com/205810638802/integrates_tasks_dev"
+            url="https://sqs.us-east-1.amazonaws.com/205810638802/integrates_tasks_dev",
+            priority=10,
         )
     },
     max_workers=10,
 )
 
 
 @worker.task("report", queue_name="default")
```

### Comparing `async_sqs_consumer-0.3.5/async_sqs_consumer/types.py` & `async_sqs_consumer-0.3.6/async_sqs_consumer/types.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.5/async_sqs_consumer/utils/retry.py` & `async_sqs_consumer-0.3.6/async_sqs_consumer/utils/retry.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.5/async_sqs_consumer/worker.py` & `async_sqs_consumer-0.3.6/async_sqs_consumer/worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from async_sqs_consumer.queue import (
     Queue,
 )
+from async_sqs_consumer.resources import (
+    RESOURCE_OPTIONS_SQS,
+    SESSION,
+)
 from async_sqs_consumer.utils import (
     TASK_NAME_PREFIX,
     validate_message,
 )
 from async_sqs_consumer.utils.retry import (
     retry_call,
 )
@@ -19,14 +23,17 @@
     partial,
 )
 import json
 import logging
 import pytz
 import signal
 import sys
+from time import (
+    sleep,
+)
 from typing import (
     Any,
     Callable,
     Iterable,
     Literal,
     Optional,
 )
@@ -41,15 +48,14 @@
 
 class Worker:  # pylint: disable=too-many-instance-attributes
     def __init__(
         self, queues: dict[str, Queue], max_workers: Optional[int] = None
     ) -> None:
         self.queues = queues
         self.running = False
-        self.handlers: dict[str, Callable[..., Any]] = {}
         self.handlers_by_queue: dict[str, dict[str, Callable[..., Any]]] = {}
         self._events: dict[str, list[Callable[[], None]]] = {}
         self._loop: Optional[asyncio.AbstractEventLoop] = None
         self._tasks: list[asyncio.Task] = []
         self._max_workers = max_workers or 1024
 
     def _sigint_handler(self, *_args: Any) -> None:
@@ -94,22 +100,22 @@
         Args:
             name (str): tasks received with this name will be
             processed by the decorated function
         Returns:
             Callable[[Callable[[], None]], None]: _description_
         """
 
+        queue_name = queue_name or "default"
+
         def decorator(func: Callable[[], Any]) -> None:
-            if queue_name:
-                if queue_name not in self.handlers_by_queue:
-                    self.handlers_by_queue[queue_name] = {name: func}
-                else:
-                    self.handlers_by_queue[queue_name][name] = func
+            queue_ = queue_name or "default"
+            if queue_ not in self.handlers_by_queue:
+                self.handlers_by_queue[queue_] = {name: func}
             else:
-                self.handlers[name] = func
+                self.handlers_by_queue[queue_][name] = func
 
         return decorator
 
     def on_event(
         self, event_name: Literal["startup", "shutdown"]
     ) -> Callable[[Callable[[], None]], None]:
         """Yo can define event handlers that need to be executed before
@@ -157,25 +163,15 @@
         signal.siginterrupt(signal.SIGTERM, False)
         signal.siginterrupt(signal.SIGUSR1, False)
         signal.signal(signal.SIGINT, partial(self._sigint_handler, self))
         signal.signal(signal.SIGTERM, partial(self._sigterm_handler, self))
 
         for event in self._events.get("startup", []):
             self._loop.run_until_complete(event())  # type: ignore
-
-        for queue_name, queue in self.queues.items():
-            polling_daemon_task = loop.create_task(
-                queue.start_polling(
-                    self._consumer_callback,
-                    queue_name,
-                    max_parallel_messages=self._max_workers,
-                )
-            )
-            self._tasks = [*self._tasks, polling_daemon_task]
-
+        loop.create_task(self._poll_messages())
         self._loop.run_forever()
 
     def _finish_message(
         self,
         _future: Optional[asyncio.Future],
         *,
         handler_name: str,
@@ -220,25 +216,23 @@
         retries: Optional[int] = None,
         receipt_handler: Optional[Any] = None,
         args: Optional[Iterable[Any]] = None,
         kwargs: Optional[dict[str, Any]] = None,
     ) -> bool:
         task_id = task_id or uuid4().hex
         LOGGER.info("Task %s[%s] received", task_name, task_id)
-
+        queue_alias = queue_alias or "default"
         if not self._loop:
             return False
 
         handler = None
-        if queue_alias:
-            if task_name:
-                handler = self.handlers_by_queue.get(queue_alias, {}).get(
-                    task_name
-                )
-                handler = handler or self.handlers.get(task_name)
+        if task_name:
+            handler = self.handlers_by_queue.get(queue_alias, {}).get(
+                task_name
+            )
         if not handler:
             LOGGER.warning(
                 "The task %s has not a candidate to be proceeded",
                 task_name,
             )
             return False
 
@@ -295,7 +289,32 @@
     ) -> None:
         with suppress(asyncio.CancelledError):
             success = await self._process_queue_message(message, queue_alias)
             if not success:
                 await self.queues[queue_alias].delete_messages(
                     message["ReceiptHandle"]
                 )
+
+    async def _poll_messages(self) -> None:
+        queues = list(sorted(self.queues.items(), key=lambda x: x[1].priority))
+        async with SESSION.client(**RESOURCE_OPTIONS_SQS) as sqs_client:
+            while True:
+                if len(
+                    [
+                        task
+                        for task in asyncio.all_tasks(asyncio.get_event_loop())
+                        if task.get_name().startswith(TASK_NAME_PREFIX)
+                    ]
+                ) > (self._max_workers):
+                    await sleep(1)  # type: ignore
+                    continue
+
+                for queue_alias, queue in queues:
+                    messages = await queue.get_messages(sqs_client)
+                    await asyncio.gather(
+                        *[
+                            self._consumer_callback(message, queue_alias)
+                            for message in messages
+                        ]
+                    )
+                    if messages:
+                        break
```

### Comparing `async_sqs_consumer-0.3.5/pyproject.toml` & `async_sqs_consumer-0.3.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_sqs_consumer"
-version = "0.3.5"
+version = "0.3.6"
 description = ""
 authors = ["Diego Restrepo <drestrepo@fluidattacks.com>"]
 repository = 'https://github.com/drestrepom/async_sqs_consumer'
 readme = "README.md"
 keywords = ["AWS", "AWS", "SQS", "sqs", "consumer", "async", "worker"]
 
 [tool.poetry.dependencies]
```

### Comparing `async_sqs_consumer-0.3.5/setup.py` & `async_sqs_consumer-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'aiohttp>=3.8.4,<4.0.0',
  'jsonschema>=4.17.3,<5.0.0',
  'pyrate-limiter>=2.10.0,<3.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'async-sqs-consumer',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': '',
     'long_description': '# Async SQS consumer\n\nPython asynchronous (**async** / **await**) worker for consuming messages\nfrom AWS SQS.\n\nThis is a hobby project, if you find the project interesting\nany contribution is welcome.\n\n## Usage\n\nYou must create an instance of the worker with the url of the queue.\n\nAws credentials are taken from environment variables, you must set the\nfollowing environment variables. Or you can provide a Context object with the\naws credentials `async_sqs_consumer.types.Context`\n\n- `AWS_ACCESS_KEY_ID`\n- `AWS_SECRET_ACCESS_KEY`\n\nExample:\n\nYou can get the queue url with the follow aws cli command\n`aws sqs get-queue-url --queue-name xxxxxx`\n\n```python\n# test_worker.py\n\nfrom async_sqs_consumer.worker import (\n    Worker,\n)\n\nworker = Worker(\n    queue_url="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name"\n)\n\n\n@worker.task("report")\nasync def report(text: str) -> None:\n    print(text)\n\nif __name__: "__main__":\n    worker.start()\n```\n\nNow you can initialize the worker `python test_worker.py`\n\nNow you need to post a message for the worker to process\n\n```python\nimport json\nimport boto3\nimport uuid\n\nclient = boto3.client("sqs")\n\nclient.send_message(\n    QueueUrl="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name",\n    MessageBody=json.dumps(\n        {\n            "task": "report",\n            "id": uuid.uuid4().hex,\n            "args": ["hello world"],\n        }\n    ),\n)\n```\n\nOr you can use aioboto3\n\n```python\nimport asyncio\nimport json\nimport aioboto3\nimport uuid\n\n\nasync def main() -> None:\n    session = aioboto3.Session()\n    async with session.client("sqs") as client:\n        await client.send_message(\n            QueueUrl="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name",\n            MessageBody=json.dumps(\n                {\n                    "task": "report",\n                    "id": uuid.uuid4().hex,\n                    "args": ["hello world"],\n                }\n            ),\n        )\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo publish the messages they must have the following structure\n\n```json\n{\n    "type": "object",\n    "properties": {\n        "task": {"type": "string"},\n        "id": {"type": "string"},\n        "args": {"type": "array"},\n        "kwargs": {"type": "object"},\n        "retries": {"type": "number"},\n        "eta": {"type": "string"},\n        "expires": {"type": "string"},\n    },\n    "required": ["task", "id"],\n}\n```\n',
     'author': 'Diego Restrepo',
     'author_email': 'drestrepo@fluidattacks.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/drestrepom/async_sqs_consumer',
```

### Comparing `async_sqs_consumer-0.3.5/PKG-INFO` & `async_sqs_consumer-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-sqs-consumer
-Version: 0.3.5
+Version: 0.3.6
 Summary: 
 Home-page: https://github.com/drestrepom/async_sqs_consumer
 Keywords: AWS,AWS,SQS,sqs,consumer,async,worker
 Author: Diego Restrepo
 Author-email: drestrepo@fluidattacks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

