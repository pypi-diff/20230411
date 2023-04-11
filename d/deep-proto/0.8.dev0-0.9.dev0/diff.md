# Comparing `tmp/deep_proto-0.8.dev0.tar.gz` & `tmp/deep_proto-0.9.dev0.tar.gz`

## Comparing `deep_proto-0.8.dev0.tar` & `deep_proto-0.9.dev0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/src/deepproto/proto/common/v1/common_pb2.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/src/deepproto/proto/poll/v1/poll_pb2.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/src/deepproto/proto/poll/v1/poll_pb2_grpc.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/src/deepproto/proto/resource/v1/resource_pb2.py
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2_grpc.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/.gitignore
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/pyproject.toml
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/../../README.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 deep_proto-0.8.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/common/v1/common_pb2.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/poll/v1/poll_pb2.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/poll/v1/poll_pb2_grpc.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/resource/v1/resource_pb2.py
+-rw-r--r--   0        0        0     5182 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2_grpc.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/.gitignore
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/pyproject.toml
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/../../README.md
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 deep_proto-0.9.dev0/PKG-INFO
```

### Comparing `deep_proto-0.8.dev0/src/deepproto/proto/common/v1/common_pb2.py` & `deep_proto-0.9.dev0/src/deepproto/proto/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `deep_proto-0.8.dev0/src/deepproto/proto/poll/v1/poll_pb2.py` & `deep_proto-0.9.dev0/src/deepproto/proto/poll/v1/poll_pb2.py`

 * *Files identical despite different names*

### Comparing `deep_proto-0.8.dev0/src/deepproto/proto/poll/v1/poll_pb2_grpc.py` & `deep_proto-0.9.dev0/src/deepproto/proto/poll/v1/poll_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `deep_proto-0.8.dev0/src/deepproto/proto/resource/v1/resource_pb2.py` & `deep_proto-0.9.dev0/src/deepproto/proto/resource/v1/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `deep_proto-0.8.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2.py` & `deep_proto-0.9.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from deepproto.proto.common.v1 import common_pb2 as deepproto_dot_proto_dot_common_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.deepproto/proto/tracepoint/v1/tracepoint.proto\x12\x1d\x64\x65\x65pproto.proto.tracepoint.v1\x1a&deepproto/proto/common/v1/common.proto\"\xc4\x01\n\x10TracePointConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0f\n\x07line_no\x18\x03 \x01(\x05\x12G\n\x04\x61rgs\x18\x04 \x03(\x0b\x32\x39.deepproto.proto.tracepoint.v1.TracePointConfig.ArgsEntry\x12\x0f\n\x07watches\x18\x05 \x03(\t\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"9\n\nVariableId\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tmodifiers\x18\x03 \x03(\t\"\x98\x01\n\x08Variable\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04hash\x18\x03 \x01(\t\x12;\n\x08\x63hildren\x18\x04 \x03(\x0b\x32).deepproto.proto.tracepoint.v1.VariableId\x12\x16\n\ttruncated\x18\x05 \x01(\x08H\x00\x88\x01\x01\x42\x0c\n\n_truncated\"\xe7\x03\n\nStackFrame\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x13\n\x0bline_number\x18\x03 \x01(\x05\x12\x17\n\nclass_name\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08is_async\x18\x05 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\rcolumn_number\x18\x06 \x01(\x05H\x02\x88\x01\x01\x12!\n\x14transpiled_file_name\x18\x07 \x01(\tH\x03\x88\x01\x01\x12#\n\x16transpiled_line_number\x18\x08 \x01(\tH\x04\x88\x01\x01\x12%\n\x18transpiled_column_number\x18\t \x01(\tH\x05\x88\x01\x01\x12<\n\tvariables\x18\n \x03(\x0b\x32).deepproto.proto.tracepoint.v1.VariableId\x12\x16\n\tapp_frame\x18\x0b \x01(\x08H\x06\x88\x01\x01\x42\r\n\x0b_class_nameB\x0b\n\t_is_asyncB\x10\n\x0e_column_numberB\x17\n\x15_transpiled_file_nameB\x19\n\x17_transpiled_line_numberB\x1b\n\x19_transpiled_column_numberB\x0c\n\n_app_frame\"\\\n\x0bWatchResult\x12\x12\n\nexpression\x18\x01 \x01(\t\x12\x39\n\x06result\x18\x02 \x01(\x0b\x32).deepproto.proto.tracepoint.v1.VariableId\"\x8e\x04\n\x08Snapshot\x12\n\n\x02id\x18\x01 \x01(\t\x12\x43\n\ntracepoint\x18\x02 \x01(\x0b\x32/.deepproto.proto.tracepoint.v1.TracePointConfig\x12J\n\nvar_lookup\x18\x03 \x03(\x0b\x32\x36.deepproto.proto.tracepoint.v1.Snapshot.VarLookupEntry\x12\n\n\x02ts\x18\x04 \x01(\x03\x12\x39\n\x06\x66rames\x18\x05 \x03(\x0b\x32).deepproto.proto.tracepoint.v1.StackFrame\x12;\n\x07watches\x18\x06 \x03(\x0b\x32*.deepproto.proto.tracepoint.v1.WatchResult\x12\x37\n\nattributes\x18\x07 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x12\x16\n\x0enanos_duration\x18\x08 \x01(\x03\x12\x35\n\x08resource\x18\t \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x1aY\n\x0eVarLookupEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.deepproto.proto.tracepoint.v1.Variable:\x02\x38\x01\"\x12\n\x10SnapshotResponse2u\n\x0fSnapshotService\x12\x62\n\x04send\x12\'.deepproto.proto.tracepoint.v1.Snapshot\x1a/.deepproto.proto.tracepoint.v1.SnapshotResponse\"\x00\x42\x64\n&com.intergral.deep.proto.tracepoint.v1P\x01Z8github.com/intergral/deep-proto/proto/deep/tracepoint/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.deepproto/proto/tracepoint/v1/tracepoint.proto\x12\x1d\x64\x65\x65pproto.proto.tracepoint.v1\x1a&deepproto/proto/common/v1/common.proto\"\xc4\x01\n\x10TracePointConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\x12\x0f\n\x07line_no\x18\x03 \x01(\x05\x12G\n\x04\x61rgs\x18\x04 \x03(\x0b\x32\x39.deepproto.proto.tracepoint.v1.TracePointConfig.ArgsEntry\x12\x0f\n\x07watches\x18\x05 \x03(\t\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"9\n\nVariableId\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tmodifiers\x18\x03 \x03(\t\"\x98\x01\n\x08Variable\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04hash\x18\x03 \x01(\t\x12;\n\x08\x63hildren\x18\x04 \x03(\x0b\x32).deepproto.proto.tracepoint.v1.VariableId\x12\x16\n\ttruncated\x18\x05 \x01(\x08H\x00\x88\x01\x01\x42\x0c\n\n_truncated\"\xe7\x03\n\nStackFrame\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x13\n\x0bmethod_name\x18\x02 \x01(\t\x12\x13\n\x0bline_number\x18\x03 \x01(\x05\x12\x17\n\nclass_name\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08is_async\x18\x05 \x01(\x08H\x01\x88\x01\x01\x12\x1a\n\rcolumn_number\x18\x06 \x01(\x05H\x02\x88\x01\x01\x12!\n\x14transpiled_file_name\x18\x07 \x01(\tH\x03\x88\x01\x01\x12#\n\x16transpiled_line_number\x18\x08 \x01(\x05H\x04\x88\x01\x01\x12%\n\x18transpiled_column_number\x18\t \x01(\x05H\x05\x88\x01\x01\x12<\n\tvariables\x18\n \x03(\x0b\x32).deepproto.proto.tracepoint.v1.VariableId\x12\x16\n\tapp_frame\x18\x0b \x01(\x08H\x06\x88\x01\x01\x42\r\n\x0b_class_nameB\x0b\n\t_is_asyncB\x10\n\x0e_column_numberB\x17\n\x15_transpiled_file_nameB\x19\n\x17_transpiled_line_numberB\x1b\n\x19_transpiled_column_numberB\x0c\n\n_app_frame\"\x85\x01\n\x0bWatchResult\x12\x12\n\nexpression\x18\x01 \x01(\t\x12@\n\x0bgood_result\x18\x02 \x01(\x0b\x32).deepproto.proto.tracepoint.v1.VariableIdH\x00\x12\x16\n\x0c\x65rror_result\x18\x03 \x01(\tH\x00\x42\x08\n\x06result\"\x8e\x04\n\x08Snapshot\x12\n\n\x02id\x18\x01 \x01(\t\x12\x43\n\ntracepoint\x18\x02 \x01(\x0b\x32/.deepproto.proto.tracepoint.v1.TracePointConfig\x12J\n\nvar_lookup\x18\x03 \x03(\x0b\x32\x36.deepproto.proto.tracepoint.v1.Snapshot.VarLookupEntry\x12\n\n\x02ts\x18\x04 \x01(\x03\x12\x39\n\x06\x66rames\x18\x05 \x03(\x0b\x32).deepproto.proto.tracepoint.v1.StackFrame\x12;\n\x07watches\x18\x06 \x03(\x0b\x32*.deepproto.proto.tracepoint.v1.WatchResult\x12\x37\n\nattributes\x18\x07 \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x12\x16\n\x0enanos_duration\x18\x08 \x01(\x03\x12\x35\n\x08resource\x18\t \x03(\x0b\x32#.deepproto.proto.common.v1.KeyValue\x1aY\n\x0eVarLookupEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.deepproto.proto.tracepoint.v1.Variable:\x02\x38\x01\"\x12\n\x10SnapshotResponse2u\n\x0fSnapshotService\x12\x62\n\x04send\x12\'.deepproto.proto.tracepoint.v1.Snapshot\x1a/.deepproto.proto.tracepoint.v1.SnapshotResponse\"\x00\x42\x64\n&com.intergral.deep.proto.tracepoint.v1P\x01Z8github.com/intergral/deep-proto/proto/deep/tracepoint/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'deepproto.proto.tracepoint.v1.tracepoint_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n&com.intergral.deep.proto.tracepoint.v1P\001Z8github.com/intergral/deep-proto/proto/deep/tracepoint/v1'
@@ -32,18 +32,18 @@
   _TRACEPOINTCONFIG_ARGSENTRY._serialized_end=318
   _VARIABLEID._serialized_start=320
   _VARIABLEID._serialized_end=377
   _VARIABLE._serialized_start=380
   _VARIABLE._serialized_end=532
   _STACKFRAME._serialized_start=535
   _STACKFRAME._serialized_end=1022
-  _WATCHRESULT._serialized_start=1024
-  _WATCHRESULT._serialized_end=1116
-  _SNAPSHOT._serialized_start=1119
-  _SNAPSHOT._serialized_end=1645
-  _SNAPSHOT_VARLOOKUPENTRY._serialized_start=1556
-  _SNAPSHOT_VARLOOKUPENTRY._serialized_end=1645
-  _SNAPSHOTRESPONSE._serialized_start=1647
-  _SNAPSHOTRESPONSE._serialized_end=1665
-  _SNAPSHOTSERVICE._serialized_start=1667
-  _SNAPSHOTSERVICE._serialized_end=1784
+  _WATCHRESULT._serialized_start=1025
+  _WATCHRESULT._serialized_end=1158
+  _SNAPSHOT._serialized_start=1161
+  _SNAPSHOT._serialized_end=1687
+  _SNAPSHOT_VARLOOKUPENTRY._serialized_start=1598
+  _SNAPSHOT_VARLOOKUPENTRY._serialized_end=1687
+  _SNAPSHOTRESPONSE._serialized_start=1689
+  _SNAPSHOTRESPONSE._serialized_end=1707
+  _SNAPSHOTSERVICE._serialized_start=1709
+  _SNAPSHOTSERVICE._serialized_end=1826
 # @@protoc_insertion_point(module_scope)
```

### Comparing `deep_proto-0.8.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2_grpc.py` & `deep_proto-0.9.dev0/src/deepproto/proto/tracepoint/v1/tracepoint_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `deep_proto-0.8.dev0/pyproject.toml` & `deep_proto-0.9.dev0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
 dependencies = []
-version = "0.8-dev"
+version = "0.9-dev"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "src/deepproto",
 ]
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `deep_proto-0.8.dev0/PKG-INFO` & `deep_proto-0.9.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-proto
-Version: 0.8.dev0
+Version: 0.9.dev0
 Summary: DEEP Python Protobuf
 Author-email: Ben Donnelly <b.w.donnelly1@gmail.com>
 License-Expression: Apache-2.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

