# Comparing `tmp/motion_python-0.1.30.tar.gz` & `tmp/motion_python-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.30.tar", max compression
+gzip compressed data, was "motion_python-0.1.31.tar", max compression
```

## Comparing `motion_python-0.1.30.tar` & `motion_python-0.1.31.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2819 2023-04-10 22:08:18.695807 motion_python-0.1.30/README.md
--rw-r--r--   0        0        0      641 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/api/__init__.py
--rw-r--r--   0        0        0     6702 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/api/models.py
--rw-r--r--   0        0        0     2618 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/cli.py
--rw-r--r--   0        0        0     9885 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/client.py
--rw-r--r--   0        0        0    21544 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/cursor.py
--rw-r--r--   0        0        0     8664 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      398 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1348 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4617 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     5003 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     2975 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/routing.py
--rw-r--r--   0        0        0     3477 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/schema.py
--rw-r--r--   0        0        0    14188 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/store.py
--rw-r--r--   0        0        0     3741 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/task.py
--rw-r--r--   0        0        0     5977 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/trigger.py
--rw-r--r--   0        0        0     1092 2023-04-10 22:08:18.699807 motion_python-0.1.30/motion/utils.py
--rw-r--r--   0        0        0     1416 2023-04-10 22:08:38.351831 motion_python-0.1.30/pyproject.toml
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.30/PKG-INFO
+-rw-r--r--   0        0        0     2819 2023-04-11 00:01:27.288007 motion_python-0.1.31/README.md
+-rw-r--r--   0        0        0      641 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/api/__init__.py
+-rw-r--r--   0        0        0     6702 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/api/models.py
+-rw-r--r--   0        0        0     2618 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/cli.py
+-rw-r--r--   0        0        0     9885 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/client.py
+-rw-r--r--   0        0        0    21630 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/cursor.py
+-rw-r--r--   0        0        0     8664 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1348 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     5003 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     2975 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/routing.py
+-rw-r--r--   0        0        0     3413 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/schema.py
+-rw-r--r--   0        0        0    14909 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/store.py
+-rw-r--r--   0        0        0     3746 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/task.py
+-rw-r--r--   0        0        0     5977 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/trigger.py
+-rw-r--r--   0        0        0     1892 2023-04-11 00:01:27.292007 motion_python-0.1.31/motion/utils.py
+-rw-r--r--   0        0        0     1416 2023-04-11 00:01:46.239987 motion_python-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.31/PKG-INFO
```

### Comparing `motion_python-0.1.30/README.md` & `motion_python-0.1.31/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/__init__.py` & `motion_python-0.1.31/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/api/api.py` & `motion_python-0.1.31/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/api/models.py` & `motion_python-0.1.31/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/cli.py` & `motion_python-0.1.31/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/client.py` & `motion_python-0.1.31/motion/client.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/cursor.py` & `motion_python-0.1.31/motion/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,18 @@
         self.triggers_to_run_on_duplicate = triggers_to_run_on_duplicate
         self.spawned_by = spawned_by
 
     def __del__(self) -> None:
         if self.wait_for_results:
             self.waitForResults()
 
+    def close(self) -> None:
+        """Closes the cursor."""
+        self.__del__()
+
     def waitForResults(self) -> None:
         """Waits for all fit events to finish."""
         for t in self.fit_events:
             t.wait()
         self.fit_events = []
 
     def getNewId(self, relation: str, key: str = "identifier") -> str:
```

### Comparing `motion_python-0.1.30/motion/entry.py` & `motion_python-0.1.31/motion/entry.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/examples/cooking/dashboard.py` & `motion_python-0.1.31/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/examples/cooking/test.py` & `motion_python-0.1.31/motion/examples/cooking/test.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.31/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.31/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/routing.py` & `motion_python-0.1.31/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/motion/schema.py` & `motion_python-0.1.31/motion/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,22 +92,21 @@
             for f in fields
             if not f.name == "identifier"
             and not f.name == "create_at"
             and not f.name == "derived_id"
             and not f.name == "session_id"
         ]
         pa_fields = [
-            pa.field("identifier", pa.string(), nullable=False),
+            pa.field("identifier", pa.string()),
             pa.field(
                 "create_at",
                 pa.timestamp("us"),
-                nullable=False,
             ),
             pa.field("derived_id", pa.string()),
-            pa.field("session_id", pa.string(), nullable=False),
+            pa.field("session_id", pa.string()),
         ]
 
         for field in user_defined_fields:
             try:
                 arrow_type = get_arrow_type(field.type_)
             except TypeError as e:
                 raise TypeError(f"Error in {relation}.{field.name}: {e}")
```

### Comparing `motion_python-0.1.30/motion/store.py` & `motion_python-0.1.31/motion/store.py`

 * *Files 3% similar despite different names*

```diff
@@ -187,28 +187,42 @@
         Args:
             name (str): The name of the relation.
             schema (motion.Schema): The schema of the relation.
         """
         pa_schema = schema.formatPaSchema(name)
 
         if name in self.relations:
-            pa_schema_names = pa_schema.names
-            pa_schema_types = pa_schema.types
+            # Try to cast existing table to current schema
+            try:
+                union_schema = pa.unify_schemas(
+                    [self.relations[name].schema, pa_schema]
+                )
+                self.relations[name] = self.relations[name].cast(union_schema)
+            except pa.ArrowInvalid as e:
+                logger.error(
+                    f"Could not cast existing table {name} to new schema. Please clear the data store with `motion clear {self.name}` and try again."
+                )
+                raise e
+            except ValueError as e:
+                # Perform schema migration
+                logger.warning(f"Performing schema migration for table {name}.")
+                # Find fields that are in the new schema but not the old
+                for field_idx in range(len(pa_schema.names)):
+                    field = pa_schema.field(field_idx)
+                    if field.name not in self.relations[name].schema.names:
+                        # Add field to existing table
+                        self.relations[name] = self.relations[name].append_column(
+                            field.name,
+                            pa.array(
+                                [None] * len(self.relations[name]),
+                                type=field.type,
+                            ),
+                        )
 
-            for old_name, old_type in zip(
-                self.relations[name].schema.names,
-                self.relations[name].schema.types,
-            ):
-                if old_name == "session_id":
-                    continue
-                name_idx = pa_schema_names.index(old_name)
-                if not old_type.equals(pa_schema_types[name_idx]):
-                    logger.error(
-                        f"relation {name} already exists with a different schema. Please clear the data store with `motion clear {self.name}` and try again."
-                    )
+                # raise e
 
         else:
             logger.info(f"Adding relation {name} with schema {pa_schema}")
             self.relations[name] = pa_schema.empty_table()
 
             self.table_columns[name] = self.relations[name].schema.names
             self.table_columns[name].remove("identifier")
```

### Comparing `motion_python-0.1.30/motion/task.py` & `motion_python-0.1.31/motion/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,18 +76,18 @@
                     raise e
 
             if self.first_run:
                 self.first_run_event.set()
                 self.first_run = False
 
             self.checkpoint_fn()
-            logger.info(f"Checkpointed store from task {self.trigger_fn.name}.")
+            logger.debug(f"Checkpointed store from task {self.trigger_fn.name}.")
 
     def stop(self) -> None:
-        logger.info(f"Stopping task thread for name {self.trigger_fn.name}")
+        logger.debug(f"Stopping task thread for name {self.trigger_fn.name}")
         self.running = False
 
 
 class CheckpointThread(threading.Thread):
     def __init__(
         self,
         store_name: str,
@@ -108,14 +108,14 @@
             )
             delay = (next_time - datetime.now()).total_seconds()
             if delay > 0:
                 time.sleep(delay)
             else:
                 continue
 
-            logger.info(f"Checkpointing store {self.name}")
+            logger.debug(f"Checkpointing store {self.name}")
             self.checkpoint_fn()
-            logger.info(f"Finished checkpointing store {self.name}")
+            logger.debug(f"Finished checkpointing store {self.name}")
 
     def stop(self) -> None:
-        logger.info(f"Stopping checkpoint thread for store {self.name}")
+        logger.debug(f"Stopping checkpoint thread for store {self.name}")
         self.running = False
```

### Comparing `motion_python-0.1.30/motion/trigger.py` & `motion_python-0.1.31/motion/trigger.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.30/pyproject.toml` & `motion_python-0.1.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.30"
+version = "0.1.31"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `motion_python-0.1.30/PKG-INFO` & `motion_python-0.1.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.30
+Version: 0.1.31
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

