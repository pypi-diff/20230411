# Comparing `tmp/formenergy-observability-0.1.1.tar.gz` & `tmp/formenergy-observability-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formenergy-observability-0.1.1.tar", last modified: Thu Jan  5 16:47:37 2023, max compression
+gzip compressed data, was "formenergy-observability-0.2.0.tar", last modified: Tue Apr 11 14:30:17 2023, max compression
```

## Comparing `formenergy-observability-0.1.1.tar` & `formenergy-observability-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      186 2023-01-04 16:50:38.583078 formenergy-observability-0.1.1/.gitignore
--rw-r--r--   0        0        0     2038 2023-01-04 16:51:23.731215 formenergy-observability-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      112 2023-01-04 16:51:23.731215 formenergy-observability-0.1.1/.pypirc
--rw-r--r--   0        0        0     1068 2023-01-04 16:09:14.490252 formenergy-observability-0.1.1/LICENSE
--rw-r--r--   0        0        0     3264 2023-01-04 16:55:10.215894 formenergy-observability-0.1.1/README.md
--rw-r--r--   0        0        0   177939 2023-01-04 16:31:04.090964 formenergy-observability-0.1.1/examples/basics-trace.png
--rwxr-xr-x   0        0        0     2570 2023-01-04 16:43:08.409665 formenergy-observability-0.1.1/examples/basics.py
--rw-r--r--   0        0        0   156173 2023-01-04 16:31:04.090964 formenergy-observability-0.1.1/examples/dagster_job.png
--rw-r--r--   0        0        0     2600 2023-01-04 16:49:36.634889 formenergy-observability-0.1.1/examples/dagster_job.py
--rwxr-xr-x   0        0        0     2040 2023-01-04 16:43:34.665751 formenergy-observability-0.1.1/examples/multithread.py
--rw-r--r--   0        0        0      602 2023-01-05 16:42:21.071691 formenergy-observability-0.1.1/form_observability/__init__.py
--rw-r--r--   0        0        0       61 2023-01-05 16:42:09.235771 formenergy-observability-0.1.1/form_observability/conftest.py
--rw-r--r--   0        0        0     8110 2023-01-05 16:42:09.235771 formenergy-observability-0.1.1/form_observability/context_aware.py
--rw-r--r--   0        0        0      299 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/dagster_otel/__init__.py
--rw-r--r--   0        0        0     8838 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/dagster_otel/otel_ops.py
--rw-r--r--   0        0        0     2352 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/dagster_otel/test_otel_op.py
--rw-r--r--   0        0        0      955 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/dagster_otel/test_timing.py
--rw-r--r--   0        0        0      734 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/dagster_otel/testing.py
--rw-r--r--   0        0        0     1291 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/dagster_otel/timing.py
--rw-r--r--   0        0        0      582 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/dagster_otel/util.py
--rw-r--r--   0        0        0     3701 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/log.py
--rw-r--r--   0        0        0     1422 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/otel_value.py
--rw-r--r--   0        0        0     3239 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/pipeline_setup.py
--rw-r--r--   0        0        0     1572 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/test_context_aware.py
--rw-r--r--   0        0        0      941 2023-01-05 16:42:09.239771 formenergy-observability-0.1.1/form_observability/testing.py
--rw-r--r--   0        0        0     1754 2023-01-05 16:45:02.122947 formenergy-observability-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 formenergy-observability-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-01-04 16:50:38.583078 formenergy-observability-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2038 2023-01-04 16:51:23.731215 formenergy-observability-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      112 2023-01-04 16:51:23.731215 formenergy-observability-0.2.0/.pypirc
+-rw-r--r--   0        0        0     1068 2023-01-04 16:09:14.490252 formenergy-observability-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3438 2023-04-11 14:24:18.896172 formenergy-observability-0.2.0/README.md
+-rw-r--r--   0        0        0   177939 2023-01-04 16:31:04.090964 formenergy-observability-0.2.0/examples/basics-trace.png
+-rwxr-xr-x   0        0        0     2570 2023-01-05 18:19:19.918044 formenergy-observability-0.2.0/examples/basics.py
+-rw-r--r--   0        0        0   156173 2023-01-04 16:31:04.090964 formenergy-observability-0.2.0/examples/dagster_job.png
+-rw-r--r--   0        0        0     2621 2023-01-05 18:20:20.389334 formenergy-observability-0.2.0/examples/dagster_job.py
+-rwxr-xr-x   0        0        0     2040 2023-01-05 18:21:06.057762 formenergy-observability-0.2.0/examples/multithread.py
+-rw-r--r--   0        0        0      602 2023-04-11 14:24:25.424182 formenergy-observability-0.2.0/form_observability/__init__.py
+-rw-r--r--   0        0        0       61 2023-01-05 16:42:09.235771 formenergy-observability-0.2.0/form_observability/conftest.py
+-rw-r--r--   0        0        0     8130 2023-01-05 18:33:53.414215 formenergy-observability-0.2.0/form_observability/context_aware.py
+-rw-r--r--   0        0        0      299 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/__init__.py
+-rw-r--r--   0        0        0     8827 2023-04-11 14:25:49.316307 formenergy-observability-0.2.0/form_observability/dagster_otel/otel_ops.py
+-rw-r--r--   0        0        0     2352 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/test_otel_op.py
+-rw-r--r--   0        0        0      955 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/test_timing.py
+-rw-r--r--   0        0        0      734 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/testing.py
+-rw-r--r--   0        0        0     1291 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/timing.py
+-rw-r--r--   0        0        0      582 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/dagster_otel/util.py
+-rw-r--r--   0        0        0     3701 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/log.py
+-rw-r--r--   0        0        0     1422 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/otel_value.py
+-rw-r--r--   0        0        0     3239 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/pipeline_setup.py
+-rw-r--r--   0        0        0     1572 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/test_context_aware.py
+-rw-r--r--   0        0        0      941 2023-01-05 16:42:09.239771 formenergy-observability-0.2.0/form_observability/testing.py
+-rw-r--r--   0        0        0     1754 2023-04-11 14:23:41.900116 formenergy-observability-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 formenergy-observability-0.2.0/PKG-INFO
```

### Comparing `formenergy-observability-0.1.1/.pre-commit-config.yaml` & `formenergy-observability-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/LICENSE` & `formenergy-observability-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/README.md` & `formenergy-observability-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 Context-aware tracing, so that spans and events can inherit attributes from parents:
 
 ```py
 from form_observability import ContextAwareTracer, ctx
 
 _trace = ContextAwareTracer(__name__)
 
-with ctx.set({"test_id": my_test_id}):
-    # many intervening function calls and spans
-    _trace.add_event("my_event")  # automatically has the test_id attribute set on it
+with ctx.set({"my_attribute_name": my_attribute_value}):
+    # There could be many intervening function calls and spans.
+    # Spans and events in this context automatically have the my_attribute_name
+    # attribute set on them.
+    _trace.add_event("my_event")
 ```
 
 Trace context propagation for Dagster ops:
 
 ```py
 from form_observability.dagster_otel import otel_op, publish_current_trace_context
 from form_observability import ContextAwareTracer
@@ -61,23 +63,24 @@
 export OTEL_EXPORTER_OTLP_ENDPOINT="your observability service, defaults to Honeycomb"
 python examples/basics.py
 dagster job execute --python-file examples/dagster_job.py
 ```
 
 ## License
 
-This library is provided under the MIT license, see [LICENSE.txt](LICENSE.txt).
+This library is provided under the MIT license, see [LICENSE](LICENSE).
 
 ## Release Notes
 
+*   0.2.0 Switch to `context.op_handle` and `materialization.metadata` as dict for Dagster 1.2.
 *   0.1.0 Initial external release, including `ContextAwareTracer`, `ctx`, and `@otel_op`.
 
 ## Development
 
-If you contribute, please ensure you and your employer accept [the license](LICENSE.txt) for any of your contributions.
+If you contribute, please ensure you and your employer accept [the license](LICENSE) for any of your contributions.
 
 ### Setup
 
 Create and activate a virtual environment with your favorite tool, such as [direnv](https://github.com/direnv/direnv/wiki/Python). This project requires Python 3.8.
 
 ```bash
 pip install flit
```

### Comparing `formenergy-observability-0.1.1/examples/basics-trace.png` & `formenergy-observability-0.2.0/examples/basics-trace.png`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/examples/basics.py` & `formenergy-observability-0.2.0/examples/basics.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,48 +15,48 @@
 )
 
 
 _trace = ContextAwareTracer(__name__)
 _log = logging.getLogger(__name__)
 
 
-def _helper_that_sometimes_catches_exceptions_internally(test_id: str) -> None:
+def _helper_that_sometimes_catches_exceptions_internally(my_data: str) -> None:
     sleep_s = random.random()
     err_f = random.random()
     # Set some attributes that will be added to any spans and events in this context.
     with ctx.set(
         {
-            "test_size": len(test_id),
+            "data_size": len(my_data),
             "sleep_s": sleep_s,
             "err_f": err_f,
         },
         # Also set these attributes on the active span.
         update_current_span=True,
     ):
         try:
             time.sleep(sleep_s)
             if err_f < 0.1:
                 raise RuntimeError("Demo error to show exception treatment.")
-            # This success event will have the test_size attribute set on it from
-            # the context above, as well as the test_id attribute set in main().
+            # This success event will have the data_size attribute set on it from
+            # the context above, as well as the my_data attribute set in main().
             _trace.add_event("success")
             return True
         except:
             _trace.add_event("failure")
-            _log.exception(f"Error during processing of {test_id=}.")
+            _log.exception(f"Error during processing of {my_data=}.")
             return False
 
 
 @_trace.traced  # Open a span for this function call. In this case it's the root span.
 def main():
     _log.info("Preparing to process tests.")
     num_errors = 0
-    for test_id in ("one", "two", "three", "four", "five", "six"):
-        with _trace.start_as_current_span("work", attributes={"test_id": test_id}):
-            if _helper_that_sometimes_catches_exceptions_internally(test_id):
+    for my_data in ("one", "two", "three", "four", "five", "six"):
+        with _trace.start_as_current_span("work", attributes={"my_data": my_data}):
+            if _helper_that_sometimes_catches_exceptions_internally(my_data):
                 num_errors += 1
     opentelemetry.trace.get_current_span().set_attributes({"num_errors": num_errors})
     _log.info("Demo processing complete.")
 
 
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
```

### Comparing `formenergy-observability-0.1.1/examples/dagster_job.png` & `formenergy-observability-0.2.0/examples/dagster_job.png`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/examples/dagster_job.py` & `formenergy-observability-0.2.0/examples/dagster_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,34 +51,34 @@
     """Each job/subgraph should have one regular op to start and publish the OTel trace."""
     with _trace.start_as_current_span(SpanName.ROOT):
         publish_current_trace_context(context)
         return "TS123"
 
 
 @_trace.traced
-def _do_work(test_id: str):
+def _do_work(my_data: str) -> None:
     """This throws an exception which should be caught by the on_exception_return."""
     raise RuntimeError("Catch me, one test had an error but the pipeline is OK.")
 
 
 @otel_op(
     # If anything in this op raises an exception, catch it and report it using
     # OpenTelemetry, but do not let it cause the Dagster op to fail. This is useful
     # in cases where the overall pipeline can continue running, and you have
     # monitoring in place to investigate specific errors.
     on_exception_return=Output(5, "result"),
 )
-def test_op(context, test_id):
+def test_op(context, my_data: str) -> None:
     """Other ops in the graph use @otel_op to pick up that trace context.
 
     This op looks for a trace context and will error if it can't find it. It should
     find the trace context published by the above op.
     """
-    with ctx.set({"test_id": test_id}, update_current_span=True):
-        _do_work(test_id)
+    with ctx.set({"my_data": my_data}, update_current_span=True):
+        _do_work(my_data)
 
 
 @job(
     # The job will use this resource to set up the span exporter. Every @otel_op
     # requires the observability resource.
     resource_defs={
         CONFIGURE_OBSERVABILITY_RESOURCE_KEY: configure_observability_resource,
```

### Comparing `formenergy-observability-0.1.1/examples/multithread.py` & `formenergy-observability-0.2.0/examples/multithread.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,36 +18,36 @@
 )
 
 
 _trace = ContextAwareTracer(__name__)
 _log = logging.getLogger(__name__)
 
 
-def _thread_worker(test_id: str, otel_ctx) -> None:
+def _thread_worker(my_data: str, otel_ctx) -> None:
     """Worker which re-attaches the OpenTelemetry trace context.
 
     OpenTelemetry does not automatically pick up a parent thread's trace context in a
     child thread. So this worker must be explicitly passed the value from
     context.get_current() which it can then context.attach(..). Thus the child's span
     is parented under the main span.
     """
     opentelemetry.context.attach(otel_ctx)
     sleep_s = random.random() * 4
-    with _trace.start_as_current_span(test_id, attributes={"sleep_s": sleep_s}):
+    with _trace.start_as_current_span(my_data, attributes={"sleep_s": sleep_s}):
         time.sleep(sleep_s)
         _trace.add_event("success")
 
 
 @_trace.traced
 def main():
     _log.info("Preparing to process in threads.")
     otel_ctx = opentelemetry.context.get_current()
     threads = []
-    for test_id in ("one", "two", "three", "four", "five", "six"):
-        thread = threading.Thread(target=_thread_worker, args=(test_id, otel_ctx))
+    for my_data in ("one", "two", "three", "four", "five", "six"):
+        thread = threading.Thread(target=_thread_worker, args=(my_data, otel_ctx))
         thread.start()
         threads.append(thread)
     for thread in threads:
         thread.join()
     _log.info("Demo processing complete.")
```

### Comparing `formenergy-observability-0.1.1/form_observability/__init__.py` & `formenergy-observability-0.2.0/form_observability/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """OTel tracing/logging tools, emphasizing data pipeline use cases with Dagster."""
 
 #: Semantic versioning number. The three dotted numbers are:
 #: *   Major: breaking API changes, significant feature additions.
 #: *   Minor: standard feature additions and improvements. No breaking changes.
 #: *   Micro: small bug fixes.
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 # Make commonly used symbols importable from form_observability.
 from .context_aware import ContextAwareTracer, ctx
 from .log import OtelSpanEventHandler
 from .otel_value import EventAttrKey, EventAttrValue, SpanName
 from .pipeline_setup import configure
```

### Comparing `formenergy-observability-0.1.1/form_observability/context_aware.py` & `formenergy-observability-0.2.0/form_observability/context_aware.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-"""OpenTelemetry tracing setup.
-
-This module handles spans and events, but should not be aware of any implementation
-under other pipeline modules (including as orchestration/ where Dagster/OTel
-integration lives).
+"""OpenTelemetry tracing with context-scoped attributes.
 
 Usage:
 
 _tracer = ContextAwareTracer(__name__)
+
 with _tracer.start_as_current_span(
     "some work",
     attributes={
-        # Attributes added to EventAttrKey/Value...
-        EventAttrKey.TEST_ID: "TST22",
-        # ...or just use one-off keys.
+        # You can use attribute names that are added to EventAttrKey/Value, which
+        # may be useful so you can reference them in monitoring, or...
+        EventAttrKey.DURATION_SECONDS: 12.5,
+        # ...just use one-off keys.
         "foo": 42,
     },
 ):
-    # This event will have the test_id attribute, same as the parent span.
-    _tracer.add_event(EventAttrValue.TEST_SKIPPED)
+    # This event will have the duration_seconds and foo attributes, same as the
+    # parent span.
+    _tracer.add_event(EventAttrValue.MY_CUSTOM_EVENT_NAME)
 
     # If you get more details after opening the span...
-    metadata = db.get...
-
-    # This adds cell_id as an attribute to the parent span since update_current_span=True.
-    with log_ctx.set({EventAttrKey.CELL_ID: metadata["cell_id"]}, update_current_span=True):
-        # Any further spans/events/logs in helper() will have test_id and cell_id.
+    var_value = db.get...
+    # This adds bar as an attribute to the parent span since update_current_span=True.
+    with log_ctx.set({"bar": bar_value, update_current_span=True):
+        # Any further spans/events/logs in helper() will have all the attributes:
+        # EventAttrKey.DURATION_SECONDS, foo, and bar.
         helper()
 """
 from contextlib import contextmanager
 import functools
 import platform
 import threading
 from typing import Optional, Any, Dict
@@ -112,19 +111,19 @@
         """
         return self.current_ctx.get(*args, **kwargs)
 
 
 #: Object to use throughout the application to attach context to logs and traces.
 #:
 #: Usage:
-#:      with ctx.set({EventAttrKey.TEST_ID: "TST22"}):
-#:          # test_id is added to the generated LogRecord.
-#:          _log.info(f"Doing some work.")
-#:          # test_id can also be read back explicitly.
-#:          print("Working on test_id", ctx.get("test_id"))
+#:      with ctx.set({"attr_name": attr_value}):
+#:          # attr_name is added to the generated LogRecord.
+#:          _log.info("Doing some work.")
+#:          # attr_value can also be read back explicitly.
+#:          print(f"Doing some work with attr_name={ctx.get('attr_value')}.")
 ctx = _ObservabilityContext()
 
 
 def _convert_types(v: Any) -> Any:
     """Converts numpy int64s to ints."""
     if type(v).__name__ in ("int8", "int32", "int64"):
         return int(v)
```

### Comparing `formenergy-observability-0.1.1/form_observability/dagster_otel/otel_ops.py` & `formenergy-observability-0.2.0/form_observability/dagster_otel/otel_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         raise RuntimeError("No active span, cannot publish trace context.")
     carrier = {}
     TraceContextTextMapPropagator().inject(carrier)
 
     # If this is in a subgraph, use the subgraph name as the trace key. Otherwise,
     # it's not in a subgraph, use the root span name.
     # Dagster's internal convention is to use dotted namespaces for subgraphs.
-    op_path = context.solid_handle.path
+    op_path = context.op_handle.path
     trace_key = SpanName.ROOT if len(op_path) <= 1 else ".".join(op_path[:-1])
 
     context.log_event(
         AssetMaterialization(
             asset_key=AssetKey(trace_key),
             description="OpenTelemetry trace context.",
             metadata={
@@ -77,15 +77,15 @@
     )
 
 
 def _find_trace_context(context):
     # Try to find a trace context for this subgraph, but fall back to parent graphs
     # up to the root.
     trace_keys = []
-    remaining_path = context.solid_handle.path[:-1]
+    remaining_path = context.op_handle.path[:-1]
     while remaining_path:
         key = ".".join(remaining_path)
         remaining_path.pop()
         trace_keys.append(key)
     trace_keys.append(SpanName.ROOT)
 
     run_ids = get_run_id_and_ancestors(context)
@@ -97,15 +97,15 @@
         for trace_key in trace_keys:
             for event_log_entry in logs:
                 materialization = (
                     event_log_entry.dagster_event.event_specific_data.materialization
                 )
                 event_asset_key = materialization.asset_key.path[0]
                 if event_asset_key == trace_key:
-                    return materialization.metadata_entries[0].entry_data.data
+                    return materialization.metadata["trace_context"].data
 
     raise RuntimeError(
         f"Could not find trace context, searched for any of {trace_keys} in"
         f" {len(all_searched_logs)} events from run IDs {run_ids}."
     )
```

### Comparing `formenergy-observability-0.1.1/form_observability/dagster_otel/test_otel_op.py` & `formenergy-observability-0.2.0/form_observability/dagster_otel/test_otel_op.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/dagster_otel/test_timing.py` & `formenergy-observability-0.2.0/form_observability/dagster_otel/test_timing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/dagster_otel/testing.py` & `formenergy-observability-0.2.0/form_observability/dagster_otel/testing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/dagster_otel/timing.py` & `formenergy-observability-0.2.0/form_observability/dagster_otel/timing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/dagster_otel/util.py` & `formenergy-observability-0.2.0/form_observability/dagster_otel/util.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/log.py` & `formenergy-observability-0.2.0/form_observability/log.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/otel_value.py` & `formenergy-observability-0.2.0/form_observability/otel_value.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/pipeline_setup.py` & `formenergy-observability-0.2.0/form_observability/pipeline_setup.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/test_context_aware.py` & `formenergy-observability-0.2.0/form_observability/test_context_aware.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/form_observability/testing.py` & `formenergy-observability-0.2.0/form_observability/testing.py`

 * *Files identical despite different names*

### Comparing `formenergy-observability-0.1.1/pyproject.toml` & `formenergy-observability-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # also satisfy OTel. (If pip picks OTel's version first, it's outside
     # Dagster's bounds.)
     "grpcio>=1.32.0,<1.48.1",
     "packaging>=20.9,<22",
     # Accept any version that's not a major version upgrade, but is at least
     # a known good recent version. This is slightly different from for example
     # ~=1.1.6 which would mean >=1.1.6,<1.2 and is too strict.
-    "dagster>=1.1.6,<2",
+    "dagster>=1.2.0,<2",
     "opentelemetry-api>=1.15.0,<2",
     "opentelemetry-sdk>=1.15.0,<2",
     "opentelemetry-exporter-otlp-proto-grpc>=1.15.0,<2",
     "opentelemetry-instrumentation-requests>=0.36b0,<1",
     "opentelemetry-instrumentation-sqlalchemy>=0.36b0,<1",
 ]
```

### Comparing `formenergy-observability-0.1.1/PKG-INFO` & `formenergy-observability-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: formenergy-observability
-Version: 0.1.1
+Version: 0.2.0
 Summary: OTel tracing/logging tools, emphasizing data pipeline use cases with Dagster.
 Author-email: Form Energy Software <software@formenergy.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: grpcio>=1.32.0,<1.48.1
 Requires-Dist: packaging>=20.9,<22
-Requires-Dist: dagster>=1.1.6,<2
+Requires-Dist: dagster>=1.2.0,<2
 Requires-Dist: opentelemetry-api>=1.15.0,<2
 Requires-Dist: opentelemetry-sdk>=1.15.0,<2
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc>=1.15.0,<2
 Requires-Dist: opentelemetry-instrumentation-requests>=0.36b0,<1
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy>=0.36b0,<1
 Requires-Dist: pytest~=6.1.2 ; extra == "test"
 Requires-Dist: pytest-html~=2.1.1 ; extra == "test"
@@ -41,17 +41,19 @@
 Context-aware tracing, so that spans and events can inherit attributes from parents:
 
 ```py
 from form_observability import ContextAwareTracer, ctx
 
 _trace = ContextAwareTracer(__name__)
 
-with ctx.set({"test_id": my_test_id}):
-    # many intervening function calls and spans
-    _trace.add_event("my_event")  # automatically has the test_id attribute set on it
+with ctx.set({"my_attribute_name": my_attribute_value}):
+    # There could be many intervening function calls and spans.
+    # Spans and events in this context automatically have the my_attribute_name
+    # attribute set on them.
+    _trace.add_event("my_event")
 ```
 
 Trace context propagation for Dagster ops:
 
 ```py
 from form_observability.dagster_otel import otel_op, publish_current_trace_context
 from form_observability import ContextAwareTracer
@@ -85,23 +87,24 @@
 export OTEL_EXPORTER_OTLP_ENDPOINT="your observability service, defaults to Honeycomb"
 python examples/basics.py
 dagster job execute --python-file examples/dagster_job.py
 ```
 
 ## License
 
-This library is provided under the MIT license, see [LICENSE.txt](LICENSE.txt).
+This library is provided under the MIT license, see [LICENSE](LICENSE).
 
 ## Release Notes
 
+*   0.2.0 Switch to `context.op_handle` and `materialization.metadata` as dict for Dagster 1.2.
 *   0.1.0 Initial external release, including `ContextAwareTracer`, `ctx`, and `@otel_op`.
 
 ## Development
 
-If you contribute, please ensure you and your employer accept [the license](LICENSE.txt) for any of your contributions.
+If you contribute, please ensure you and your employer accept [the license](LICENSE) for any of your contributions.
 
 ### Setup
 
 Create and activate a virtual environment with your favorite tool, such as [direnv](https://github.com/direnv/direnv/wiki/Python). This project requires Python 3.8.
 
 ```bash
 pip install flit
```

