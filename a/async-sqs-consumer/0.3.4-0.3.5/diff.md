# Comparing `tmp/async_sqs_consumer-0.3.4.tar.gz` & `tmp/async_sqs_consumer-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_sqs_consumer-0.3.4.tar", max compression
+gzip compressed data, was "async_sqs_consumer-0.3.5.tar", max compression
```

## Comparing `async_sqs_consumer-0.3.4.tar` & `async_sqs_consumer-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2410 2023-03-31 13:48:41.692048 async_sqs_consumer-0.3.4/README.md
--rw-r--r--   0        0        0        0 2023-03-31 14:08:47.294687 async_sqs_consumer-0.3.4/async_sqs_consumer/__init__.py
--rw-r--r--   0        0        0     4158 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.4/async_sqs_consumer/queue.py
--rw-r--r--   0        0        0     2254 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.4/async_sqs_consumer/resources.py
--rw-r--r--   0        0        0        0 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.4/async_sqs_consumer/test/__init__.py
--rw-r--r--   0        0        0      539 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.4/async_sqs_consumer/test/send_message.py
--rw-r--r--   0        0        0      517 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.4/async_sqs_consumer/test/server.py
--rw-r--r--   0        0        0      753 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.4/async_sqs_consumer/types.py
--rw-r--r--   0        0        0      486 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.4/async_sqs_consumer/utils/__init__.py
--rw-r--r--   0        0        0     3776 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.4/async_sqs_consumer/utils/retry.py
--rw-r--r--   0        0        0     9207 2023-04-01 16:13:26.544332 async_sqs_consumer-0.3.4/async_sqs_consumer/worker.py
--rw-r--r--   0        0        0      611 2023-04-01 16:15:03.466526 async_sqs_consumer-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.4/setup.py
--rw-r--r--   0        0        0     3177 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     2410 2023-03-31 13:48:41.692048 async_sqs_consumer-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2023-03-31 14:08:47.294687 async_sqs_consumer-0.3.5/async_sqs_consumer/__init__.py
+-rw-r--r--   0        0        0     4158 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/queue.py
+-rw-r--r--   0        0        0     2254 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/resources.py
+-rw-r--r--   0        0        0        0 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/test/__init__.py
+-rw-r--r--   0        0        0      542 2023-04-02 17:24:04.634142 async_sqs_consumer-0.3.5/async_sqs_consumer/test/send_message.py
+-rw-r--r--   0        0        0      517 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/test/server.py
+-rw-r--r--   0        0        0      753 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/types.py
+-rw-r--r--   0        0        0      486 2023-03-31 14:08:47.295687 async_sqs_consumer-0.3.5/async_sqs_consumer/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2023-04-11 12:49:23.872046 async_sqs_consumer-0.3.5/async_sqs_consumer/utils/retry.py
+-rw-r--r--   0        0        0     9445 2023-04-11 14:17:02.626204 async_sqs_consumer-0.3.5/async_sqs_consumer/worker.py
+-rw-r--r--   0        0        0      647 2023-04-11 14:19:07.227046 async_sqs_consumer-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3388 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.5/setup.py
+-rw-r--r--   0        0        0     3256 1970-01-01 00:00:00.000000 async_sqs_consumer-0.3.5/PKG-INFO
```

### Comparing `async_sqs_consumer-0.3.4/README.md` & `async_sqs_consumer-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.4/async_sqs_consumer/queue.py` & `async_sqs_consumer-0.3.5/async_sqs_consumer/queue.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.4/async_sqs_consumer/resources.py` & `async_sqs_consumer-0.3.5/async_sqs_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.4/async_sqs_consumer/test/send_message.py` & `async_sqs_consumer-0.3.5/async_sqs_consumer/test/send_message.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     client.send_message(
         QueueUrl=(
             "https://sqs.us-east-1.amazonaws.com/205810638802/integrates_tasks_dev"
         ),
         MessageBody=json.dumps(
             {
                 "id": uuid.uuid4().hex,
-                "task": "clone",
+                "task": "report",
                 "args": [
                     "vergeladc",
-                    "ddafdd56-c17f-43c3-9e4c-7e3e074399b9",
+                    # "ddafdd56-c17f-43c3-9e4c-7e3e074399b9",
                 ],
             }
         ),
     )
```

### Comparing `async_sqs_consumer-0.3.4/async_sqs_consumer/test/server.py` & `async_sqs_consumer-0.3.5/async_sqs_consumer/test/server.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.4/async_sqs_consumer/types.py` & `async_sqs_consumer-0.3.5/async_sqs_consumer/types.py`

 * *Files identical despite different names*

### Comparing `async_sqs_consumer-0.3.4/async_sqs_consumer/utils/retry.py` & `async_sqs_consumer-0.3.5/async_sqs_consumer/utils/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
         return wrapper
 
     return decorator
 
 
 async def retry_call(
-    func: partial,
+    func: Union[partial, Callable[..., Any]],
     tries: int,
     exceptions: Union[
         Type[BaseException], list[type[BaseException]]
     ] = Exception,
     delay: Optional[float] = None,
     max_delay: Optional[float] = None,
     backoff: Optional[float] = None,
```

### Comparing `async_sqs_consumer-0.3.4/async_sqs_consumer/worker.py` & `async_sqs_consumer-0.3.5/async_sqs_consumer/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,23 +70,24 @@
         if self._loop:
             LOGGER.debug("Stop worker")
             self.running = False
             for queue in self.queues.values():
                 queue.stop_polling()
             for event in self._events.get("shutdown", []):
                 self._loop.run_until_complete(event())  # type: ignore
-            for task in self._tasks:
-                task.cancel()
+
+            map(lambda task: task.cancel(), self._tasks)
+
             _queue_tasks = [
                 task
                 for task in asyncio.all_tasks(self._loop)
                 if task.get_name().startswith(TASK_NAME_PREFIX)
             ]
-            # TODO: make sure all tasks are finished before finishing the entire process
-
+            # TODO: make sure all tasks are finished before finishing the
+            # entire process
             self._loop.stop()
 
     def task(
         self, name: str, queue_name: Optional[str] = None
     ) -> Callable[..., None]:
         """A decorator to add a task that could be handled by the worker.
 
@@ -154,27 +155,27 @@
             )
 
         signal.siginterrupt(signal.SIGTERM, False)
         signal.siginterrupt(signal.SIGUSR1, False)
         signal.signal(signal.SIGINT, partial(self._sigint_handler, self))
         signal.signal(signal.SIGTERM, partial(self._sigterm_handler, self))
 
+        for event in self._events.get("startup", []):
+            self._loop.run_until_complete(event())  # type: ignore
+
         for queue_name, queue in self.queues.items():
             polling_daemon_task = loop.create_task(
                 queue.start_polling(
                     self._consumer_callback,
                     queue_name,
                     max_parallel_messages=self._max_workers,
                 )
             )
             self._tasks = [*self._tasks, polling_daemon_task]
 
-        for event in self._events.get("startup", []):
-            self._loop.run_until_complete(event())  # type: ignore
-
         self._loop.run_forever()
 
     def _finish_message(
         self,
         _future: Optional[asyncio.Future],
         *,
         handler_name: str,
@@ -182,15 +183,15 @@
         queue_alias: str,
         start_time: float,
         receipt_handle: Optional[Any] = None,
     ) -> None:
         start_date = datetime.fromtimestamp(start_time, pytz.UTC)
         end_date = datetime.utcnow().replace(tzinfo=pytz.UTC)
         total_seconds = end_date - start_date
-        if _future.exception() is not None:
+        if _future and _future.exception() is not None:
             LOGGER.warning(
                 "Failed to execute task %s[%s]", handler_name, task_id
             )
         else:
             LOGGER.info(
                 "Task %s[%s] succeeded in %ss: None",
                 handler_name,
@@ -216,30 +217,39 @@
         task_id: Optional[str] = None,
         task_name: Optional[str] = None,
         queue_alias: Optional[str] = None,
         retries: Optional[int] = None,
         receipt_handler: Optional[Any] = None,
         args: Optional[Iterable[Any]] = None,
         kwargs: Optional[dict[str, Any]] = None,
-    ) -> None:
+    ) -> bool:
         task_id = task_id or uuid4().hex
         LOGGER.info("Task %s[%s] received", task_name, task_id)
-        handler = self.handlers_by_queue.get(queue_alias, {}).get(task_name)
-        handler = handler or self.handlers.get(task_name)
+
+        if not self._loop:
+            return False
+
+        handler = None
+        if queue_alias:
+            if task_name:
+                handler = self.handlers_by_queue.get(queue_alias, {}).get(
+                    task_name
+                )
+                handler = handler or self.handlers.get(task_name)
         if not handler:
             LOGGER.warning(
                 "The task %s has not a candidate to be proceeded",
                 task_name,
             )
             return False
 
         task = self._loop.create_task(
             retry_call(
                 handler,
-                fargs=args or [],
+                fargs=tuple(args or []),
                 fkwargs=kwargs or {},
                 tries=retries or 1,
             ),
             name=(
                 f"{TASK_NAME_PREFIX}{queue_alias}"
                 f"_{task_name}_{uuid4().hex[:8]}"
             ),
@@ -252,15 +262,15 @@
                 start_time=datetime.utcnow().timestamp(),
                 handler_name=task_name,
                 task_id=task_id,
             )
         )
         return True
 
-    async def _process_message(
+    async def _process_queue_message(
         self, message_content: dict[str, Any], queue_alias: str
     ) -> bool:
         try:
             body = json.loads(message_content["Body"])
         except json.JSONDecodeError:
             return False
 
@@ -274,16 +284,18 @@
             queue_alias=queue_alias,
             retries=body.get("retries", 1),
             receipt_handler=message_content["ReceiptHandle"],
             args=body.get("args", []),
             kwargs=body.get("kwargs", {}),
         )
 
+        return True
+
     async def _consumer_callback(
         self, message: dict[str, Any], queue_alias: str
     ) -> None:
         with suppress(asyncio.CancelledError):
-            success = await self._process_message(message, queue_alias)
+            success = await self._process_queue_message(message, queue_alias)
             if not success:
                 await self.queues[queue_alias].delete_messages(
                     message["ReceiptHandle"]
                 )
```

### Comparing `async_sqs_consumer-0.3.4/pyproject.toml` & `async_sqs_consumer-0.3.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "async_sqs_consumer"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["Diego Restrepo <drestrepo@fluidattacks.com>"]
 repository = 'https://github.com/drestrepom/async_sqs_consumer'
 readme = "README.md"
 keywords = ["AWS", "AWS", "SQS", "sqs", "consumer", "async", "worker"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiobotocore = "^2.4.0"
 aioboto3 = "^10.1.0"
 jsonschema = "^4.17.3"
 pyrate-limiter = "^2.10.0"
+aiohttp = "^3.8.4"
+pytz = "^2023.3"
 
 [tool.poetry.dev-dependencies]
 prospector = "^1.7.7"
 black = "^22.8.0"
 isort = "^5.10.1"
 
 [build-system]
```

### Comparing `async_sqs_consumer-0.3.4/setup.py` & `async_sqs_consumer-0.3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aioboto3>=10.1.0,<11.0.0',
  'aiobotocore>=2.4.0,<3.0.0',
+ 'aiohttp>=3.8.4,<4.0.0',
  'jsonschema>=4.17.3,<5.0.0',
- 'pyrate-limiter>=2.10.0,<3.0.0']
+ 'pyrate-limiter>=2.10.0,<3.0.0',
+ 'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'async-sqs-consumer',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': '',
     'long_description': '# Async SQS consumer\n\nPython asynchronous (**async** / **await**) worker for consuming messages\nfrom AWS SQS.\n\nThis is a hobby project, if you find the project interesting\nany contribution is welcome.\n\n## Usage\n\nYou must create an instance of the worker with the url of the queue.\n\nAws credentials are taken from environment variables, you must set the\nfollowing environment variables. Or you can provide a Context object with the\naws credentials `async_sqs_consumer.types.Context`\n\n- `AWS_ACCESS_KEY_ID`\n- `AWS_SECRET_ACCESS_KEY`\n\nExample:\n\nYou can get the queue url with the follow aws cli command\n`aws sqs get-queue-url --queue-name xxxxxx`\n\n```python\n# test_worker.py\n\nfrom async_sqs_consumer.worker import (\n    Worker,\n)\n\nworker = Worker(\n    queue_url="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name"\n)\n\n\n@worker.task("report")\nasync def report(text: str) -> None:\n    print(text)\n\nif __name__: "__main__":\n    worker.start()\n```\n\nNow you can initialize the worker `python test_worker.py`\n\nNow you need to post a message for the worker to process\n\n```python\nimport json\nimport boto3\nimport uuid\n\nclient = boto3.client("sqs")\n\nclient.send_message(\n    QueueUrl="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name",\n    MessageBody=json.dumps(\n        {\n            "task": "report",\n            "id": uuid.uuid4().hex,\n            "args": ["hello world"],\n        }\n    ),\n)\n```\n\nOr you can use aioboto3\n\n```python\nimport asyncio\nimport json\nimport aioboto3\nimport uuid\n\n\nasync def main() -> None:\n    session = aioboto3.Session()\n    async with session.client("sqs") as client:\n        await client.send_message(\n            QueueUrl="https://sqs.us-east-1.amazonaws.com/xxxxxxx/queue_name",\n            MessageBody=json.dumps(\n                {\n                    "task": "report",\n                    "id": uuid.uuid4().hex,\n                    "args": ["hello world"],\n                }\n            ),\n        )\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\nTo publish the messages they must have the following structure\n\n```json\n{\n    "type": "object",\n    "properties": {\n        "task": {"type": "string"},\n        "id": {"type": "string"},\n        "args": {"type": "array"},\n        "kwargs": {"type": "object"},\n        "retries": {"type": "number"},\n        "eta": {"type": "string"},\n        "expires": {"type": "string"},\n    },\n    "required": ["task", "id"],\n}\n```\n',
     'author': 'Diego Restrepo',
     'author_email': 'drestrepo@fluidattacks.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/drestrepom/async_sqs_consumer',
```

### Comparing `async_sqs_consumer-0.3.4/PKG-INFO` & `async_sqs_consumer-0.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: async-sqs-consumer
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Home-page: https://github.com/drestrepom/async_sqs_consumer
 Keywords: AWS,AWS,SQS,sqs,consumer,async,worker
 Author: Diego Restrepo
 Author-email: drestrepo@fluidattacks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aioboto3 (>=10.1.0,<11.0.0)
 Requires-Dist: aiobotocore (>=2.4.0,<3.0.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: pyrate-limiter (>=2.10.0,<3.0.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Project-URL: Repository, https://github.com/drestrepom/async_sqs_consumer
 Description-Content-Type: text/markdown
 
 # Async SQS consumer
 
 Python asynchronous (**async** / **await**) worker for consuming messages
 from AWS SQS.
```

