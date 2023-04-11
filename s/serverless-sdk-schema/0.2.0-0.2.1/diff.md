# Comparing `tmp/serverless-sdk-schema-0.2.0.tar.gz` & `tmp/serverless-sdk-schema-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk-schema/dist/.tmp-aobt1e6y/serverless-sdk-schema-0.2.0.tar", last modified: Wed Mar 29 07:14:45 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk-schema/dist/.tmp-t5i1vddo/serverless-sdk-schema-0.2.1.tar", last modified: Tue Apr 11 20:27:52 2023, max compression
```

## Comparing `serverless-sdk-schema-0.2.0.tar` & `serverless-sdk-schema-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-29 07:14:28.000000 serverless-sdk-schema-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-29 07:14:28.000000 serverless-sdk-schema-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-29 07:14:28.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    10819 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/notice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/tags_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/warning_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/dev_mode_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/event_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/request_response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-03-29 07:14:32.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/trace_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/serverless_sdk_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 07:14:45.000000 serverless-sdk-schema-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-03-29 07:14:28.000000 serverless-sdk-schema-0.2.0/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-11 20:27:30.000000 serverless-sdk-schema-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-11 20:27:30.000000 serverless-sdk-schema-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-11 20:27:30.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/notice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/tags_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/warning_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/dev_mode_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/event_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/request_response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-11 20:27:36.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/trace_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 20:27:52.000000 serverless-sdk-schema-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-11 20:27:30.000000 serverless-sdk-schema-0.2.1/tests/test_schema.py
```

### Comparing `serverless-sdk-schema-0.2.0/PKG-INFO` & `serverless-sdk-schema-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk-schema
-Version: 0.2.0
+Version: 0.2.1
 Summary: The protobuf generated Serverless SDK Schema
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk-schema/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk-schema
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-schema-0.2.0/README.md` & `serverless-sdk-schema-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/pyproject.toml` & `serverless-sdk-schema-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
     "setuptools>=65.6.3",
     "wheel",
 ]
 
 [project]
 name = "serverless-sdk-schema"
-version = "0.2.0"
+version = "0.2.1"
 description = "The protobuf generated Serverless SDK Schema"
 readme = "README.md"
 authors = [{ name = "serverlessinc" }]
 requires-python = ">=3.7"
 dependencies = [
     "protobuf>=4.22",
     "typing-extensions>=4.4", # included in Python 3.8 - 3.11
```

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/aws_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from serverless.instrumentation.tags.v1 import common_pb2 as serverless_dot_instrumentation_dot_tags_dot_v1_dot_common__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,serverless/instrumentation/tags/v1/aws.proto\x12\"serverless.instrumentation.tags.v1\x1a/serverless/instrumentation/tags/v1/common.proto\"\x96\x04\n\x07\x41wsTags\x12N\n\x06lambda\x18\x64 \x01(\x0b\x32\x31.serverless.instrumentation.tags.v1.AwsLambdaTagsH\x00R\x06lambda\x88\x01\x01\x12\x45\n\x03sdk\x18\x65 \x01(\x0b\x32..serverless.instrumentation.tags.v1.AwsSdkTagsH\x01R\x03sdk\x88\x01\x01\x12\"\n\naccount_id\x18\x66 \x01(\tH\x02R\taccountId\x88\x01\x01\x12\x1b\n\x06region\x18g \x01(\tH\x03R\x06region\x88\x01\x01\x12\"\n\nrequest_id\x18h \x01(\tH\x04R\trequestId\x88\x01\x01\x12(\n\rresource_name\x18i \x01(\tH\x05R\x0cresourceName\x88\x01\x01\x12$\n\x0bsequence_id\x18\x03 \x01(\tH\x06R\nsequenceId\x88\x01\x01\x12 \n\tlog_group\x18\x04 \x01(\tH\x07R\x08logGroup\x88\x01\x01\x12\"\n\nlog_stream\x18\x05 \x01(\tH\x08R\tlogStream\x88\x01\x01\x42\t\n\x07_lambdaB\x06\n\x04_sdkB\r\n\x0b_account_idB\t\n\x07_regionB\r\n\x0b_request_idB\x10\n\x0e_resource_nameB\x0e\n\x0c_sequence_idB\x0c\n\n_log_groupB\r\n\x0b_log_stream\"\xe5\x02\n\x11\x41wsApiGatewayTags\x12\x1d\n\naccount_id\x18\x01 \x01(\tR\taccountId\x12\x15\n\x06\x61pi_id\x18\x02 \x01(\tR\x05\x61piId\x12\x1b\n\tapi_stage\x18\x03 \x01(\tR\x08\x61piStage\x12h\n\x07request\x18\x0f \x01(\x0b\x32N.serverless.instrumentation.tags.v1.AwsApiGatewayTags.AwsApiGatewayRequestTagsR\x07request\x1a\x92\x01\n\x18\x41wsApiGatewayRequestTags\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\ntime_epoch\x18\x02 \x01(\x04R\ttimeEpoch\x12\x30\n\x14path_parameter_names\x18\x04 \x03(\tR\x12pathParameterNamesJ\x04\x08\x03\x10\x04R\x0fpath_parameters\"\xde\x0e\n\rAwsLambdaTags\x12\x12\n\x04\x61rch\x18\x01 \x01(\tR\x04\x61rch\x12!\n\x0cis_coldstart\x18\x02 \x01(\x08R\x0bisColdstart\x12\"\n\nevent_type\x18\x03 \x01(\tH\x00R\teventType\x88\x01\x01\x12&\n\x0c\x65vent_source\x18\x04 \x01(\tH\x01R\x0b\x65ventSource\x88\x01\x01\x12 \n\tlog_group\x18\x05 \x01(\tH\x02R\x08logGroup\x88\x01\x01\x12+\n\x0flog_stream_name\x18\x06 \x01(\tH\x03R\rlogStreamName\x88\x01\x01\x12\"\n\nmax_memory\x18\x07 \x01(\rH\x04R\tmaxMemory\x88\x01\x01\x12\x12\n\x04name\x18\x08 \x01(\tR\x04name\x12\x1d\n\nrequest_id\x18\t \x01(\tR\trequestId\x12\x18\n\x07version\x18\x0b \x01(\tR\x07version\x12\"\n\naccount_id\x18\x0c \x01(\tH\x05R\taccountId\x88\x01\x01\x12S\n\x07outcome\x18\x0e \x01(\x0e\x32\x39.serverless.instrumentation.tags.v1.AwsLambdaTags.OutcomeR\x07outcome\x12;\n\x17\x65rror_exception_message\x18\x0f \x01(\tH\x06R\x15\x65rrorExceptionMessage\x88\x01\x01\x12\x41\n\x1a\x65rror_exception_stacktrace\x18\x10 \x01(\tH\x07R\x18\x65rrorExceptionStacktrace\x88\x01\x01\x12\x1f\n\x08\x64uration\x18\x11 \x01(\rH\x08R\x08\x64uration\x88\x01\x01\x12&\n\x0crequest_body\x18\x12 \x01(\tH\tR\x0brequestBody\x88\x01\x01\x12(\n\rresponse_body\x18\x13 \x01(\tH\nR\x0cresponseBody\x88\x01\x01\x12J\n\x03sqs\x18\x64 \x01(\x0b\x32\x33.serverless.instrumentation.tags.v1.AwsSqsEventTagsH\x0bR\x03sqs\x88\x01\x01\x12J\n\x03sns\x18\x65 \x01(\x0b\x32\x33.serverless.instrumentation.tags.v1.AwsSnsEventTagsH\x0cR\x03sns\x88\x01\x01\x12\x45\n\x04http\x18\x66 \x01(\x0b\x32,.serverless.instrumentation.tags.v1.HttpTagsH\rR\x04http\x88\x01\x01\x12[\n\x0b\x61pi_gateway\x18g \x01(\x0b\x32\x35.serverless.instrumentation.tags.v1.AwsApiGatewayTagsH\x0eR\napiGateway\x88\x01\x01\x12X\n\x0bhttp_router\x18j \x01(\x0b\x32\x32.serverless.instrumentation.tags.v1.HttpRouterTagsH\x0fR\nhttpRouter\x88\x01\x01\x12l\n\x0einitialization\x18h \x01(\x0b\x32?.serverless.instrumentation.tags.v1.AwsLambdaInitializationTagsH\x10R\x0einitialization\x88\x01\x01\x12`\n\ninvocation\x18i \x01(\x0b\x32;.serverless.instrumentation.tags.v1.AwsLambdaInvocationTagsH\x11R\ninvocation\x88\x01\x01\x12W\n\x07runtime\x18k \x01(\x0b\x32\x38.serverless.instrumentation.tags.v1.AwsLambdaRuntimeTagsH\x12R\x07runtime\x88\x01\x01\"\xac\x01\n\x07Outcome\x12\x17\n\x13OUTCOME_UNSPECIFIED\x10\x00\x12\x13\n\x0fOUTCOME_SUCCESS\x10\x01\x12 \n\x1cOUTCOME_ERROR_INITIALIZATION\x10\x02\x12\x1b\n\x17OUTCOME_ERROR_UNHANDLED\x10\x03\x12\x19\n\x15OUTCOME_ERROR_TIMEOUT\x10\x04\x12\x19\n\x15OUTCOME_ERROR_HANDLED\x10\x05\x42\r\n\x0b_event_typeB\x0f\n\r_event_sourceB\x0c\n\n_log_groupB\x12\n\x10_log_stream_nameB\r\n\x0b_max_memoryB\r\n\x0b_account_idB\x1a\n\x18_error_exception_messageB\x1d\n\x1b_error_exception_stacktraceB\x0b\n\t_durationB\x0f\n\r_request_bodyB\x10\n\x0e_response_bodyB\x06\n\x04_sqsB\x06\n\x04_snsB\x07\n\x05_httpB\x0e\n\x0c_api_gatewayB\x0e\n\x0c_http_routerB\x11\n\x0f_initializationB\r\n\x0b_invocationB\n\n\x08_runtime\"$\n\x0eHttpRouterTags\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"Q\n\x0f\x41wsSqsEventTags\x12\x1d\n\nqueue_name\x18\x01 \x01(\tR\tqueueName\x12\x1f\n\x0bmessage_ids\x18\x02 \x03(\tR\nmessageIds\"Q\n\x0f\x41wsSnsEventTags\x12\x1d\n\ntopic_name\x18\x01 \x01(\tR\ttopicName\x12\x1f\n\x0bmessage_ids\x18\x02 \x03(\tR\nmessageIds\"b\n\x14\x41wsLambdaRuntimeTags\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\x12\x18\n\x07version\x18\x02 \x01(\tR\x07version\x12\x10\n\x03\x61rn\x18\x03 \x01(\tR\x03\x61rn\"V\n\x1b\x41wsLambdaInitializationTags\x12\x37\n\x17initialization_duration\x18\x01 \x01(\rR\x16initializationDuration\"J\n\x17\x41wsLambdaInvocationTags\x12/\n\x13invocation_duration\x18\x01 \x01(\rR\x12invocationDuration\"\xd1\x04\n\nAwsSdkTags\x12\x1b\n\x06region\x18\x02 \x01(\tH\x00R\x06region\x88\x01\x01\x12\x30\n\x11signature_version\x18\x03 \x01(\tH\x01R\x10signatureVersion\x88\x01\x01\x12\x18\n\x07service\x18\x04 \x01(\tR\x07service\x12\x1c\n\toperation\x18\x05 \x01(\tR\toperation\x12\"\n\nrequest_id\x18\x06 \x01(\tH\x02R\trequestId\x88\x01\x01\x12\x19\n\x05\x65rror\x18\x07 \x01(\tH\x03R\x05\x65rror\x88\x01\x01\x12W\n\x08\x64ynamodb\x18\x64 \x01(\x0b\x32\x36.serverless.instrumentation.tags.v1.AwsSdkDynamodbTagsH\x04R\x08\x64ynamodb\x88\x01\x01\x12H\n\x03sqs\x18\x65 \x01(\x0b\x32\x31.serverless.instrumentation.tags.v1.AwsSdkSqsTagsH\x05R\x03sqs\x88\x01\x01\x12H\n\x03sns\x18\x66 \x01(\x0b\x32\x31.serverless.instrumentation.tags.v1.AwsSdkSnsTagsH\x06R\x03sns\x88\x01\x01\x42\t\n\x07_regionB\x14\n\x12_signature_versionB\r\n\x0b_request_idB\x08\n\x06_errorB\x0b\n\t_dynamodbB\x06\n\x04_sqsB\x06\n\x04_snsJ\x04\x08\x01\x10\x02J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nR\naccount_idR\x0crequest_bodyR\rresponse_body\"\xe3\x06\n\x12\x41wsSdkDynamodbTags\x12\"\n\ntable_name\x18\x01 \x01(\tH\x00R\ttableName\x88\x01\x01\x12#\n\nprojection\x18\x02 \x01(\tH\x01R\nprojection\x88\x01\x01\x12&\n\x0cscan_forward\x18\x03 \x01(\x08H\x02R\x0bscanForward\x88\x01\x01\x12*\n\x11\x61ttributes_to_get\x18\x04 \x03(\tR\x0f\x61ttributesToGet\x12,\n\x0f\x63onsistent_read\x18\x05 \x01(\x08H\x03R\x0e\x63onsistentRead\x88\x01\x01\x12\"\n\nindex_name\x18\x06 \x01(\tH\x04R\tindexName\x88\x01\x01\x12\x19\n\x05limit\x18\x07 \x01(\rH\x05R\x05limit\x88\x01\x01\x12\x1b\n\x06select\x18\x08 \x01(\tH\x06R\x06select\x88\x01\x01\x12\x1d\n\x07segment\x18\t \x01(\rH\x07R\x07segment\x88\x01\x01\x12*\n\x0etotal_segments\x18\n \x01(\x04H\x08R\rtotalSegments\x88\x01\x01\x12\x1b\n\x06\x66ilter\x18\x0b \x01(\tH\tR\x06\x66ilter\x88\x01\x01\x12(\n\rkey_condition\x18\x0c \x01(\tH\nR\x0ckeyCondition\x88\x01\x01\x12\x33\n\x13\x65xclusive_start_key\x18\r \x01(\tH\x0bR\x11\x65xclusiveStartKey\x88\x01\x01\x12.\n\x10\x61ttribute_values\x18\x0e \x01(\tH\x0cR\x0f\x61ttributeValues\x88\x01\x01\x12\x19\n\x05\x63ount\x18\x64 \x01(\x04H\rR\x05\x63ount\x88\x01\x01\x12(\n\rscanned_count\x18\x65 \x01(\x04H\x0eR\x0cscannedCount\x88\x01\x01\x42\r\n\x0b_table_nameB\r\n\x0b_projectionB\x0f\n\r_scan_forwardB\x12\n\x10_consistent_readB\r\n\x0b_index_nameB\x08\n\x06_limitB\t\n\x07_selectB\n\n\x08_segmentB\x11\n\x0f_total_segmentsB\t\n\x07_filterB\x10\n\x0e_key_conditionB\x16\n\x14_exclusive_start_keyB\x13\n\x11_attribute_valuesB\x08\n\x06_countB\x10\n\x0e_scanned_count\"c\n\rAwsSdkSqsTags\x12\"\n\nqueue_name\x18\x01 \x01(\tH\x00R\tqueueName\x88\x01\x01\x12\x1f\n\x0bmessage_ids\x18\x02 \x03(\tR\nmessageIdsB\r\n\x0b_queue_name\"c\n\rAwsSdkSnsTags\x12\"\n\ntopic_name\x18\x01 \x01(\tH\x00R\ttopicName\x88\x01\x01\x12\x1f\n\x0bmessage_ids\x18\x02 \x03(\tR\nmessageIdsB\r\n\x0b_topic_nameB\nZ\x08.;protocb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,serverless/instrumentation/tags/v1/aws.proto\x12\"serverless.instrumentation.tags.v1\x1a/serverless/instrumentation/tags/v1/common.proto\"\x96\x04\n\x07\x41wsTags\x12N\n\x06lambda\x18\x64 \x01(\x0b\x32\x31.serverless.instrumentation.tags.v1.AwsLambdaTagsH\x00R\x06lambda\x88\x01\x01\x12\x45\n\x03sdk\x18\x65 \x01(\x0b\x32..serverless.instrumentation.tags.v1.AwsSdkTagsH\x01R\x03sdk\x88\x01\x01\x12\"\n\naccount_id\x18\x66 \x01(\tH\x02R\taccountId\x88\x01\x01\x12\x1b\n\x06region\x18g \x01(\tH\x03R\x06region\x88\x01\x01\x12\"\n\nrequest_id\x18h \x01(\tH\x04R\trequestId\x88\x01\x01\x12(\n\rresource_name\x18i \x01(\tH\x05R\x0cresourceName\x88\x01\x01\x12$\n\x0bsequence_id\x18\x03 \x01(\tH\x06R\nsequenceId\x88\x01\x01\x12 \n\tlog_group\x18\x04 \x01(\tH\x07R\x08logGroup\x88\x01\x01\x12\"\n\nlog_stream\x18\x05 \x01(\tH\x08R\tlogStream\x88\x01\x01\x42\t\n\x07_lambdaB\x06\n\x04_sdkB\r\n\x0b_account_idB\t\n\x07_regionB\r\n\x0b_request_idB\x10\n\x0e_resource_nameB\x0e\n\x0c_sequence_idB\x0c\n\n_log_groupB\r\n\x0b_log_stream\"\xe5\x02\n\x11\x41wsApiGatewayTags\x12\x1d\n\naccount_id\x18\x01 \x01(\tR\taccountId\x12\x15\n\x06\x61pi_id\x18\x02 \x01(\tR\x05\x61piId\x12\x1b\n\tapi_stage\x18\x03 \x01(\tR\x08\x61piStage\x12h\n\x07request\x18\x0f \x01(\x0b\x32N.serverless.instrumentation.tags.v1.AwsApiGatewayTags.AwsApiGatewayRequestTagsR\x07request\x1a\x92\x01\n\x18\x41wsApiGatewayRequestTags\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1d\n\ntime_epoch\x18\x02 \x01(\x04R\ttimeEpoch\x12\x30\n\x14path_parameter_names\x18\x04 \x03(\tR\x12pathParameterNamesJ\x04\x08\x03\x10\x04R\x0fpath_parameters\"\xf6\x0f\n\rAwsLambdaTags\x12\x12\n\x04\x61rch\x18\x01 \x01(\tR\x04\x61rch\x12!\n\x0cis_coldstart\x18\x02 \x01(\x08R\x0bisColdstart\x12\"\n\nevent_type\x18\x03 \x01(\tH\x00R\teventType\x88\x01\x01\x12&\n\x0c\x65vent_source\x18\x04 \x01(\tH\x01R\x0b\x65ventSource\x88\x01\x01\x12 \n\tlog_group\x18\x05 \x01(\tH\x02R\x08logGroup\x88\x01\x01\x12+\n\x0flog_stream_name\x18\x06 \x01(\tH\x03R\rlogStreamName\x88\x01\x01\x12\"\n\nmax_memory\x18\x07 \x01(\rH\x04R\tmaxMemory\x88\x01\x01\x12\x12\n\x04name\x18\x08 \x01(\tR\x04name\x12\x1d\n\nrequest_id\x18\t \x01(\tR\trequestId\x12\x18\n\x07version\x18\x0b \x01(\tR\x07version\x12\"\n\naccount_id\x18\x0c \x01(\tH\x05R\taccountId\x88\x01\x01\x12S\n\x07outcome\x18\x0e \x01(\x0e\x32\x39.serverless.instrumentation.tags.v1.AwsLambdaTags.OutcomeR\x07outcome\x12;\n\x17\x65rror_exception_message\x18\x0f \x01(\tH\x06R\x15\x65rrorExceptionMessage\x88\x01\x01\x12\x41\n\x1a\x65rror_exception_stacktrace\x18\x10 \x01(\tH\x07R\x18\x65rrorExceptionStacktrace\x88\x01\x01\x12\x1f\n\x08\x64uration\x18\x11 \x01(\rH\x08R\x08\x64uration\x88\x01\x01\x12&\n\x0crequest_body\x18\x12 \x01(\tH\tR\x0brequestBody\x88\x01\x01\x12(\n\rresponse_body\x18\x13 \x01(\tH\nR\x0cresponseBody\x88\x01\x01\x12\x34\n\x14logs_start_time_unix\x18\x14 \x01(\x04H\x0bR\x11logsStartTimeUnix\x88\x01\x01\x12\x30\n\x12logs_end_time_unix\x18\x15 \x01(\x04H\x0cR\x0flogsEndTimeUnix\x88\x01\x01\x12J\n\x03sqs\x18\x64 \x01(\x0b\x32\x33.serverless.instrumentation.tags.v1.AwsSqsEventTagsH\rR\x03sqs\x88\x01\x01\x12J\n\x03sns\x18\x65 \x01(\x0b\x32\x33.serverless.instrumentation.tags.v1.AwsSnsEventTagsH\x0eR\x03sns\x88\x01\x01\x12\x45\n\x04http\x18\x66 \x01(\x0b\x32,.serverless.instrumentation.tags.v1.HttpTagsH\x0fR\x04http\x88\x01\x01\x12[\n\x0b\x61pi_gateway\x18g \x01(\x0b\x32\x35.serverless.instrumentation.tags.v1.AwsApiGatewayTagsH\x10R\napiGateway\x88\x01\x01\x12X\n\x0bhttp_router\x18j \x01(\x0b\x32\x32.serverless.instrumentation.tags.v1.HttpRouterTagsH\x11R\nhttpRouter\x88\x01\x01\x12l\n\x0einitialization\x18h \x01(\x0b\x32?.serverless.instrumentation.tags.v1.AwsLambdaInitializationTagsH\x12R\x0einitialization\x88\x01\x01\x12`\n\ninvocation\x18i \x01(\x0b\x32;.serverless.instrumentation.tags.v1.AwsLambdaInvocationTagsH\x13R\ninvocation\x88\x01\x01\x12W\n\x07runtime\x18k \x01(\x0b\x32\x38.serverless.instrumentation.tags.v1.AwsLambdaRuntimeTagsH\x14R\x07runtime\x88\x01\x01\"\xac\x01\n\x07Outcome\x12\x17\n\x13OUTCOME_UNSPECIFIED\x10\x00\x12\x13\n\x0fOUTCOME_SUCCESS\x10\x01\x12 \n\x1cOUTCOME_ERROR_INITIALIZATION\x10\x02\x12\x1b\n\x17OUTCOME_ERROR_UNHANDLED\x10\x03\x12\x19\n\x15OUTCOME_ERROR_TIMEOUT\x10\x04\x12\x19\n\x15OUTCOME_ERROR_HANDLED\x10\x05\x42\r\n\x0b_event_typeB\x0f\n\r_event_sourceB\x0c\n\n_log_groupB\x12\n\x10_log_stream_nameB\r\n\x0b_max_memoryB\r\n\x0b_account_idB\x1a\n\x18_error_exception_messageB\x1d\n\x1b_error_exception_stacktraceB\x0b\n\t_durationB\x0f\n\r_request_bodyB\x10\n\x0e_response_bodyB\x17\n\x15_logs_start_time_unixB\x15\n\x13_logs_end_time_unixB\x06\n\x04_sqsB\x06\n\x04_snsB\x07\n\x05_httpB\x0e\n\x0c_api_gatewayB\x0e\n\x0c_http_routerB\x11\n\x0f_initializationB\r\n\x0b_invocationB\n\n\x08_runtime\"$\n\x0eHttpRouterTags\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\"Q\n\x0f\x41wsSqsEventTags\x12\x1d\n\nqueue_name\x18\x01 \x01(\tR\tqueueName\x12\x1f\n\x0bmessage_ids\x18\x02 \x03(\tR\nmessageIds\"Q\n\x0f\x41wsSnsEventTags\x12\x1d\n\ntopic_name\x18\x01 \x01(\tR\ttopicName\x12\x1f\n\x0bmessage_ids\x18\x02 \x03(\tR\nmessageIds\"b\n\x14\x41wsLambdaRuntimeTags\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\x12\x18\n\x07version\x18\x02 \x01(\tR\x07version\x12\x10\n\x03\x61rn\x18\x03 \x01(\tR\x03\x61rn\"V\n\x1b\x41wsLambdaInitializationTags\x12\x37\n\x17initialization_duration\x18\x01 \x01(\rR\x16initializationDuration\"J\n\x17\x41wsLambdaInvocationTags\x12/\n\x13invocation_duration\x18\x01 \x01(\rR\x12invocationDuration\"\xd1\x04\n\nAwsSdkTags\x12\x1b\n\x06region\x18\x02 \x01(\tH\x00R\x06region\x88\x01\x01\x12\x30\n\x11signature_version\x18\x03 \x01(\tH\x01R\x10signatureVersion\x88\x01\x01\x12\x18\n\x07service\x18\x04 \x01(\tR\x07service\x12\x1c\n\toperation\x18\x05 \x01(\tR\toperation\x12\"\n\nrequest_id\x18\x06 \x01(\tH\x02R\trequestId\x88\x01\x01\x12\x19\n\x05\x65rror\x18\x07 \x01(\tH\x03R\x05\x65rror\x88\x01\x01\x12W\n\x08\x64ynamodb\x18\x64 \x01(\x0b\x32\x36.serverless.instrumentation.tags.v1.AwsSdkDynamodbTagsH\x04R\x08\x64ynamodb\x88\x01\x01\x12H\n\x03sqs\x18\x65 \x01(\x0b\x32\x31.serverless.instrumentation.tags.v1.AwsSdkSqsTagsH\x05R\x03sqs\x88\x01\x01\x12H\n\x03sns\x18\x66 \x01(\x0b\x32\x31.serverless.instrumentation.tags.v1.AwsSdkSnsTagsH\x06R\x03sns\x88\x01\x01\x42\t\n\x07_regionB\x14\n\x12_signature_versionB\r\n\x0b_request_idB\x08\n\x06_errorB\x0b\n\t_dynamodbB\x06\n\x04_sqsB\x06\n\x04_snsJ\x04\x08\x01\x10\x02J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nR\naccount_idR\x0crequest_bodyR\rresponse_body\"\xe3\x06\n\x12\x41wsSdkDynamodbTags\x12\"\n\ntable_name\x18\x01 \x01(\tH\x00R\ttableName\x88\x01\x01\x12#\n\nprojection\x18\x02 \x01(\tH\x01R\nprojection\x88\x01\x01\x12&\n\x0cscan_forward\x18\x03 \x01(\x08H\x02R\x0bscanForward\x88\x01\x01\x12*\n\x11\x61ttributes_to_get\x18\x04 \x03(\tR\x0f\x61ttributesToGet\x12,\n\x0f\x63onsistent_read\x18\x05 \x01(\x08H\x03R\x0e\x63onsistentRead\x88\x01\x01\x12\"\n\nindex_name\x18\x06 \x01(\tH\x04R\tindexName\x88\x01\x01\x12\x19\n\x05limit\x18\x07 \x01(\rH\x05R\x05limit\x88\x01\x01\x12\x1b\n\x06select\x18\x08 \x01(\tH\x06R\x06select\x88\x01\x01\x12\x1d\n\x07segment\x18\t \x01(\rH\x07R\x07segment\x88\x01\x01\x12*\n\x0etotal_segments\x18\n \x01(\x04H\x08R\rtotalSegments\x88\x01\x01\x12\x1b\n\x06\x66ilter\x18\x0b \x01(\tH\tR\x06\x66ilter\x88\x01\x01\x12(\n\rkey_condition\x18\x0c \x01(\tH\nR\x0ckeyCondition\x88\x01\x01\x12\x33\n\x13\x65xclusive_start_key\x18\r \x01(\tH\x0bR\x11\x65xclusiveStartKey\x88\x01\x01\x12.\n\x10\x61ttribute_values\x18\x0e \x01(\tH\x0cR\x0f\x61ttributeValues\x88\x01\x01\x12\x19\n\x05\x63ount\x18\x64 \x01(\x04H\rR\x05\x63ount\x88\x01\x01\x12(\n\rscanned_count\x18\x65 \x01(\x04H\x0eR\x0cscannedCount\x88\x01\x01\x42\r\n\x0b_table_nameB\r\n\x0b_projectionB\x0f\n\r_scan_forwardB\x12\n\x10_consistent_readB\r\n\x0b_index_nameB\x08\n\x06_limitB\t\n\x07_selectB\n\n\x08_segmentB\x11\n\x0f_total_segmentsB\t\n\x07_filterB\x10\n\x0e_key_conditionB\x16\n\x14_exclusive_start_keyB\x13\n\x11_attribute_valuesB\x08\n\x06_countB\x10\n\x0e_scanned_count\"c\n\rAwsSdkSqsTags\x12\"\n\nqueue_name\x18\x01 \x01(\tH\x00R\tqueueName\x88\x01\x01\x12\x1f\n\x0bmessage_ids\x18\x02 \x03(\tR\nmessageIdsB\r\n\x0b_queue_name\"c\n\rAwsSdkSnsTags\x12\"\n\ntopic_name\x18\x01 \x01(\tH\x00R\ttopicName\x88\x01\x01\x12\x1f\n\x0bmessage_ids\x18\x02 \x03(\tR\nmessageIdsB\r\n\x0b_topic_nameB\nZ\x08.;protocb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'serverless.instrumentation.tags.v1.aws_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -26,31 +26,31 @@
   _globals['_AWSTAGS']._serialized_start=134
   _globals['_AWSTAGS']._serialized_end=668
   _globals['_AWSAPIGATEWAYTAGS']._serialized_start=671
   _globals['_AWSAPIGATEWAYTAGS']._serialized_end=1028
   _globals['_AWSAPIGATEWAYTAGS_AWSAPIGATEWAYREQUESTTAGS']._serialized_start=882
   _globals['_AWSAPIGATEWAYTAGS_AWSAPIGATEWAYREQUESTTAGS']._serialized_end=1028
   _globals['_AWSLAMBDATAGS']._serialized_start=1031
-  _globals['_AWSLAMBDATAGS']._serialized_end=2917
-  _globals['_AWSLAMBDATAGS_OUTCOME']._serialized_start=2439
-  _globals['_AWSLAMBDATAGS_OUTCOME']._serialized_end=2611
-  _globals['_HTTPROUTERTAGS']._serialized_start=2919
-  _globals['_HTTPROUTERTAGS']._serialized_end=2955
-  _globals['_AWSSQSEVENTTAGS']._serialized_start=2957
-  _globals['_AWSSQSEVENTTAGS']._serialized_end=3038
-  _globals['_AWSSNSEVENTTAGS']._serialized_start=3040
-  _globals['_AWSSNSEVENTTAGS']._serialized_end=3121
-  _globals['_AWSLAMBDARUNTIMETAGS']._serialized_start=3123
-  _globals['_AWSLAMBDARUNTIMETAGS']._serialized_end=3221
-  _globals['_AWSLAMBDAINITIALIZATIONTAGS']._serialized_start=3223
-  _globals['_AWSLAMBDAINITIALIZATIONTAGS']._serialized_end=3309
-  _globals['_AWSLAMBDAINVOCATIONTAGS']._serialized_start=3311
-  _globals['_AWSLAMBDAINVOCATIONTAGS']._serialized_end=3385
-  _globals['_AWSSDKTAGS']._serialized_start=3388
-  _globals['_AWSSDKTAGS']._serialized_end=3981
-  _globals['_AWSSDKDYNAMODBTAGS']._serialized_start=3984
-  _globals['_AWSSDKDYNAMODBTAGS']._serialized_end=4851
-  _globals['_AWSSDKSQSTAGS']._serialized_start=4853
-  _globals['_AWSSDKSQSTAGS']._serialized_end=4952
-  _globals['_AWSSDKSNSTAGS']._serialized_start=4954
-  _globals['_AWSSDKSNSTAGS']._serialized_end=5053
+  _globals['_AWSLAMBDATAGS']._serialized_end=3069
+  _globals['_AWSLAMBDATAGS_OUTCOME']._serialized_start=2543
+  _globals['_AWSLAMBDATAGS_OUTCOME']._serialized_end=2715
+  _globals['_HTTPROUTERTAGS']._serialized_start=3071
+  _globals['_HTTPROUTERTAGS']._serialized_end=3107
+  _globals['_AWSSQSEVENTTAGS']._serialized_start=3109
+  _globals['_AWSSQSEVENTTAGS']._serialized_end=3190
+  _globals['_AWSSNSEVENTTAGS']._serialized_start=3192
+  _globals['_AWSSNSEVENTTAGS']._serialized_end=3273
+  _globals['_AWSLAMBDARUNTIMETAGS']._serialized_start=3275
+  _globals['_AWSLAMBDARUNTIMETAGS']._serialized_end=3373
+  _globals['_AWSLAMBDAINITIALIZATIONTAGS']._serialized_start=3375
+  _globals['_AWSLAMBDAINITIALIZATIONTAGS']._serialized_end=3461
+  _globals['_AWSLAMBDAINVOCATIONTAGS']._serialized_start=3463
+  _globals['_AWSLAMBDAINVOCATIONTAGS']._serialized_end=3537
+  _globals['_AWSSDKTAGS']._serialized_start=3540
+  _globals['_AWSSDKTAGS']._serialized_end=4133
+  _globals['_AWSSDKDYNAMODBTAGS']._serialized_start=4136
+  _globals['_AWSSDKDYNAMODBTAGS']._serialized_end=5003
+  _globals['_AWSSDKSQSTAGS']._serialized_start=5005
+  _globals['_AWSSDKSQSTAGS']._serialized_end=5104
+  _globals['_AWSSDKSNSTAGS']._serialized_start=5106
+  _globals['_AWSSDKSNSTAGS']._serialized_end=5205
 # @@protoc_insertion_point(module_scope)
```

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/error_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/error_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/notice_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/notice_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/tags_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/tags_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/warning_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/tags/v1/warning_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/dev_mode_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/dev_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/event_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/log_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/log_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/metric_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/request_response_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/request_response_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema/schema/serverless/instrumentation/v1/trace_pb2.py` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema/schema/serverless/instrumentation/v1/trace_pb2.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema.egg-info/PKG-INFO` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk-schema
-Version: 0.2.0
+Version: 0.2.1
 Summary: The protobuf generated Serverless SDK Schema
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk-schema/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk-schema
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-schema-0.2.0/serverless_sdk_schema.egg-info/SOURCES.txt` & `serverless-sdk-schema-0.2.1/serverless_sdk_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-schema-0.2.0/tests/test_schema.py` & `serverless-sdk-schema-0.2.1/tests/test_schema.py`

 * *Files identical despite different names*

