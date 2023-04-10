# Comparing `tmp/dramatiq_mongodb-0.8.2.tar.gz` & `tmp/dramatiq_mongodb-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_mongodb-0.8.2.tar", max compression
+gzip compressed data, was "dramatiq_mongodb-0.8.3.tar", max compression
```

## Comparing `dramatiq_mongodb-0.8.2.tar` & `dramatiq_mongodb-0.8.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6385 2023-04-10 21:24:04.779771 dramatiq_mongodb-0.8.2/CHANGELOG.md
--rw-r--r--   0        0        0     1071 2023-04-10 21:23:18.995244 dramatiq_mongodb-0.8.2/LICENSE
--rw-r--r--   0        0        0     2096 2023-04-10 21:23:18.995244 dramatiq_mongodb-0.8.2/README.md
--rw-r--r--   0        0        0     2556 2023-04-10 21:24:04.791771 dramatiq_mongodb-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      172 2023-04-10 21:24:04.791771 dramatiq_mongodb-0.8.2/src/dramatiq_mongodb/__init__.py
--rw-r--r--   0        0        0     6538 2023-04-10 21:23:18.995244 dramatiq_mongodb-0.8.2/src/dramatiq_mongodb/backend.py
--rw-r--r--   0        0        0     8608 2023-04-10 21:23:18.995244 dramatiq_mongodb-0.8.2/src/dramatiq_mongodb/broker.py
--rw-r--r--   0        0        0      181 2023-04-10 21:23:18.995244 dramatiq_mongodb-0.8.2/src/dramatiq_mongodb/state.py
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     6582 2023-04-10 22:06:12.730353 dramatiq_mongodb-0.8.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1071 2023-04-10 22:05:24.305192 dramatiq_mongodb-0.8.3/LICENSE
+-rw-r--r--   0        0        0     2096 2023-04-10 22:05:24.305192 dramatiq_mongodb-0.8.3/README.md
+-rw-r--r--   0        0        0     2556 2023-04-10 22:06:12.742353 dramatiq_mongodb-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-04-10 22:06:12.742353 dramatiq_mongodb-0.8.3/src/dramatiq_mongodb/__init__.py
+-rw-r--r--   0        0        0     6538 2023-04-10 22:05:24.305192 dramatiq_mongodb-0.8.3/src/dramatiq_mongodb/backend.py
+-rw-r--r--   0        0        0     9419 2023-04-10 22:05:24.305192 dramatiq_mongodb-0.8.3/src/dramatiq_mongodb/broker.py
+-rw-r--r--   0        0        0      181 2023-04-10 22:05:24.305192 dramatiq_mongodb-0.8.3/src/dramatiq_mongodb/state.py
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 dramatiq_mongodb-0.8.3/PKG-INFO
```

### Comparing `dramatiq_mongodb-0.8.2/CHANGELOG.md` & `dramatiq_mongodb-0.8.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.8.3 (2023-04-10)
+### Fix
+* Change enqueue and requeue to use different logic ([`c0cd21b`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/c0cd21b0fb1743e1bbe76a6319b76085e4ce2db8))
+
 ## v0.8.2 (2023-04-10)
 ### Fix
 * Turns out python3.7 doesn't have = in f-strings ([`caf8b48`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/caf8b48abbd93b5ae632e3c3ea796b1e4005f3df))
 * Convert enqueue back to replace with better edge case detection ([`d15ad01`](https://github.com/obscuritylabs/dramatiq-mongodb/commit/d15ad01a44136c5ba4d2db89ded3af4bc729d022))
 
 ## v0.8.1 (2023-04-10)
 ### Fix
```

### Comparing `dramatiq_mongodb-0.8.2/LICENSE` & `dramatiq_mongodb-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.8.2/README.md` & `dramatiq_mongodb-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.8.2/pyproject.toml` & `dramatiq_mongodb-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 authors = ["Tory Clasen <ToryClasen@Gmail.com>"]
 description = "Dramatiq-Mongodb Broker and Results Backend for Dramatiq"
 include = ["CHANGELOG.md"]
 license = "MIT"
 name = "dramatiq-mongodb"
 readme = "README.md"
 repository = "https://github.com/obscuritylabs/dramatiq-mongodb"
-version = "0.8.2"
+version = "0.8.3"
 
 [tool.poetry.dependencies]
 dramatiq = "^1.14.2"
 pymongo = ">=4.1,<5"
 python = ">=3.7,<4"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `dramatiq_mongodb-0.8.2/src/dramatiq_mongodb/backend.py` & `dramatiq_mongodb-0.8.3/src/dramatiq_mongodb/backend.py`

 * *Files identical despite different names*

### Comparing `dramatiq_mongodb-0.8.2/src/dramatiq_mongodb/broker.py` & `dramatiq_mongodb-0.8.3/src/dramatiq_mongodb/broker.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,29 +103,52 @@
         self.emit_before("enqueue", message, delay)  # type: ignore
         queue_name = message.queue_name
         self.logger.debug(f"Enqueueing message {message.message_id} on queue {queue_name}")
         if delay:
             millis: int = current_millis()  # type: ignore
             message = message.copy(options={"eta": millis + delay})
 
+        document = {
+            "_id": UUID(message.message_id),
+            "msg": message.asdict(),
+            "state": State.QUEUED,
+        }
+        collection = self.queues[queue_name]
+        collection.insert_one(document)
+
+        self.emit_after("enqueue", message, delay)  # type: ignore
+        return message
+
+    def requeue(self: MongoDBBroker, message: Message[Any], *, delay: Optional[int] = None) -> Message[Any]:
+        """Requeue an existing message on the designated queue.
+
+        Args:
+            message (Message[Any]): The message to enqueue
+            delay (Optional[int], optional): Milliseconds until message should br processed. Defaults to None.
+
+        Returns:
+            Message[Any]: The message that was requeued.
+        """
+        self.emit_before("enqueue", message, delay)  # type: ignore
+        queue_name = message.queue_name
+        self.logger.debug(f"Requeueing message {message.message_id} on queue {queue_name}")
+        if delay:
+            millis: int = current_millis()  # type: ignore
+            message = message.copy(options={"eta": millis + delay})
+
         document = {"msg": message.asdict(), "state": State.QUEUED}
         collection = self.queues[queue_name]
 
-        results = collection.replace_one(
+        collection.replace_one(
             filter={
                 "_id": UUID(message.message_id),
-                "state": {"$or": [{"$exists": False}, {"state": State.CONSUMED}]},
+                "state": State.CONSUMED,
             },
             replacement=document,
-            upsert=True,
         )
-        if results.matched_count > 1 or results.modified_count > 1:
-            self.logger.exception(
-                f"Failed to enqueue {message.message_id} / {results.matched_count} / {results.modified_count}"
-            )
 
         self.emit_after("enqueue", message, delay)  # type: ignore
         return message
 
     def flush(self: MongoDBBroker, queue_name: str) -> None:
         """Drop collection that the queue resides in.
 
@@ -222,8 +245,8 @@
     def requeue(self: _MongoDBConsumer, messages: List[MessageProxy]) -> None:
         """Requeue all messaged that have been claimed but not acked or nacked.
 
         Args:
             messages (List[MessageProxy]): The list of messages to requeue.
         """
         for message in messages:
-            self.broker.enqueue(message._message)  # noqa: SF01
+            self.broker.requeue(message._message)  # noqa: SF01
```

### Comparing `dramatiq_mongodb-0.8.2/PKG-INFO` & `dramatiq_mongodb-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramatiq-mongodb
-Version: 0.8.2
+Version: 0.8.3
 Summary: Dramatiq-Mongodb Broker and Results Backend for Dramatiq
 Home-page: https://github.com/obscuritylabs/dramatiq-mongodb
 License: MIT
 Author: Tory Clasen
 Author-email: ToryClasen@Gmail.com
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
```

