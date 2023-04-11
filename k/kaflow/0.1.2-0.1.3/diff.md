# Comparing `tmp/kaflow-0.1.2.tar.gz` & `tmp/kaflow-0.1.3.tar.gz`

## Comparing `kaflow-0.1.2.tar` & `kaflow-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.1.2/Makefile
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.1.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.1.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/__init__.py
--rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/_consumer.py
--rw-r--r--   0        0        0    21832 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/applications.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/dependencies.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/exceptions.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/logger.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/message.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/py.typed
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/serializers.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/_utils/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/_utils/asyncio.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/_utils/inspect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/asyncapi/__init__.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/asyncapi/_builder.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/asyncapi/docs.py
--rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.1.2/kaflow/asyncapi/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/key_value.proto
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/key_value_pb2.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/key_value_pb2.pyi
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/test_application.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/test_serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/_utils/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/_utils/test_asyncio.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.1.2/tests/_utils/test_inspect.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.1.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.1.2/LICENSE
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 kaflow-0.1.2/README.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 kaflow-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 kaflow-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 kaflow-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 kaflow-0.1.3/Makefile
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 kaflow-0.1.3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 kaflow-0.1.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/__init__.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/_consumer.py
+-rw-r--r--   0        0        0    21884 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/applications.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/dependencies.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/exceptions.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/logger.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/message.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/py.typed
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/serializers.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/_utils/__init__.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/_utils/asyncio.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/_utils/inspect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/asyncapi/__init__.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/asyncapi/_builder.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/asyncapi/docs.py
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 kaflow-0.1.3/kaflow/asyncapi/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/key_value.proto
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/key_value_pb2.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/key_value_pb2.pyi
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/test_application.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/test_serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/_utils/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/_utils/test_asyncio.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 kaflow-0.1.3/tests/_utils/test_inspect.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 kaflow-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 kaflow-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 kaflow-0.1.3/README.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 kaflow-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3323 2020-02-02 00:00:00.000000 kaflow-0.1.3/PKG-INFO
```

### Comparing `kaflow-0.1.2/.github/workflows/release.yaml` & `kaflow-0.1.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/.github/workflows/test.yaml` & `kaflow-0.1.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/kaflow/__init__.py` & `kaflow-0.1.3/kaflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,8 @@
     __all__.append("Avro")
 
 if has_protobuf:
     from kaflow.serializers import Protobuf  # noqa: F401
 
     __all__.append("Protobuf")
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `kaflow-0.1.2/kaflow/_consumer.py` & `kaflow-0.1.3/kaflow/_consumer.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/kaflow/applications.py` & `kaflow-0.1.3/kaflow/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,17 @@
         max_poll_interval_ms: int = 300000,
         rebalance_timeout_ms: int | None = None,
         session_timeout_ms: int = 10000,
         heartbeat_interval_ms: int = 3000,
         consumer_timeout_ms: int = 200,
         max_poll_records: int | None = None,
         kafka_api_version: str = "auto",
-        security_protocol: Literal["PLAINTEXT", "SSL"] = "PLAINTEXT",
+        security_protocol: Literal[
+            "PLAINTEXT", "SSL", "SASL_PLAINTEXT", "SASL_SSL"
+        ] = "PLAINTEXT",
         exclude_internal_topics: bool = True,
         connection_max_idle_ms: int = 540000,
         isolation_level: Literal[
             "read_committed", "read_uncommitted"
         ] = "read_committed",
         cafile: str | None = None,
         capath: str | None = None,
```

### Comparing `kaflow-0.1.2/kaflow/message.py` & `kaflow-0.1.3/kaflow/message.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/kaflow/parameters.py` & `kaflow-0.1.3/kaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/kaflow/serializers.py` & `kaflow-0.1.3/kaflow/serializers.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,24 +70,36 @@
 
 Json = Annotated[T, JsonSerializer, MESSAGE_SERIALIZER_FLAG]
 
 
 if has_fastavro:
 
     class AvroSerializer(Serializer):
-        def __init__(self, avro_schema: dict[str, Any], **kwargs: Any) -> None:
+        def __init__(
+            self,
+            avro_schema: dict[str, Any] | None = None,
+            include_schema: bool = False,
+            **kwargs: Any,
+        ) -> None:
             self.avro_schema = avro_schema
+            self.include_schema = include_schema
 
         def serialize(self, data: Any) -> bytes:
             bytes_io = io.BytesIO()
-            fastavro.schemaless_writer(bytes_io, self.avro_schema, data)
+            if self.include_schema:
+                fastavro.writer(bytes_io, self.avro_schema, [data])
+            else:
+                fastavro.schemaless_writer(bytes_io, self.avro_schema, data)
             return bytes_io.getvalue()
 
         def deserialize(self, data: bytes) -> Any:
-            return fastavro.schemaless_reader(io.BytesIO(data), self.avro_schema)
+            bytes_io = io.BytesIO(data)
+            if self.avro_schema:
+                return fastavro.schemaless_reader(io.BytesIO(data), self.avro_schema)
+            return list(fastavro.reader(bytes_io))[0]
 
         @staticmethod
         def extra_annotations_keys() -> list[str]:
             return ["avro_schema"]
 
     Avro = Annotated[T, AvroSerializer, MESSAGE_SERIALIZER_FLAG]
```

### Comparing `kaflow-0.1.2/kaflow/_utils/asyncio.py` & `kaflow-0.1.3/kaflow/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/kaflow/_utils/inspect.py` & `kaflow-0.1.3/kaflow/_utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/kaflow/asyncapi/_builder.py` & `kaflow-0.1.3/kaflow/asyncapi/_builder.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/kaflow/asyncapi/docs.py` & `kaflow-0.1.3/kaflow/asyncapi/docs.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/kaflow/asyncapi/models.py` & `kaflow-0.1.3/kaflow/asyncapi/models.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/tests/key_value_pb2.py` & `kaflow-0.1.3/tests/key_value_pb2.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/tests/test_serializers.py` & `kaflow-0.1.3/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/tests/_utils/test_inspect.py` & `kaflow-0.1.3/tests/_utils/test_inspect.py`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/.gitignore` & `kaflow-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/LICENSE` & `kaflow-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/README.md` & `kaflow-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/pyproject.toml` & `kaflow-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kaflow-0.1.2/PKG-INFO` & `kaflow-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaflow
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Stream processing backed by Apache Kafka.
 Project-URL: Documentation, https://github.com/gabrielmbmb/kaflow#readme
 Project-URL: Issues, https://github.com/gabrielmbmb/kaflow/issues
 Project-URL: Source, https://github.com/gabrielmbmb/kaflow
 Author-email: Gabriel Martin Blazquez <gmartinbdev@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
```

