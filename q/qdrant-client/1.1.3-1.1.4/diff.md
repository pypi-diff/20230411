# Comparing `tmp/qdrant_client-1.1.3.tar.gz` & `tmp/qdrant_client-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdrant_client-1.1.3.tar", max compression
+gzip compressed data, was "qdrant_client-1.1.4.tar", max compression
```

## Comparing `qdrant_client-1.1.3.tar` & `qdrant_client-1.1.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    11357 2023-04-08 14:52:52.635923 qdrant_client-1.1.3/LICENSE
--rw-r--r--   0        0        0     5639 2023-04-08 14:52:52.635923 qdrant_client-1.1.3/README.md
--rw-r--r--   0        0        0     1277 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/pyproject.toml
--rw-r--r--   0        0        0       56 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/__init__.py
--rw-r--r--   0        0        0    25845 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/client_base.py
--rw-r--r--   0        0        0     1104 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/connection.py
--rw-r--r--   0        0        0        0 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/conversions/__init__.py
--rw-r--r--   0        0        0     3231 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/conversions/common_types.py
--rw-r--r--   0        0        0    61186 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/conversions/conversion.py
--rw-r--r--   0        0        0      252 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/__init__.py
--rw-r--r--   0        0        0    28376 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/collections_pb2.py
--rw-r--r--   0        0        0      159 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/collections_pb2_grpc.py
--rw-r--r--   0        0        0     1794 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/collections_service_pb2.py
--rw-r--r--   0        0        0    13456 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/collections_service_pb2_grpc.py
--rw-r--r--   0        0        0     3395 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/json_with_int_pb2.py
--rw-r--r--   0        0        0      159 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/json_with_int_pb2_grpc.py
--rw-r--r--   0        0        0    43930 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/points_pb2.py
--rw-r--r--   0        0        0      159 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/points_pb2_grpc.py
--rw-r--r--   0        0        0     2502 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/points_service_pb2.py
--rw-r--r--   0        0        0    23690 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/points_service_pb2_grpc.py
--rw-r--r--   0        0        0     2254 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/qdrant_pb2.py
--rw-r--r--   0        0        0     2411 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/qdrant_pb2_grpc.py
--rw-r--r--   0        0        0     7768 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/snapshots_service_pb2.py
--rw-r--r--   0        0        0    10406 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/grpc/snapshots_service_pb2_grpc.py
--rw-r--r--   0        0        0      505 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/api/__init__.py
--rw-r--r--   0        0        0    10437 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/api/cluster_api.py
--rw-r--r--   0        0        0    27408 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/api/collections_api.py
--rw-r--r--   0        0        0    30820 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/api/points_api.py
--rw-r--r--   0        0        0     9499 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/api/service_api.py
--rw-r--r--   0        0        0    15295 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/api/snapshots_api.py
--rw-r--r--   0        0        0     7577 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/api_client.py
--rw-r--r--   0        0        0      233 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/configuration.py
--rw-r--r--   0        0        0     1616 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/exceptions.py
--rw-r--r--   0        0        0       22 2023-04-08 14:52:52.639923 qdrant_client-1.1.3/qdrant_client/http/models/__init__.py
--rw-r--r--   0        0        0    58719 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/http/models/models.py
--rw-r--r--   0        0        0        0 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/local/__init__.py
--rw-r--r--   0        0        0     2962 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/local/distances.py
--rw-r--r--   0        0        0     1446 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/local/geo.py
--rw-r--r--   0        0        0    21837 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/local/local_collection.py
--rw-r--r--   0        0        0     5595 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/local/payload_filters.py
--rw-r--r--   0        0        0     2713 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/local/payload_value_extractor.py
--rw-r--r--   0        0        0     2237 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/local/persistence.py
--rw-r--r--   0        0        0    18877 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/local/qdrant_local.py
--rw-r--r--   0        0        0       40 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/models/__init__.py
--rw-r--r--   0        0        0     7034 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/parallel_processor.py
--rw-r--r--   0        0        0    10624 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/proto/collections.proto
--rw-r--r--   0        0        0     1168 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/proto/collections_service.proto
--rw-r--r--   0        0        0     1929 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/proto/json_with_int.proto
--rw-r--r--   0        0        0    14485 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/proto/points.proto
--rw-r--r--   0        0        0     2191 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/proto/points_service.proto
--rw-r--r--   0        0        0      331 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/proto/qdrant.proto
--rw-r--r--   0        0        0     1895 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/proto/snapshots_service.proto
--rw-r--r--   0        0        0        8 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/py.typed
--rw-r--r--   0        0        0    54281 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/qdrant_client.py
--rw-r--r--   0        0        0    88692 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/qdrant_remote.py
--rw-r--r--   0        0        0        0 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/uploader/__init__.py
--rw-r--r--   0        0        0     2865 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/uploader/grpc_uploader.py
--rw-r--r--   0        0        0     2537 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/uploader/rest_uploader.py
--rw-r--r--   0        0        0     3200 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_client/uploader/uploader.py
--rw-r--r--   0        0        0      267 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_openapi_client/__init__.py
--rw-r--r--   0        0        0       37 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_openapi_client/api/__init__.py
--rw-r--r--   0        0        0       53 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_openapi_client/api/collections_api.py
--rw-r--r--   0        0        0       48 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_openapi_client/api/points_api.py
--rw-r--r--   0        0        0       44 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_openapi_client/exceptions.py
--rw-r--r--   0        0        0       47 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_openapi_client/models/__init__.py
--rw-r--r--   0        0        0       47 2023-04-08 14:52:52.643923 qdrant_client-1.1.3/qdrant_openapi_client/models/models.py
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 qdrant_client-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/LICENSE
+-rw-r--r--   0        0        0     5639 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/README.md
+-rw-r--r--   0        0        0     1277 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/qdrant_client/__init__.py
+-rw-r--r--   0        0        0    25845 2023-04-11 18:35:02.040182 qdrant_client-1.1.4/qdrant_client/client_base.py
+-rw-r--r--   0        0        0     1104 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/connection.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/conversions/__init__.py
+-rw-r--r--   0        0        0     3231 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/conversions/common_types.py
+-rw-r--r--   0        0        0    62445 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/conversions/conversion.py
+-rw-r--r--   0        0        0      252 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/__init__.py
+-rw-r--r--   0        0        0    28633 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/collections_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/collections_pb2_grpc.py
+-rw-r--r--   0        0        0     1794 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/collections_service_pb2.py
+-rw-r--r--   0        0        0    13456 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/collections_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3395 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/json_with_int_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/json_with_int_pb2_grpc.py
+-rw-r--r--   0        0        0    44493 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/points_pb2.py
+-rw-r--r--   0        0        0      159 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/points_pb2_grpc.py
+-rw-r--r--   0        0        0     2502 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/points_service_pb2.py
+-rw-r--r--   0        0        0    23694 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/points_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2254 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/qdrant_pb2.py
+-rw-r--r--   0        0        0     2411 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/qdrant_pb2_grpc.py
+-rw-r--r--   0        0        0     7768 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/snapshots_service_pb2.py
+-rw-r--r--   0        0        0    10406 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/grpc/snapshots_service_pb2_grpc.py
+-rw-r--r--   0        0        0      505 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/__init__.py
+-rw-r--r--   0        0        0    10437 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/cluster_api.py
+-rw-r--r--   0        0        0    30407 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/collections_api.py
+-rw-r--r--   0        0        0    30820 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/points_api.py
+-rw-r--r--   0        0        0     9499 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/service_api.py
+-rw-r--r--   0        0        0    18850 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api/snapshots_api.py
+-rw-r--r--   0        0        0     7577 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/api_client.py
+-rw-r--r--   0        0        0      233 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/configuration.py
+-rw-r--r--   0        0        0     1616 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/exceptions.py
+-rw-r--r--   0        0        0       22 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/models/__init__.py
+-rw-r--r--   0        0        0    60032 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/http/models/models.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/__init__.py
+-rw-r--r--   0        0        0     2962 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/distances.py
+-rw-r--r--   0        0        0     1446 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/geo.py
+-rw-r--r--   0        0        0    21902 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/local_collection.py
+-rw-r--r--   0        0        0     5866 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/payload_filters.py
+-rw-r--r--   0        0        0     2922 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/payload_value_extractor.py
+-rw-r--r--   0        0        0     2237 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/persistence.py
+-rw-r--r--   0        0        0    18939 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/local/qdrant_local.py
+-rw-r--r--   0        0        0       40 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/models/__init__.py
+-rw-r--r--   0        0        0     7034 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/parallel_processor.py
+-rw-r--r--   0        0        0    10979 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/collections.proto
+-rw-r--r--   0        0        0     1168 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/collections_service.proto
+-rw-r--r--   0        0        0     1936 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/json_with_int.proto
+-rw-r--r--   0        0        0    14566 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/points.proto
+-rw-r--r--   0        0        0     2196 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/points_service.proto
+-rw-r--r--   0        0        0      331 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/qdrant.proto
+-rw-r--r--   0        0        0     1895 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/proto/snapshots_service.proto
+-rw-r--r--   0        0        0        8 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/py.typed
+-rw-r--r--   0        0        0    54281 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/qdrant_client.py
+-rw-r--r--   0        0        0    88692 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/qdrant_remote.py
+-rw-r--r--   0        0        0        0 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/uploader/__init__.py
+-rw-r--r--   0        0        0     2865 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/uploader/grpc_uploader.py
+-rw-r--r--   0        0        0     2537 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/uploader/rest_uploader.py
+-rw-r--r--   0        0        0     3200 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_client/uploader/uploader.py
+-rw-r--r--   0        0        0      267 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/api/__init__.py
+-rw-r--r--   0        0        0       53 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/api/collections_api.py
+-rw-r--r--   0        0        0       48 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/api/points_api.py
+-rw-r--r--   0        0        0       44 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/exceptions.py
+-rw-r--r--   0        0        0       47 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/models/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-11 18:35:02.044182 qdrant_client-1.1.4/qdrant_openapi_client/models/models.py
+-rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 qdrant_client-1.1.4/PKG-INFO
```

### Comparing `qdrant_client-1.1.3/LICENSE` & `qdrant_client-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/README.md` & `qdrant_client-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/pyproject.toml` & `qdrant_client-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qdrant-client"
-version = "1.1.3"
+version = "1.1.4"
 description = "Client library for the Qdrant vector search engine"
 authors = ["Andrey Vasnetsov <andrey@qdrant.tech>"]
 packages = [
     {include = "qdrant_client"},
     {include = "qdrant_openapi_client"}
 ]
 readme = "README.md"
```

### Comparing `qdrant_client-1.1.3/qdrant_client/client_base.py` & `qdrant_client-1.1.4/qdrant_client/client_base.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/connection.py` & `qdrant_client-1.1.4/qdrant_client/connection.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/conversions/common_types.py` & `qdrant_client-1.1.4/qdrant_client/conversions/common_types.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/conversions/conversion.py` & `qdrant_client-1.1.4/qdrant_client/conversions/conversion.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
             return cls.convert_field_condition(val)
         if name == "filter":
             return cls.convert_filter(val)
         if name == "has_id":
             return cls.convert_has_id_condition(val)
         if name == "is_empty":
             return cls.convert_is_empty_condition(val)
+        if name == "is_null":
+            return cls.convert_is_null_condition(val)
 
         raise ValueError(f"invalid Condition model: {model}")  # pragma: no cover
 
     @classmethod
     def convert_filter(cls, model: grpc.Filter) -> rest.Filter:
         return rest.Filter(
             must=[cls.convert_condition(condition) for condition in model.must],
@@ -308,14 +310,18 @@
         )
 
     @classmethod
     def convert_is_empty_condition(cls, model: grpc.IsEmptyCondition) -> rest.IsEmptyCondition:
         return rest.IsEmptyCondition(is_empty=rest.PayloadField(key=model.key))
 
     @classmethod
+    def convert_is_null_condition(cls, model: grpc.IsNullCondition) -> rest.IsNullCondition:
+        return rest.IsNullCondition(is_null=rest.PayloadField(key=model.key))
+
+    @classmethod
     def convert_search_params(cls, model: grpc.SearchParams) -> rest.SearchParams:
         return rest.SearchParams(
             hnsw_ef=model.hnsw_ef if model.HasField("hnsw_ef") else None,
             exact=model.exact if model.HasField("exact") else None,
             quantization=cls.convert_quantization_search_params(model.quantization)
             if model.HasField("quantization")
             else None,
@@ -568,15 +574,24 @@
             if model.HasField("creation_time")
             else None,
             size=model.size,
         )
 
     @classmethod
     def convert_vector_params(cls, model: grpc.VectorParams) -> rest.VectorParams:
-        return rest.VectorParams(size=model.size, distance=cls.convert_distance(model.distance))
+        return rest.VectorParams(
+            size=model.size,
+            distance=cls.convert_distance(model.distance),
+            hnsw_config=cls.convert_hnsw_config_diff(model.hnsw_config)
+            if model.HasField("hnsw_config")
+            else None,
+            quantization_config=cls.convert_quantization_config(model.quantization_config)
+            if model.HasField("quantization_config")
+            else None,
+        )
 
     @classmethod
     def convert_vectors_config(cls, model: grpc.VectorsConfig) -> rest.VectorsConfig:
         name = model.WhichOneof("config")
         val = getattr(model, name)
 
         if name == "params":
@@ -891,14 +906,18 @@
         )
 
     @classmethod
     def convert_is_empty_condition(cls, model: rest.IsEmptyCondition) -> grpc.IsEmptyCondition:
         return grpc.IsEmptyCondition(key=model.is_empty.key)
 
     @classmethod
+    def convert_is_null_condition(cls, model: rest.IsNullCondition) -> grpc.IsNullCondition:
+        return grpc.IsNullCondition(key=model.is_null.key)
+
+    @classmethod
     def convert_search_params(cls, model: rest.SearchParams) -> grpc.SearchParams:
         return grpc.SearchParams(
             hnsw_ef=model.hnsw_ef,
             exact=model.exact,
             quantization=cls.convert_quantization_search_params(model.quantization)
             if model.quantization is not None
             else None,
@@ -1158,14 +1177,16 @@
 
     @classmethod
     def convert_condition(cls, model: rest.Condition) -> grpc.Condition:
         if isinstance(model, rest.FieldCondition):
             return grpc.Condition(field=cls.convert_field_condition(model))
         if isinstance(model, rest.IsEmptyCondition):
             return grpc.Condition(is_empty=cls.convert_is_empty_condition(model))
+        if isinstance(model, rest.IsNullCondition):
+            return grpc.Condition(is_null=cls.convert_is_null_condition(model))
         if isinstance(model, rest.HasIdCondition):
             return grpc.Condition(has_id=cls.convert_has_id_condition(model))
         if isinstance(model, rest.Filter):
             return grpc.Condition(filter=cls.convert_filter(model))
 
         raise ValueError(f"invalid Condition model: {model}")  # pragma: no cover
 
@@ -1232,15 +1253,24 @@
             name=model.name,
             creation_time=timestamp,
             size=model.size,
         )
 
     @classmethod
     def convert_vector_params(cls, model: rest.VectorParams) -> grpc.VectorParams:
-        return grpc.VectorParams(size=model.size, distance=cls.convert_distance(model.distance))
+        return grpc.VectorParams(
+            size=model.size,
+            distance=cls.convert_distance(model.distance),
+            hnsw_config=cls.convert_hnsw_config_diff(model.hnsw_config)
+            if model.hnsw_config is not None
+            else None,
+            quantization_config=cls.convert_quantization_config(model.quantization_config)
+            if model.quantization_config is not None
+            else None,
+        )
 
     @classmethod
     def convert_vectors_config(cls, model: rest.VectorsConfig) -> grpc.VectorsConfig:
         if isinstance(model, rest.VectorParams):
             return grpc.VectorsConfig(params=cls.convert_vector_params(model))
         elif isinstance(model, dict):
             return grpc.VectorsConfig(
```

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/collections_pb2.py` & `qdrant_client-1.1.4/qdrant_client/grpc/collections_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63ollections.proto\x12\x06qdrant\"@\n\x0cVectorParams\x12\x0c\n\x04size\x18\x01 \x01(\x04\x12\"\n\x08\x64istance\x18\x02 \x01(\x0e\x32\x10.qdrant.Distance\"\x82\x01\n\x0fVectorParamsMap\x12-\n\x03map\x18\x01 \x03(\x0b\x32 .qdrant.VectorParamsMap.MapEntry\x1a@\n\x08MapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.qdrant.VectorParams:\x02\x38\x01\"p\n\rVectorsConfig\x12&\n\x06params\x18\x01 \x01(\x0b\x32\x14.qdrant.VectorParamsH\x00\x12-\n\nparams_map\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorParamsMapH\x00\x42\x08\n\x06\x63onfig\"3\n\x18GetCollectionInfoRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\x18\n\x16ListCollectionsRequest\"%\n\x15\x43ollectionDescription\x12\x0c\n\x04name\x18\x01 \x01(\t\"Q\n\x19GetCollectionInfoResponse\x12&\n\x06result\x18\x01 \x01(\x0b\x32\x16.qdrant.CollectionInfo\x12\x0c\n\x04time\x18\x02 \x01(\x01\"[\n\x17ListCollectionsResponse\x12\x32\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\x1d.qdrant.CollectionDescription\x12\x0c\n\x04time\x18\x02 \x01(\x01\",\n\x0fOptimizerStatus\x12\n\n\x02ok\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\x90\x02\n\x0eHnswConfigDiff\x12\x0e\n\x01m\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x19\n\x0c\x65\x66_construct\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12 \n\x13\x66ull_scan_threshold\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12!\n\x14max_indexing_threads\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x14\n\x07on_disk\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12\x16\n\tpayload_m\x18\x06 \x01(\x04H\x05\x88\x01\x01\x42\x04\n\x02_mB\x0f\n\r_ef_constructB\x16\n\x14_full_scan_thresholdB\x17\n\x15_max_indexing_threadsB\n\n\x08_on_diskB\x0c\n\n_payload_m\"y\n\rWalConfigDiff\x12\x1c\n\x0fwal_capacity_mb\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x1f\n\x12wal_segments_ahead\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x12\n\x10_wal_capacity_mbB\x15\n\x13_wal_segments_ahead\"\xec\x03\n\x14OptimizersConfigDiff\x12\x1e\n\x11\x64\x65leted_threshold\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12%\n\x18vacuum_min_vector_number\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12#\n\x16\x64\x65\x66\x61ult_segment_number\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x1d\n\x10max_segment_size\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x1d\n\x10memmap_threshold\x18\x05 \x01(\x04H\x04\x88\x01\x01\x12\x1f\n\x12indexing_threshold\x18\x06 \x01(\x04H\x05\x88\x01\x01\x12\x1f\n\x12\x66lush_interval_sec\x18\x07 \x01(\x04H\x06\x88\x01\x01\x12%\n\x18max_optimization_threads\x18\x08 \x01(\x04H\x07\x88\x01\x01\x42\x14\n\x12_deleted_thresholdB\x1b\n\x19_vacuum_min_vector_numberB\x19\n\x17_default_segment_numberB\x13\n\x11_max_segment_sizeB\x13\n\x11_memmap_thresholdB\x15\n\x13_indexing_thresholdB\x15\n\x13_flush_interval_secB\x1b\n\x19_max_optimization_threads\"\x88\x01\n\x12ScalarQuantization\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.qdrant.QuantizationType\x12\x15\n\x08quantile\x18\x02 \x01(\x02H\x00\x88\x01\x01\x12\x17\n\nalways_ram\x18\x03 \x01(\x08H\x01\x88\x01\x01\x42\x0b\n\t_quantileB\r\n\x0b_always_ram\"R\n\x12QuantizationConfig\x12,\n\x06scalar\x18\x01 \x01(\x0b\x32\x1a.qdrant.ScalarQuantizationH\x00\x42\x0e\n\x0cquantization\"\xe1\x05\n\x10\x43reateCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x0bhnsw_config\x18\x04 \x01(\x0b\x32\x16.qdrant.HnswConfigDiffH\x00\x88\x01\x01\x12.\n\nwal_config\x18\x05 \x01(\x0b\x32\x15.qdrant.WalConfigDiffH\x01\x88\x01\x01\x12<\n\x11optimizers_config\x18\x06 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiffH\x02\x88\x01\x01\x12\x19\n\x0cshard_number\x18\x07 \x01(\rH\x03\x88\x01\x01\x12\x1c\n\x0fon_disk_payload\x18\x08 \x01(\x08H\x04\x88\x01\x01\x12\x14\n\x07timeout\x18\t \x01(\x04H\x05\x88\x01\x01\x12\x32\n\x0evectors_config\x18\n \x01(\x0b\x32\x15.qdrant.VectorsConfigH\x06\x88\x01\x01\x12\x1f\n\x12replication_factor\x18\x0b \x01(\rH\x07\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x0c \x01(\rH\x08\x88\x01\x01\x12!\n\x14init_from_collection\x18\r \x01(\tH\t\x88\x01\x01\x12<\n\x13quantization_config\x18\x0e \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\n\x88\x01\x01\x42\x0e\n\x0c_hnsw_configB\r\n\x0b_wal_configB\x14\n\x12_optimizers_configB\x0f\n\r_shard_numberB\x12\n\x10_on_disk_payloadB\n\n\x08_timeoutB\x11\n\x0f_vectors_configB\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factorB\x17\n\x15_init_from_collectionB\x16\n\x14_quantization_configJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"\xdf\x01\n\x10UpdateCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12<\n\x11optimizers_config\x18\x02 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiffH\x00\x88\x01\x01\x12\x14\n\x07timeout\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x31\n\x06params\x18\x04 \x01(\x0b\x32\x1c.qdrant.CollectionParamsDiffH\x02\x88\x01\x01\x42\x14\n\x12_optimizers_configB\n\n\x08_timeoutB\t\n\x07_params\"M\n\x10\x44\x65leteCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\n\n\x08_timeout\";\n\x1b\x43ollectionOperationResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x90\x02\n\x10\x43ollectionParams\x12\x14\n\x0cshard_number\x18\x03 \x01(\r\x12\x17\n\x0fon_disk_payload\x18\x04 \x01(\x08\x12\x32\n\x0evectors_config\x18\x05 \x01(\x0b\x32\x15.qdrant.VectorsConfigH\x00\x88\x01\x01\x12\x1f\n\x12replication_factor\x18\x06 \x01(\rH\x01\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x07 \x01(\rH\x02\x88\x01\x01\x42\x11\n\x0f_vectors_configB\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factorJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x92\x01\n\x14\x43ollectionParamsDiff\x12\x1f\n\x12replication_factor\x18\x01 \x01(\rH\x00\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x02 \x01(\rH\x01\x88\x01\x01\x42\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factor\"\xa2\x02\n\x10\x43ollectionConfig\x12(\n\x06params\x18\x01 \x01(\x0b\x32\x18.qdrant.CollectionParams\x12+\n\x0bhnsw_config\x18\x02 \x01(\x0b\x32\x16.qdrant.HnswConfigDiff\x12\x36\n\x10optimizer_config\x18\x03 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiff\x12)\n\nwal_config\x18\x04 \x01(\x0b\x32\x15.qdrant.WalConfigDiff\x12<\n\x13quantization_config\x18\x05 \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\x00\x88\x01\x01\x42\x16\n\x14_quantization_config\"\xbd\x01\n\x0fTextIndexParams\x12(\n\ttokenizer\x18\x01 \x01(\x0e\x32\x15.qdrant.TokenizerType\x12\x16\n\tlowercase\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1a\n\rmin_token_len\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1a\n\rmax_token_len\x18\x04 \x01(\x04H\x02\x88\x01\x01\x42\x0c\n\n_lowercaseB\x10\n\x0e_min_token_lenB\x10\n\x0e_max_token_len\"Z\n\x12PayloadIndexParams\x12\x34\n\x11text_index_params\x18\x01 \x01(\x0b\x32\x17.qdrant.TextIndexParamsH\x00\x42\x0e\n\x0cindex_params\"\x9d\x01\n\x11PayloadSchemaInfo\x12,\n\tdata_type\x18\x01 \x01(\x0e\x32\x19.qdrant.PayloadSchemaType\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x00\x88\x01\x01\x12\x13\n\x06points\x18\x03 \x01(\x04H\x01\x88\x01\x01\x42\t\n\x07_paramsB\t\n\x07_points\"\xba\x03\n\x0e\x43ollectionInfo\x12(\n\x06status\x18\x01 \x01(\x0e\x32\x18.qdrant.CollectionStatus\x12\x31\n\x10optimizer_status\x18\x02 \x01(\x0b\x32\x17.qdrant.OptimizerStatus\x12\x15\n\rvectors_count\x18\x03 \x01(\x04\x12\x16\n\x0esegments_count\x18\x04 \x01(\x04\x12(\n\x06\x63onfig\x18\x07 \x01(\x0b\x32\x18.qdrant.CollectionConfig\x12\x41\n\x0epayload_schema\x18\x08 \x03(\x0b\x32).qdrant.CollectionInfo.PayloadSchemaEntry\x12\x14\n\x0cpoints_count\x18\t \x01(\x04\x12\"\n\x15indexed_vectors_count\x18\n \x01(\x04H\x00\x88\x01\x01\x1aO\n\x12PayloadSchemaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.qdrant.PayloadSchemaInfo:\x02\x38\x01\x42\x18\n\x16_indexed_vectors_countJ\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"[\n\rChangeAliases\x12(\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x17.qdrant.AliasOperations\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\n\n\x08_timeout\"\xa2\x01\n\x0f\x41liasOperations\x12+\n\x0c\x63reate_alias\x18\x01 \x01(\x0b\x32\x13.qdrant.CreateAliasH\x00\x12+\n\x0crename_alias\x18\x02 \x01(\x0b\x32\x13.qdrant.RenameAliasH\x00\x12+\n\x0c\x64\x65lete_alias\x18\x03 \x01(\x0b\x32\x13.qdrant.DeleteAliasH\x00\x42\x08\n\x06\x61\x63tion\":\n\x0b\x43reateAlias\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nalias_name\x18\x02 \x01(\t\"=\n\x0bRenameAlias\x12\x16\n\x0eold_alias_name\x18\x01 \x01(\t\x12\x16\n\x0enew_alias_name\x18\x02 \x01(\t\"!\n\x0b\x44\x65leteAlias\x12\x12\n\nalias_name\x18\x01 \x01(\t\"\x14\n\x12ListAliasesRequest\"7\n\x1cListCollectionAliasesRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"?\n\x10\x41liasDescription\x12\x12\n\nalias_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\"N\n\x13ListAliasesResponse\x12)\n\x07\x61liases\x18\x01 \x03(\x0b\x32\x18.qdrant.AliasDescription\x12\x0c\n\x04time\x18\x02 \x01(\x01*@\n\x08\x44istance\x12\x13\n\x0fUnknownDistance\x10\x00\x12\n\n\x06\x43osine\x10\x01\x12\n\n\x06\x45uclid\x10\x02\x12\x07\n\x03\x44ot\x10\x03*O\n\x10\x43ollectionStatus\x12\x1b\n\x17UnknownCollectionStatus\x10\x00\x12\t\n\x05Green\x10\x01\x12\n\n\x06Yellow\x10\x02\x12\x07\n\x03Red\x10\x03*\\\n\x11PayloadSchemaType\x12\x0f\n\x0bUnknownType\x10\x00\x12\x0b\n\x07Keyword\x10\x01\x12\x0b\n\x07Integer\x10\x02\x12\t\n\x05\x46loat\x10\x03\x12\x07\n\x03Geo\x10\x04\x12\x08\n\x04Text\x10\x05*5\n\x10QuantizationType\x12\x17\n\x13UnknownQuantization\x10\x00\x12\x08\n\x04Int8\x10\x01*B\n\rTokenizerType\x12\x0b\n\x07Unknown\x10\x00\x12\n\n\x06Prefix\x10\x01\x12\x0e\n\nWhitespace\x10\x02\x12\x08\n\x04Word\x10\x03\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63ollections.proto\x12\x06qdrant\"\xd8\x01\n\x0cVectorParams\x12\x0c\n\x04size\x18\x01 \x01(\x04\x12\"\n\x08\x64istance\x18\x02 \x01(\x0e\x32\x10.qdrant.Distance\x12\x30\n\x0bhnsw_config\x18\x03 \x01(\x0b\x32\x16.qdrant.HnswConfigDiffH\x00\x88\x01\x01\x12<\n\x13quantization_config\x18\x04 \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\x01\x88\x01\x01\x42\x0e\n\x0c_hnsw_configB\x16\n\x14_quantization_config\"\x82\x01\n\x0fVectorParamsMap\x12-\n\x03map\x18\x01 \x03(\x0b\x32 .qdrant.VectorParamsMap.MapEntry\x1a@\n\x08MapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.qdrant.VectorParams:\x02\x38\x01\"p\n\rVectorsConfig\x12&\n\x06params\x18\x01 \x01(\x0b\x32\x14.qdrant.VectorParamsH\x00\x12-\n\nparams_map\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorParamsMapH\x00\x42\x08\n\x06\x63onfig\"3\n\x18GetCollectionInfoRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\x18\n\x16ListCollectionsRequest\"%\n\x15\x43ollectionDescription\x12\x0c\n\x04name\x18\x01 \x01(\t\"Q\n\x19GetCollectionInfoResponse\x12&\n\x06result\x18\x01 \x01(\x0b\x32\x16.qdrant.CollectionInfo\x12\x0c\n\x04time\x18\x02 \x01(\x01\"[\n\x17ListCollectionsResponse\x12\x32\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\x1d.qdrant.CollectionDescription\x12\x0c\n\x04time\x18\x02 \x01(\x01\",\n\x0fOptimizerStatus\x12\n\n\x02ok\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\x90\x02\n\x0eHnswConfigDiff\x12\x0e\n\x01m\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x19\n\x0c\x65\x66_construct\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12 \n\x13\x66ull_scan_threshold\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12!\n\x14max_indexing_threads\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x14\n\x07on_disk\x18\x05 \x01(\x08H\x04\x88\x01\x01\x12\x16\n\tpayload_m\x18\x06 \x01(\x04H\x05\x88\x01\x01\x42\x04\n\x02_mB\x0f\n\r_ef_constructB\x16\n\x14_full_scan_thresholdB\x17\n\x15_max_indexing_threadsB\n\n\x08_on_diskB\x0c\n\n_payload_m\"y\n\rWalConfigDiff\x12\x1c\n\x0fwal_capacity_mb\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x1f\n\x12wal_segments_ahead\x18\x02 \x01(\x04H\x01\x88\x01\x01\x42\x12\n\x10_wal_capacity_mbB\x15\n\x13_wal_segments_ahead\"\xec\x03\n\x14OptimizersConfigDiff\x12\x1e\n\x11\x64\x65leted_threshold\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12%\n\x18vacuum_min_vector_number\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12#\n\x16\x64\x65\x66\x61ult_segment_number\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x1d\n\x10max_segment_size\x18\x04 \x01(\x04H\x03\x88\x01\x01\x12\x1d\n\x10memmap_threshold\x18\x05 \x01(\x04H\x04\x88\x01\x01\x12\x1f\n\x12indexing_threshold\x18\x06 \x01(\x04H\x05\x88\x01\x01\x12\x1f\n\x12\x66lush_interval_sec\x18\x07 \x01(\x04H\x06\x88\x01\x01\x12%\n\x18max_optimization_threads\x18\x08 \x01(\x04H\x07\x88\x01\x01\x42\x14\n\x12_deleted_thresholdB\x1b\n\x19_vacuum_min_vector_numberB\x19\n\x17_default_segment_numberB\x13\n\x11_max_segment_sizeB\x13\n\x11_memmap_thresholdB\x15\n\x13_indexing_thresholdB\x15\n\x13_flush_interval_secB\x1b\n\x19_max_optimization_threads\"\x88\x01\n\x12ScalarQuantization\x12&\n\x04type\x18\x01 \x01(\x0e\x32\x18.qdrant.QuantizationType\x12\x15\n\x08quantile\x18\x02 \x01(\x02H\x00\x88\x01\x01\x12\x17\n\nalways_ram\x18\x03 \x01(\x08H\x01\x88\x01\x01\x42\x0b\n\t_quantileB\r\n\x0b_always_ram\"R\n\x12QuantizationConfig\x12,\n\x06scalar\x18\x01 \x01(\x0b\x32\x1a.qdrant.ScalarQuantizationH\x00\x42\x0e\n\x0cquantization\"\xe1\x05\n\x10\x43reateCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x0bhnsw_config\x18\x04 \x01(\x0b\x32\x16.qdrant.HnswConfigDiffH\x00\x88\x01\x01\x12.\n\nwal_config\x18\x05 \x01(\x0b\x32\x15.qdrant.WalConfigDiffH\x01\x88\x01\x01\x12<\n\x11optimizers_config\x18\x06 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiffH\x02\x88\x01\x01\x12\x19\n\x0cshard_number\x18\x07 \x01(\rH\x03\x88\x01\x01\x12\x1c\n\x0fon_disk_payload\x18\x08 \x01(\x08H\x04\x88\x01\x01\x12\x14\n\x07timeout\x18\t \x01(\x04H\x05\x88\x01\x01\x12\x32\n\x0evectors_config\x18\n \x01(\x0b\x32\x15.qdrant.VectorsConfigH\x06\x88\x01\x01\x12\x1f\n\x12replication_factor\x18\x0b \x01(\rH\x07\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x0c \x01(\rH\x08\x88\x01\x01\x12!\n\x14init_from_collection\x18\r \x01(\tH\t\x88\x01\x01\x12<\n\x13quantization_config\x18\x0e \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\n\x88\x01\x01\x42\x0e\n\x0c_hnsw_configB\r\n\x0b_wal_configB\x14\n\x12_optimizers_configB\x0f\n\r_shard_numberB\x12\n\x10_on_disk_payloadB\n\n\x08_timeoutB\x11\n\x0f_vectors_configB\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factorB\x17\n\x15_init_from_collectionB\x16\n\x14_quantization_configJ\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04\"\xdf\x01\n\x10UpdateCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12<\n\x11optimizers_config\x18\x02 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiffH\x00\x88\x01\x01\x12\x14\n\x07timeout\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x31\n\x06params\x18\x04 \x01(\x0b\x32\x1c.qdrant.CollectionParamsDiffH\x02\x88\x01\x01\x42\x14\n\x12_optimizers_configB\n\n\x08_timeoutB\t\n\x07_params\"M\n\x10\x44\x65leteCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\n\n\x08_timeout\";\n\x1b\x43ollectionOperationResponse\x12\x0e\n\x06result\x18\x01 \x01(\x08\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x90\x02\n\x10\x43ollectionParams\x12\x14\n\x0cshard_number\x18\x03 \x01(\r\x12\x17\n\x0fon_disk_payload\x18\x04 \x01(\x08\x12\x32\n\x0evectors_config\x18\x05 \x01(\x0b\x32\x15.qdrant.VectorsConfigH\x00\x88\x01\x01\x12\x1f\n\x12replication_factor\x18\x06 \x01(\rH\x01\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x07 \x01(\rH\x02\x88\x01\x01\x42\x11\n\x0f_vectors_configB\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factorJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x92\x01\n\x14\x43ollectionParamsDiff\x12\x1f\n\x12replication_factor\x18\x01 \x01(\rH\x00\x88\x01\x01\x12%\n\x18write_consistency_factor\x18\x02 \x01(\rH\x01\x88\x01\x01\x42\x15\n\x13_replication_factorB\x1b\n\x19_write_consistency_factor\"\xa2\x02\n\x10\x43ollectionConfig\x12(\n\x06params\x18\x01 \x01(\x0b\x32\x18.qdrant.CollectionParams\x12+\n\x0bhnsw_config\x18\x02 \x01(\x0b\x32\x16.qdrant.HnswConfigDiff\x12\x36\n\x10optimizer_config\x18\x03 \x01(\x0b\x32\x1c.qdrant.OptimizersConfigDiff\x12)\n\nwal_config\x18\x04 \x01(\x0b\x32\x15.qdrant.WalConfigDiff\x12<\n\x13quantization_config\x18\x05 \x01(\x0b\x32\x1a.qdrant.QuantizationConfigH\x00\x88\x01\x01\x42\x16\n\x14_quantization_config\"\xbd\x01\n\x0fTextIndexParams\x12(\n\ttokenizer\x18\x01 \x01(\x0e\x32\x15.qdrant.TokenizerType\x12\x16\n\tlowercase\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x1a\n\rmin_token_len\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1a\n\rmax_token_len\x18\x04 \x01(\x04H\x02\x88\x01\x01\x42\x0c\n\n_lowercaseB\x10\n\x0e_min_token_lenB\x10\n\x0e_max_token_len\"Z\n\x12PayloadIndexParams\x12\x34\n\x11text_index_params\x18\x01 \x01(\x0b\x32\x17.qdrant.TextIndexParamsH\x00\x42\x0e\n\x0cindex_params\"\x9d\x01\n\x11PayloadSchemaInfo\x12,\n\tdata_type\x18\x01 \x01(\x0e\x32\x19.qdrant.PayloadSchemaType\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x00\x88\x01\x01\x12\x13\n\x06points\x18\x03 \x01(\x04H\x01\x88\x01\x01\x42\t\n\x07_paramsB\t\n\x07_points\"\xba\x03\n\x0e\x43ollectionInfo\x12(\n\x06status\x18\x01 \x01(\x0e\x32\x18.qdrant.CollectionStatus\x12\x31\n\x10optimizer_status\x18\x02 \x01(\x0b\x32\x17.qdrant.OptimizerStatus\x12\x15\n\rvectors_count\x18\x03 \x01(\x04\x12\x16\n\x0esegments_count\x18\x04 \x01(\x04\x12(\n\x06\x63onfig\x18\x07 \x01(\x0b\x32\x18.qdrant.CollectionConfig\x12\x41\n\x0epayload_schema\x18\x08 \x03(\x0b\x32).qdrant.CollectionInfo.PayloadSchemaEntry\x12\x14\n\x0cpoints_count\x18\t \x01(\x04\x12\"\n\x15indexed_vectors_count\x18\n \x01(\x04H\x00\x88\x01\x01\x1aO\n\x12PayloadSchemaEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.qdrant.PayloadSchemaInfo:\x02\x38\x01\x42\x18\n\x16_indexed_vectors_countJ\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07\"[\n\rChangeAliases\x12(\n\x07\x61\x63tions\x18\x01 \x03(\x0b\x32\x17.qdrant.AliasOperations\x12\x14\n\x07timeout\x18\x02 \x01(\x04H\x00\x88\x01\x01\x42\n\n\x08_timeout\"\xa2\x01\n\x0f\x41liasOperations\x12+\n\x0c\x63reate_alias\x18\x01 \x01(\x0b\x32\x13.qdrant.CreateAliasH\x00\x12+\n\x0crename_alias\x18\x02 \x01(\x0b\x32\x13.qdrant.RenameAliasH\x00\x12+\n\x0c\x64\x65lete_alias\x18\x03 \x01(\x0b\x32\x13.qdrant.DeleteAliasH\x00\x42\x08\n\x06\x61\x63tion\":\n\x0b\x43reateAlias\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nalias_name\x18\x02 \x01(\t\"=\n\x0bRenameAlias\x12\x16\n\x0eold_alias_name\x18\x01 \x01(\t\x12\x16\n\x0enew_alias_name\x18\x02 \x01(\t\"!\n\x0b\x44\x65leteAlias\x12\x12\n\nalias_name\x18\x01 \x01(\t\"\x14\n\x12ListAliasesRequest\"7\n\x1cListCollectionAliasesRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"?\n\x10\x41liasDescription\x12\x12\n\nalias_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x02 \x01(\t\"N\n\x13ListAliasesResponse\x12)\n\x07\x61liases\x18\x01 \x03(\x0b\x32\x18.qdrant.AliasDescription\x12\x0c\n\x04time\x18\x02 \x01(\x01*@\n\x08\x44istance\x12\x13\n\x0fUnknownDistance\x10\x00\x12\n\n\x06\x43osine\x10\x01\x12\n\n\x06\x45uclid\x10\x02\x12\x07\n\x03\x44ot\x10\x03*O\n\x10\x43ollectionStatus\x12\x1b\n\x17UnknownCollectionStatus\x10\x00\x12\t\n\x05Green\x10\x01\x12\n\n\x06Yellow\x10\x02\x12\x07\n\x03Red\x10\x03*\\\n\x11PayloadSchemaType\x12\x0f\n\x0bUnknownType\x10\x00\x12\x0b\n\x07Keyword\x10\x01\x12\x0b\n\x07Integer\x10\x02\x12\t\n\x05\x46loat\x10\x03\x12\x07\n\x03Geo\x10\x04\x12\x08\n\x04Text\x10\x05*5\n\x10QuantizationType\x12\x17\n\x13UnknownQuantization\x10\x00\x12\x08\n\x04Int8\x10\x01*B\n\rTokenizerType\x12\x0b\n\x07Unknown\x10\x00\x12\n\n\x06Prefix\x10\x01\x12\x0e\n\nWhitespace\x10\x02\x12\x08\n\x04Word\x10\x03\x62\x06proto3')
 
 _DISTANCE = DESCRIPTOR.enum_types_by_name['Distance']
 Distance = enum_type_wrapper.EnumTypeWrapper(_DISTANCE)
 _COLLECTIONSTATUS = DESCRIPTOR.enum_types_by_name['CollectionStatus']
 CollectionStatus = enum_type_wrapper.EnumTypeWrapper(_COLLECTIONSTATUS)
 _PAYLOADSCHEMATYPE = DESCRIPTOR.enum_types_by_name['PayloadSchemaType']
 PayloadSchemaType = enum_type_wrapper.EnumTypeWrapper(_PAYLOADSCHEMATYPE)
@@ -342,90 +342,90 @@
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _VECTORPARAMSMAP_MAPENTRY._options = None
   _VECTORPARAMSMAP_MAPENTRY._serialized_options = b'8\001'
   _COLLECTIONINFO_PAYLOADSCHEMAENTRY._options = None
   _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_options = b'8\001'
-  _DISTANCE._serialized_start=5150
-  _DISTANCE._serialized_end=5214
-  _COLLECTIONSTATUS._serialized_start=5216
-  _COLLECTIONSTATUS._serialized_end=5295
-  _PAYLOADSCHEMATYPE._serialized_start=5297
-  _PAYLOADSCHEMATYPE._serialized_end=5389
-  _QUANTIZATIONTYPE._serialized_start=5391
-  _QUANTIZATIONTYPE._serialized_end=5444
-  _TOKENIZERTYPE._serialized_start=5446
-  _TOKENIZERTYPE._serialized_end=5512
-  _VECTORPARAMS._serialized_start=29
-  _VECTORPARAMS._serialized_end=93
-  _VECTORPARAMSMAP._serialized_start=96
-  _VECTORPARAMSMAP._serialized_end=226
-  _VECTORPARAMSMAP_MAPENTRY._serialized_start=162
-  _VECTORPARAMSMAP_MAPENTRY._serialized_end=226
-  _VECTORSCONFIG._serialized_start=228
-  _VECTORSCONFIG._serialized_end=340
-  _GETCOLLECTIONINFOREQUEST._serialized_start=342
-  _GETCOLLECTIONINFOREQUEST._serialized_end=393
-  _LISTCOLLECTIONSREQUEST._serialized_start=395
-  _LISTCOLLECTIONSREQUEST._serialized_end=419
-  _COLLECTIONDESCRIPTION._serialized_start=421
-  _COLLECTIONDESCRIPTION._serialized_end=458
-  _GETCOLLECTIONINFORESPONSE._serialized_start=460
-  _GETCOLLECTIONINFORESPONSE._serialized_end=541
-  _LISTCOLLECTIONSRESPONSE._serialized_start=543
-  _LISTCOLLECTIONSRESPONSE._serialized_end=634
-  _OPTIMIZERSTATUS._serialized_start=636
-  _OPTIMIZERSTATUS._serialized_end=680
-  _HNSWCONFIGDIFF._serialized_start=683
-  _HNSWCONFIGDIFF._serialized_end=955
-  _WALCONFIGDIFF._serialized_start=957
-  _WALCONFIGDIFF._serialized_end=1078
-  _OPTIMIZERSCONFIGDIFF._serialized_start=1081
-  _OPTIMIZERSCONFIGDIFF._serialized_end=1573
-  _SCALARQUANTIZATION._serialized_start=1576
-  _SCALARQUANTIZATION._serialized_end=1712
-  _QUANTIZATIONCONFIG._serialized_start=1714
-  _QUANTIZATIONCONFIG._serialized_end=1796
-  _CREATECOLLECTION._serialized_start=1799
-  _CREATECOLLECTION._serialized_end=2536
-  _UPDATECOLLECTION._serialized_start=2539
-  _UPDATECOLLECTION._serialized_end=2762
-  _DELETECOLLECTION._serialized_start=2764
-  _DELETECOLLECTION._serialized_end=2841
-  _COLLECTIONOPERATIONRESPONSE._serialized_start=2843
-  _COLLECTIONOPERATIONRESPONSE._serialized_end=2902
-  _COLLECTIONPARAMS._serialized_start=2905
-  _COLLECTIONPARAMS._serialized_end=3177
-  _COLLECTIONPARAMSDIFF._serialized_start=3180
-  _COLLECTIONPARAMSDIFF._serialized_end=3326
-  _COLLECTIONCONFIG._serialized_start=3329
-  _COLLECTIONCONFIG._serialized_end=3619
-  _TEXTINDEXPARAMS._serialized_start=3622
-  _TEXTINDEXPARAMS._serialized_end=3811
-  _PAYLOADINDEXPARAMS._serialized_start=3813
-  _PAYLOADINDEXPARAMS._serialized_end=3903
-  _PAYLOADSCHEMAINFO._serialized_start=3906
-  _PAYLOADSCHEMAINFO._serialized_end=4063
-  _COLLECTIONINFO._serialized_start=4066
-  _COLLECTIONINFO._serialized_end=4508
-  _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_start=4391
-  _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_end=4470
-  _CHANGEALIASES._serialized_start=4510
-  _CHANGEALIASES._serialized_end=4601
-  _ALIASOPERATIONS._serialized_start=4604
-  _ALIASOPERATIONS._serialized_end=4766
-  _CREATEALIAS._serialized_start=4768
-  _CREATEALIAS._serialized_end=4826
-  _RENAMEALIAS._serialized_start=4828
-  _RENAMEALIAS._serialized_end=4889
-  _DELETEALIAS._serialized_start=4891
-  _DELETEALIAS._serialized_end=4924
-  _LISTALIASESREQUEST._serialized_start=4926
-  _LISTALIASESREQUEST._serialized_end=4946
-  _LISTCOLLECTIONALIASESREQUEST._serialized_start=4948
-  _LISTCOLLECTIONALIASESREQUEST._serialized_end=5003
-  _ALIASDESCRIPTION._serialized_start=5005
-  _ALIASDESCRIPTION._serialized_end=5068
-  _LISTALIASESRESPONSE._serialized_start=5070
-  _LISTALIASESRESPONSE._serialized_end=5148
+  _DISTANCE._serialized_start=5303
+  _DISTANCE._serialized_end=5367
+  _COLLECTIONSTATUS._serialized_start=5369
+  _COLLECTIONSTATUS._serialized_end=5448
+  _PAYLOADSCHEMATYPE._serialized_start=5450
+  _PAYLOADSCHEMATYPE._serialized_end=5542
+  _QUANTIZATIONTYPE._serialized_start=5544
+  _QUANTIZATIONTYPE._serialized_end=5597
+  _TOKENIZERTYPE._serialized_start=5599
+  _TOKENIZERTYPE._serialized_end=5665
+  _VECTORPARAMS._serialized_start=30
+  _VECTORPARAMS._serialized_end=246
+  _VECTORPARAMSMAP._serialized_start=249
+  _VECTORPARAMSMAP._serialized_end=379
+  _VECTORPARAMSMAP_MAPENTRY._serialized_start=315
+  _VECTORPARAMSMAP_MAPENTRY._serialized_end=379
+  _VECTORSCONFIG._serialized_start=381
+  _VECTORSCONFIG._serialized_end=493
+  _GETCOLLECTIONINFOREQUEST._serialized_start=495
+  _GETCOLLECTIONINFOREQUEST._serialized_end=546
+  _LISTCOLLECTIONSREQUEST._serialized_start=548
+  _LISTCOLLECTIONSREQUEST._serialized_end=572
+  _COLLECTIONDESCRIPTION._serialized_start=574
+  _COLLECTIONDESCRIPTION._serialized_end=611
+  _GETCOLLECTIONINFORESPONSE._serialized_start=613
+  _GETCOLLECTIONINFORESPONSE._serialized_end=694
+  _LISTCOLLECTIONSRESPONSE._serialized_start=696
+  _LISTCOLLECTIONSRESPONSE._serialized_end=787
+  _OPTIMIZERSTATUS._serialized_start=789
+  _OPTIMIZERSTATUS._serialized_end=833
+  _HNSWCONFIGDIFF._serialized_start=836
+  _HNSWCONFIGDIFF._serialized_end=1108
+  _WALCONFIGDIFF._serialized_start=1110
+  _WALCONFIGDIFF._serialized_end=1231
+  _OPTIMIZERSCONFIGDIFF._serialized_start=1234
+  _OPTIMIZERSCONFIGDIFF._serialized_end=1726
+  _SCALARQUANTIZATION._serialized_start=1729
+  _SCALARQUANTIZATION._serialized_end=1865
+  _QUANTIZATIONCONFIG._serialized_start=1867
+  _QUANTIZATIONCONFIG._serialized_end=1949
+  _CREATECOLLECTION._serialized_start=1952
+  _CREATECOLLECTION._serialized_end=2689
+  _UPDATECOLLECTION._serialized_start=2692
+  _UPDATECOLLECTION._serialized_end=2915
+  _DELETECOLLECTION._serialized_start=2917
+  _DELETECOLLECTION._serialized_end=2994
+  _COLLECTIONOPERATIONRESPONSE._serialized_start=2996
+  _COLLECTIONOPERATIONRESPONSE._serialized_end=3055
+  _COLLECTIONPARAMS._serialized_start=3058
+  _COLLECTIONPARAMS._serialized_end=3330
+  _COLLECTIONPARAMSDIFF._serialized_start=3333
+  _COLLECTIONPARAMSDIFF._serialized_end=3479
+  _COLLECTIONCONFIG._serialized_start=3482
+  _COLLECTIONCONFIG._serialized_end=3772
+  _TEXTINDEXPARAMS._serialized_start=3775
+  _TEXTINDEXPARAMS._serialized_end=3964
+  _PAYLOADINDEXPARAMS._serialized_start=3966
+  _PAYLOADINDEXPARAMS._serialized_end=4056
+  _PAYLOADSCHEMAINFO._serialized_start=4059
+  _PAYLOADSCHEMAINFO._serialized_end=4216
+  _COLLECTIONINFO._serialized_start=4219
+  _COLLECTIONINFO._serialized_end=4661
+  _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_start=4544
+  _COLLECTIONINFO_PAYLOADSCHEMAENTRY._serialized_end=4623
+  _CHANGEALIASES._serialized_start=4663
+  _CHANGEALIASES._serialized_end=4754
+  _ALIASOPERATIONS._serialized_start=4757
+  _ALIASOPERATIONS._serialized_end=4919
+  _CREATEALIAS._serialized_start=4921
+  _CREATEALIAS._serialized_end=4979
+  _RENAMEALIAS._serialized_start=4981
+  _RENAMEALIAS._serialized_end=5042
+  _DELETEALIAS._serialized_start=5044
+  _DELETEALIAS._serialized_end=5077
+  _LISTALIASESREQUEST._serialized_start=5079
+  _LISTALIASESREQUEST._serialized_end=5099
+  _LISTCOLLECTIONALIASESREQUEST._serialized_start=5101
+  _LISTCOLLECTIONALIASESREQUEST._serialized_end=5156
+  _ALIASDESCRIPTION._serialized_start=5158
+  _ALIASDESCRIPTION._serialized_end=5221
+  _LISTALIASESRESPONSE._serialized_start=5223
+  _LISTALIASESRESPONSE._serialized_end=5301
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/collections_service_pb2.py` & `qdrant_client-1.1.4/qdrant_client/grpc/collections_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/collections_service_pb2_grpc.py` & `qdrant_client-1.1.4/qdrant_client/grpc/collections_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/json_with_int_pb2.py` & `qdrant_client-1.1.4/qdrant_client/grpc/json_with_int_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/points_pb2.py` & `qdrant_client-1.1.4/qdrant_client/grpc/points_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import json_with_int_pb2 as json__with__int__pb2
 from . import collections_pb2 as collections__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpoints.proto\x12\x06qdrant\x1a\x13json_with_int.proto\x1a\x11\x63ollections.proto\"8\n\rWriteOrdering\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.qdrant.WriteOrderingType\"Y\n\x0fReadConsistency\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1b.qdrant.ReadConsistencyTypeH\x00\x12\x10\n\x06\x66\x61\x63tor\x18\x02 \x01(\x04H\x00\x42\x07\n\x05value\"<\n\x07PointId\x12\r\n\x03num\x18\x01 \x01(\x04H\x00\x12\x0e\n\x04uuid\x18\x02 \x01(\tH\x00\x42\x12\n\x10point_id_options\"\x16\n\x06Vector\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\"\xa3\x01\n\x0cUpsertPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12#\n\x06points\x18\x03 \x03(\x0b\x32\x13.qdrant.PointStruct\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xa6\x01\n\x0c\x44\x65letePoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\x91\x02\n\tGetPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1c\n\x03ids\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x0cwith_payload\x18\x04 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x00\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x06 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x01\x88\x01\x01\x42\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x03\x10\x04\"\xc9\x02\n\x10SetPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x36\n\x07payload\x18\x03 \x03(\x0b\x32%.qdrant.SetPayloadPoints.PayloadEntry\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xe3\x01\n\x13\x44\x65letePayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x0c\n\x04keys\x18\x03 \x03(\t\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xac\x01\n\x12\x43learPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xaf\x02\n\x1a\x43reateFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12*\n\nfield_type\x18\x04 \x01(\x0e\x32\x11.qdrant.FieldTypeH\x01\x88\x01\x01\x12;\n\x12\x66ield_index_params\x18\x05 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x02\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x03\x88\x01\x01\x42\x07\n\x05_waitB\r\n\x0b_field_typeB\x15\n\x13_field_index_paramsB\x0b\n\t_ordering\"\xa0\x01\n\x1a\x44\x65leteFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"(\n\x16PayloadIncludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"(\n\x16PayloadExcludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"\xa1\x01\n\x13WithPayloadSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12\x31\n\x07include\x18\x02 \x01(\x0b\x32\x1e.qdrant.PayloadIncludeSelectorH\x00\x12\x31\n\x07\x65xclude\x18\x03 \x01(\x0b\x32\x1e.qdrant.PayloadExcludeSelectorH\x00\x42\x12\n\x10selector_options\"\x82\x01\n\x0cNamedVectors\x12\x32\n\x07vectors\x18\x01 \x03(\x0b\x32!.qdrant.NamedVectors.VectorsEntry\x1a>\n\x0cVectorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.qdrant.Vector:\x02\x38\x01\"g\n\x07Vectors\x12 \n\x06vector\x18\x01 \x01(\x0b\x32\x0e.qdrant.VectorH\x00\x12\'\n\x07vectors\x18\x02 \x01(\x0b\x32\x14.qdrant.NamedVectorsH\x00\x42\x11\n\x0fvectors_options\" \n\x0fVectorsSelector\x12\r\n\x05names\x18\x01 \x03(\t\"g\n\x13WithVectorsSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12*\n\x07include\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorsSelectorH\x00\x42\x12\n\x10selector_options\"\\\n\x18QuantizationSearchParams\x12\x13\n\x06ignore\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x14\n\x07rescore\x18\x02 \x01(\x08H\x01\x88\x01\x01\x42\t\n\x07_ignoreB\n\n\x08_rescore\"\x9c\x01\n\x0cSearchParams\x12\x14\n\x07hnsw_ef\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05\x65xact\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12;\n\x0cquantization\x18\x03 \x01(\x0b\x32 .qdrant.QuantizationSearchParamsH\x02\x88\x01\x01\x42\n\n\x08_hnsw_efB\x08\n\x06_exactB\x0f\n\r_quantization\"\xd7\x03\n\x0cSearchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\t \x01(\x04H\x01\x88\x01\x01\x12\x18\n\x0bvector_name\x18\n \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0b \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"\xa6\x01\n\x11SearchBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12+\n\rsearch_points\x18\x02 \x03(\x0b\x32\x14.qdrant.SearchPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\xe5\x02\n\x0cScrollPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12$\n\x06offset\x18\x03 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x08 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x08\n\x06_limitB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"S\n\x0eLookupLocation\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x18\n\x0bvector_name\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_vector_name\"\xc6\x04\n\x0fRecommendPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x08 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\n \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05using\x18\x0b \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0c \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x30\n\x0blookup_from\x18\r \x01(\x0b\x32\x16.qdrant.LookupLocationH\x04\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x05\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistencyJ\x04\x08\x06\x10\x07\"\xaf\x01\n\x14RecommendBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x10recommend_points\x18\x02 \x03(\x0b\x32\x17.qdrant.RecommendPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"d\n\x0b\x43ountPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12\x12\n\x05\x65xact\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_exact\"M\n\x17PointsOperationResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.UpdateResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x0cUpdateResult\x12\x14\n\x0coperation_id\x18\x01 \x01(\x04\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.qdrant.UpdateStatus\"\xf5\x01\n\x0bScoredPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x02 \x03(\x0b\x32 .qdrant.ScoredPoint.PayloadEntry\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x0f\n\x07version\x18\x05 \x01(\x04\x12%\n\x07vectors\x18\x06 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x04\x10\x05\"C\n\x0eSearchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"2\n\x0b\x42\x61tchResult\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\"H\n\x13SearchBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"B\n\rCountResponse\x12#\n\x06result\x18\x01 \x01(\x0b\x32\x13.qdrant.CountResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x8b\x01\n\x0eScrollResponse\x12.\n\x10next_page_offset\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12&\n\x06result\x18\x02 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x03 \x01(\x01\x42\x13\n\x11_next_page_offset\"\x1c\n\x0b\x43ountResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\"\xdb\x01\n\x0eRetrievedPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x34\n\x07payload\x18\x02 \x03(\x0b\x32#.qdrant.RetrievedPoint.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x03\x10\x04\"C\n\x0bGetResponse\x12&\n\x06result\x18\x01 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"F\n\x11RecommendResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"K\n\x16RecommendBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"q\n\x06\x46ilter\x12!\n\x06should\x18\x01 \x03(\x0b\x32\x11.qdrant.Condition\x12\x1f\n\x04must\x18\x02 \x03(\x0b\x32\x11.qdrant.Condition\x12#\n\x08must_not\x18\x03 \x03(\x0b\x32\x11.qdrant.Condition\"\xc2\x01\n\tCondition\x12\'\n\x05\x66ield\x18\x01 \x01(\x0b\x32\x16.qdrant.FieldConditionH\x00\x12,\n\x08is_empty\x18\x02 \x01(\x0b\x32\x18.qdrant.IsEmptyConditionH\x00\x12(\n\x06has_id\x18\x03 \x01(\x0b\x32\x16.qdrant.HasIdConditionH\x00\x12 \n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x42\x12\n\x10\x63ondition_one_of\"\x1f\n\x10IsEmptyCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"1\n\x0eHasIdCondition\x12\x1f\n\x06has_id\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xdd\x01\n\x0e\x46ieldCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05match\x18\x02 \x01(\x0b\x32\r.qdrant.Match\x12\x1c\n\x05range\x18\x03 \x01(\x0b\x32\r.qdrant.Range\x12\x30\n\x10geo_bounding_box\x18\x04 \x01(\x0b\x32\x16.qdrant.GeoBoundingBox\x12%\n\ngeo_radius\x18\x05 \x01(\x0b\x32\x11.qdrant.GeoRadius\x12)\n\x0cvalues_count\x18\x06 \x01(\x0b\x32\x13.qdrant.ValuesCount\"\xba\x01\n\x05Match\x12\x11\n\x07keyword\x18\x01 \x01(\tH\x00\x12\x11\n\x07integer\x18\x02 \x01(\x03H\x00\x12\x11\n\x07\x62oolean\x18\x03 \x01(\x08H\x00\x12\x0e\n\x04text\x18\x04 \x01(\tH\x00\x12+\n\x08keywords\x18\x05 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x12,\n\x08integers\x18\x06 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x42\r\n\x0bmatch_value\"\"\n\x0fRepeatedStrings\x12\x0f\n\x07strings\x18\x01 \x03(\t\"$\n\x10RepeatedIntegers\x12\x10\n\x08integers\x18\x01 \x03(\x03\"k\n\x05Range\x12\x0f\n\x02lt\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x01H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x01H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"\\\n\x0eGeoBoundingBox\x12\"\n\x08top_left\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12&\n\x0c\x62ottom_right\x18\x02 \x01(\x0b\x32\x10.qdrant.GeoPoint\"=\n\tGeoRadius\x12 \n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12\x0e\n\x06radius\x18\x02 \x01(\x02\"q\n\x0bValuesCount\x12\x0f\n\x02lt\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x04H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"u\n\x0ePointsSelector\x12\'\n\x06points\x18\x01 \x01(\x0b\x32\x15.qdrant.PointsIdsListH\x00\x12 \n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x42\x18\n\x16points_selector_one_of\"-\n\rPointsIdsList\x12\x1c\n\x03ids\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xd5\x01\n\x0bPointStruct\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x03 \x03(\x0b\x32 .qdrant.PointStruct.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x02\x10\x03\"$\n\x08GeoPoint\x12\x0b\n\x03lon\x18\x01 \x01(\x01\x12\x0b\n\x03lat\x18\x02 \x01(\x01*5\n\x11WriteOrderingType\x12\x08\n\x04Weak\x10\x00\x12\n\n\x06Medium\x10\x01\x12\n\n\x06Strong\x10\x02*8\n\x13ReadConsistencyType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08Majority\x10\x01\x12\n\n\x06Quorum\x10\x02*p\n\tFieldType\x12\x14\n\x10\x46ieldTypeKeyword\x10\x00\x12\x14\n\x10\x46ieldTypeInteger\x10\x01\x12\x12\n\x0e\x46ieldTypeFloat\x10\x02\x12\x10\n\x0c\x46ieldTypeGeo\x10\x03\x12\x11\n\rFieldTypeText\x10\x04*H\n\x0cUpdateStatus\x12\x17\n\x13UnknownUpdateStatus\x10\x00\x12\x10\n\x0c\x41\x63knowledged\x10\x01\x12\r\n\tCompleted\x10\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0cpoints.proto\x12\x06qdrant\x1a\x13json_with_int.proto\x1a\x11\x63ollections.proto\"8\n\rWriteOrdering\x12\'\n\x04type\x18\x01 \x01(\x0e\x32\x19.qdrant.WriteOrderingType\"Y\n\x0fReadConsistency\x12+\n\x04type\x18\x01 \x01(\x0e\x32\x1b.qdrant.ReadConsistencyTypeH\x00\x12\x10\n\x06\x66\x61\x63tor\x18\x02 \x01(\x04H\x00\x42\x07\n\x05value\"<\n\x07PointId\x12\r\n\x03num\x18\x01 \x01(\x04H\x00\x12\x0e\n\x04uuid\x18\x02 \x01(\tH\x00\x42\x12\n\x10point_id_options\"\x16\n\x06Vector\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x02\"\xa3\x01\n\x0cUpsertPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12#\n\x06points\x18\x03 \x03(\x0b\x32\x13.qdrant.PointStruct\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xa6\x01\n\x0c\x44\x65letePoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\x91\x02\n\tGetPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1c\n\x03ids\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x0cwith_payload\x18\x04 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x05 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x00\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x06 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x01\x88\x01\x01\x42\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x03\x10\x04\"\xc9\x02\n\x10SetPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x36\n\x07payload\x18\x03 \x03(\x0b\x32%.qdrant.SetPayloadPoints.PayloadEntry\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xe3\x01\n\x13\x44\x65letePayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x0c\n\x04keys\x18\x03 \x03(\t\x12\x34\n\x0fpoints_selector\x18\x05 \x01(\x0b\x32\x16.qdrant.PointsSelectorH\x01\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x02\x88\x01\x01\x42\x07\n\x05_waitB\x12\n\x10_points_selectorB\x0b\n\t_orderingJ\x04\x08\x04\x10\x05\"\xac\x01\n\x12\x43learPayloadPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12&\n\x06points\x18\x03 \x01(\x0b\x32\x16.qdrant.PointsSelector\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"\xaf\x02\n\x1a\x43reateFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12*\n\nfield_type\x18\x04 \x01(\x0e\x32\x11.qdrant.FieldTypeH\x01\x88\x01\x01\x12;\n\x12\x66ield_index_params\x18\x05 \x01(\x0b\x32\x1a.qdrant.PayloadIndexParamsH\x02\x88\x01\x01\x12,\n\x08ordering\x18\x06 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x03\x88\x01\x01\x42\x07\n\x05_waitB\r\n\x0b_field_typeB\x15\n\x13_field_index_paramsB\x0b\n\t_ordering\"\xa0\x01\n\x1a\x44\x65leteFieldIndexCollection\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x11\n\x04wait\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12\x12\n\nfield_name\x18\x03 \x01(\t\x12,\n\x08ordering\x18\x04 \x01(\x0b\x32\x15.qdrant.WriteOrderingH\x01\x88\x01\x01\x42\x07\n\x05_waitB\x0b\n\t_ordering\"(\n\x16PayloadIncludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"(\n\x16PayloadExcludeSelector\x12\x0e\n\x06\x66ields\x18\x01 \x03(\t\"\xa1\x01\n\x13WithPayloadSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12\x31\n\x07include\x18\x02 \x01(\x0b\x32\x1e.qdrant.PayloadIncludeSelectorH\x00\x12\x31\n\x07\x65xclude\x18\x03 \x01(\x0b\x32\x1e.qdrant.PayloadExcludeSelectorH\x00\x42\x12\n\x10selector_options\"\x82\x01\n\x0cNamedVectors\x12\x32\n\x07vectors\x18\x01 \x03(\x0b\x32!.qdrant.NamedVectors.VectorsEntry\x1a>\n\x0cVectorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.qdrant.Vector:\x02\x38\x01\"g\n\x07Vectors\x12 \n\x06vector\x18\x01 \x01(\x0b\x32\x0e.qdrant.VectorH\x00\x12\'\n\x07vectors\x18\x02 \x01(\x0b\x32\x14.qdrant.NamedVectorsH\x00\x42\x11\n\x0fvectors_options\" \n\x0fVectorsSelector\x12\r\n\x05names\x18\x01 \x03(\t\"g\n\x13WithVectorsSelector\x12\x10\n\x06\x65nable\x18\x01 \x01(\x08H\x00\x12*\n\x07include\x18\x02 \x01(\x0b\x32\x17.qdrant.VectorsSelectorH\x00\x42\x12\n\x10selector_options\"\\\n\x18QuantizationSearchParams\x12\x13\n\x06ignore\x18\x01 \x01(\x08H\x00\x88\x01\x01\x12\x14\n\x07rescore\x18\x02 \x01(\x08H\x01\x88\x01\x01\x42\t\n\x07_ignoreB\n\n\x08_rescore\"\x9c\x01\n\x0cSearchParams\x12\x14\n\x07hnsw_ef\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x12\n\x05\x65xact\x18\x02 \x01(\x08H\x01\x88\x01\x01\x12;\n\x0cquantization\x18\x03 \x01(\x0b\x32 .qdrant.QuantizationSearchParamsH\x02\x88\x01\x01\x42\n\n\x08_hnsw_efB\x08\n\x06_exactB\x0f\n\r_quantization\"\xd7\x03\n\x0cSearchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x0e\n\x06vector\x18\x02 \x03(\x02\x12\x1e\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x04 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x07 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\x08 \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\t \x01(\x04H\x01\x88\x01\x01\x12\x18\n\x0bvector_name\x18\n \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0b \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0c \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x04\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x0e\n\x0c_vector_nameB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"\xa6\x01\n\x11SearchBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12+\n\rsearch_points\x18\x02 \x03(\x0b\x32\x14.qdrant.SearchPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"\xe5\x02\n\x0cScrollPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12$\n\x06offset\x18\x03 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12\x12\n\x05limit\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x31\n\x0cwith_payload\x18\x06 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12\x36\n\x0cwith_vectors\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x02\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x08 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x08\n\x06_limitB\x0f\n\r_with_vectorsB\x13\n\x11_read_consistencyJ\x04\x08\x05\x10\x06\"S\n\x0eLookupLocation\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x18\n\x0bvector_name\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\x0e\n\x0c_vector_name\"\xc6\x04\n\x0fRecommendPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12!\n\x08positive\x18\x02 \x03(\x0b\x32\x0f.qdrant.PointId\x12!\n\x08negative\x18\x03 \x03(\x0b\x32\x0f.qdrant.PointId\x12\x1e\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.Filter\x12\r\n\x05limit\x18\x05 \x01(\x04\x12\x31\n\x0cwith_payload\x18\x07 \x01(\x0b\x32\x1b.qdrant.WithPayloadSelector\x12$\n\x06params\x18\x08 \x01(\x0b\x32\x14.qdrant.SearchParams\x12\x1c\n\x0fscore_threshold\x18\t \x01(\x02H\x00\x88\x01\x01\x12\x13\n\x06offset\x18\n \x01(\x04H\x01\x88\x01\x01\x12\x12\n\x05using\x18\x0b \x01(\tH\x02\x88\x01\x01\x12\x36\n\x0cwith_vectors\x18\x0c \x01(\x0b\x32\x1b.qdrant.WithVectorsSelectorH\x03\x88\x01\x01\x12\x30\n\x0blookup_from\x18\r \x01(\x0b\x32\x16.qdrant.LookupLocationH\x04\x88\x01\x01\x12\x36\n\x10read_consistency\x18\x0e \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x05\x88\x01\x01\x42\x12\n\x10_score_thresholdB\t\n\x07_offsetB\x08\n\x06_usingB\x0f\n\r_with_vectorsB\x0e\n\x0c_lookup_fromB\x13\n\x11_read_consistencyJ\x04\x08\x06\x10\x07\"\xaf\x01\n\x14RecommendBatchPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x10recommend_points\x18\x02 \x03(\x0b\x32\x17.qdrant.RecommendPoints\x12\x36\n\x10read_consistency\x18\x03 \x01(\x0b\x32\x17.qdrant.ReadConsistencyH\x00\x88\x01\x01\x42\x13\n\x11_read_consistency\"d\n\x0b\x43ountPoints\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x1e\n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.Filter\x12\x12\n\x05\x65xact\x18\x03 \x01(\x08H\x00\x88\x01\x01\x42\x08\n\x06_exact\"M\n\x17PointsOperationResponse\x12$\n\x06result\x18\x01 \x01(\x0b\x32\x14.qdrant.UpdateResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"J\n\x0cUpdateResult\x12\x14\n\x0coperation_id\x18\x01 \x01(\x04\x12$\n\x06status\x18\x02 \x01(\x0e\x32\x14.qdrant.UpdateStatus\"\xf5\x01\n\x0bScoredPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x02 \x03(\x0b\x32 .qdrant.ScoredPoint.PayloadEntry\x12\r\n\x05score\x18\x03 \x01(\x02\x12\x0f\n\x07version\x18\x05 \x01(\x04\x12%\n\x07vectors\x18\x06 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x04\x10\x05\"C\n\x0eSearchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"2\n\x0b\x42\x61tchResult\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\"H\n\x13SearchBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"B\n\rCountResponse\x12#\n\x06result\x18\x01 \x01(\x0b\x32\x13.qdrant.CountResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"\x8b\x01\n\x0eScrollResponse\x12.\n\x10next_page_offset\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointIdH\x00\x88\x01\x01\x12&\n\x06result\x18\x02 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x03 \x01(\x01\x42\x13\n\x11_next_page_offset\"\x1c\n\x0b\x43ountResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\"\xdb\x01\n\x0eRetrievedPoint\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x34\n\x07payload\x18\x02 \x03(\x0b\x32#.qdrant.RetrievedPoint.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x03\x10\x04\"C\n\x0bGetResponse\x12&\n\x06result\x18\x01 \x03(\x0b\x32\x16.qdrant.RetrievedPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"F\n\x11RecommendResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.ScoredPoint\x12\x0c\n\x04time\x18\x02 \x01(\x01\"K\n\x16RecommendBatchResponse\x12#\n\x06result\x18\x01 \x03(\x0b\x32\x13.qdrant.BatchResult\x12\x0c\n\x04time\x18\x02 \x01(\x01\"q\n\x06\x46ilter\x12!\n\x06should\x18\x01 \x03(\x0b\x32\x11.qdrant.Condition\x12\x1f\n\x04must\x18\x02 \x03(\x0b\x32\x11.qdrant.Condition\x12#\n\x08must_not\x18\x03 \x03(\x0b\x32\x11.qdrant.Condition\"\xee\x01\n\tCondition\x12\'\n\x05\x66ield\x18\x01 \x01(\x0b\x32\x16.qdrant.FieldConditionH\x00\x12,\n\x08is_empty\x18\x02 \x01(\x0b\x32\x18.qdrant.IsEmptyConditionH\x00\x12(\n\x06has_id\x18\x03 \x01(\x0b\x32\x16.qdrant.HasIdConditionH\x00\x12 \n\x06\x66ilter\x18\x04 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x12*\n\x07is_null\x18\x05 \x01(\x0b\x32\x17.qdrant.IsNullConditionH\x00\x42\x12\n\x10\x63ondition_one_of\"\x1f\n\x10IsEmptyCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"\x1e\n\x0fIsNullCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\"1\n\x0eHasIdCondition\x12\x1f\n\x06has_id\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xdd\x01\n\x0e\x46ieldCondition\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05match\x18\x02 \x01(\x0b\x32\r.qdrant.Match\x12\x1c\n\x05range\x18\x03 \x01(\x0b\x32\r.qdrant.Range\x12\x30\n\x10geo_bounding_box\x18\x04 \x01(\x0b\x32\x16.qdrant.GeoBoundingBox\x12%\n\ngeo_radius\x18\x05 \x01(\x0b\x32\x11.qdrant.GeoRadius\x12)\n\x0cvalues_count\x18\x06 \x01(\x0b\x32\x13.qdrant.ValuesCount\"\xba\x01\n\x05Match\x12\x11\n\x07keyword\x18\x01 \x01(\tH\x00\x12\x11\n\x07integer\x18\x02 \x01(\x03H\x00\x12\x11\n\x07\x62oolean\x18\x03 \x01(\x08H\x00\x12\x0e\n\x04text\x18\x04 \x01(\tH\x00\x12+\n\x08keywords\x18\x05 \x01(\x0b\x32\x17.qdrant.RepeatedStringsH\x00\x12,\n\x08integers\x18\x06 \x01(\x0b\x32\x18.qdrant.RepeatedIntegersH\x00\x42\r\n\x0bmatch_value\"\"\n\x0fRepeatedStrings\x12\x0f\n\x07strings\x18\x01 \x03(\t\"$\n\x10RepeatedIntegers\x12\x10\n\x08integers\x18\x01 \x03(\x03\"k\n\x05Range\x12\x0f\n\x02lt\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x01H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x01H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"\\\n\x0eGeoBoundingBox\x12\"\n\x08top_left\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12&\n\x0c\x62ottom_right\x18\x02 \x01(\x0b\x32\x10.qdrant.GeoPoint\"=\n\tGeoRadius\x12 \n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x10.qdrant.GeoPoint\x12\x0e\n\x06radius\x18\x02 \x01(\x02\"q\n\x0bValuesCount\x12\x0f\n\x02lt\x18\x01 \x01(\x04H\x00\x88\x01\x01\x12\x0f\n\x02gt\x18\x02 \x01(\x04H\x01\x88\x01\x01\x12\x10\n\x03gte\x18\x03 \x01(\x04H\x02\x88\x01\x01\x12\x10\n\x03lte\x18\x04 \x01(\x04H\x03\x88\x01\x01\x42\x05\n\x03_ltB\x05\n\x03_gtB\x06\n\x04_gteB\x06\n\x04_lte\"u\n\x0ePointsSelector\x12\'\n\x06points\x18\x01 \x01(\x0b\x32\x15.qdrant.PointsIdsListH\x00\x12 \n\x06\x66ilter\x18\x02 \x01(\x0b\x32\x0e.qdrant.FilterH\x00\x42\x18\n\x16points_selector_one_of\"-\n\rPointsIdsList\x12\x1c\n\x03ids\x18\x01 \x03(\x0b\x32\x0f.qdrant.PointId\"\xd5\x01\n\x0bPointStruct\x12\x1b\n\x02id\x18\x01 \x01(\x0b\x32\x0f.qdrant.PointId\x12\x31\n\x07payload\x18\x03 \x03(\x0b\x32 .qdrant.PointStruct.PayloadEntry\x12%\n\x07vectors\x18\x04 \x01(\x0b\x32\x0f.qdrant.VectorsH\x00\x88\x01\x01\x1a=\n\x0cPayloadEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1c\n\x05value\x18\x02 \x01(\x0b\x32\r.qdrant.Value:\x02\x38\x01\x42\n\n\x08_vectorsJ\x04\x08\x02\x10\x03\"$\n\x08GeoPoint\x12\x0b\n\x03lon\x18\x01 \x01(\x01\x12\x0b\n\x03lat\x18\x02 \x01(\x01*5\n\x11WriteOrderingType\x12\x08\n\x04Weak\x10\x00\x12\n\n\x06Medium\x10\x01\x12\n\n\x06Strong\x10\x02*8\n\x13ReadConsistencyType\x12\x07\n\x03\x41ll\x10\x00\x12\x0c\n\x08Majority\x10\x01\x12\n\n\x06Quorum\x10\x02*p\n\tFieldType\x12\x14\n\x10\x46ieldTypeKeyword\x10\x00\x12\x14\n\x10\x46ieldTypeInteger\x10\x01\x12\x12\n\x0e\x46ieldTypeFloat\x10\x02\x12\x10\n\x0c\x46ieldTypeGeo\x10\x03\x12\x11\n\rFieldTypeText\x10\x04*H\n\x0cUpdateStatus\x12\x17\n\x13UnknownUpdateStatus\x10\x00\x12\x10\n\x0c\x41\x63knowledged\x10\x01\x12\r\n\tCompleted\x10\x02\x62\x06proto3')
 
 _WRITEORDERINGTYPE = DESCRIPTOR.enum_types_by_name['WriteOrderingType']
 WriteOrderingType = enum_type_wrapper.EnumTypeWrapper(_WRITEORDERINGTYPE)
 _READCONSISTENCYTYPE = DESCRIPTOR.enum_types_by_name['ReadConsistencyType']
 ReadConsistencyType = enum_type_wrapper.EnumTypeWrapper(_READCONSISTENCYTYPE)
 _FIELDTYPE = DESCRIPTOR.enum_types_by_name['FieldType']
 FieldType = enum_type_wrapper.EnumTypeWrapper(_FIELDTYPE)
@@ -87,14 +87,15 @@
 _RETRIEVEDPOINT_PAYLOADENTRY = _RETRIEVEDPOINT.nested_types_by_name['PayloadEntry']
 _GETRESPONSE = DESCRIPTOR.message_types_by_name['GetResponse']
 _RECOMMENDRESPONSE = DESCRIPTOR.message_types_by_name['RecommendResponse']
 _RECOMMENDBATCHRESPONSE = DESCRIPTOR.message_types_by_name['RecommendBatchResponse']
 _FILTER = DESCRIPTOR.message_types_by_name['Filter']
 _CONDITION = DESCRIPTOR.message_types_by_name['Condition']
 _ISEMPTYCONDITION = DESCRIPTOR.message_types_by_name['IsEmptyCondition']
+_ISNULLCONDITION = DESCRIPTOR.message_types_by_name['IsNullCondition']
 _HASIDCONDITION = DESCRIPTOR.message_types_by_name['HasIdCondition']
 _FIELDCONDITION = DESCRIPTOR.message_types_by_name['FieldCondition']
 _MATCH = DESCRIPTOR.message_types_by_name['Match']
 _REPEATEDSTRINGS = DESCRIPTOR.message_types_by_name['RepeatedStrings']
 _REPEATEDINTEGERS = DESCRIPTOR.message_types_by_name['RepeatedIntegers']
 _RANGE = DESCRIPTOR.message_types_by_name['Range']
 _GEOBOUNDINGBOX = DESCRIPTOR.message_types_by_name['GeoBoundingBox']
@@ -441,14 +442,21 @@
 IsEmptyCondition = _reflection.GeneratedProtocolMessageType('IsEmptyCondition', (_message.Message,), {
   'DESCRIPTOR' : _ISEMPTYCONDITION,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.IsEmptyCondition)
   })
 _sym_db.RegisterMessage(IsEmptyCondition)
 
+IsNullCondition = _reflection.GeneratedProtocolMessageType('IsNullCondition', (_message.Message,), {
+  'DESCRIPTOR' : _ISNULLCONDITION,
+  '__module__' : 'points_pb2'
+  # @@protoc_insertion_point(class_scope:qdrant.IsNullCondition)
+  })
+_sym_db.RegisterMessage(IsNullCondition)
+
 HasIdCondition = _reflection.GeneratedProtocolMessageType('HasIdCondition', (_message.Message,), {
   'DESCRIPTOR' : _HASIDCONDITION,
   '__module__' : 'points_pb2'
   # @@protoc_insertion_point(class_scope:qdrant.HasIdCondition)
   })
 _sym_db.RegisterMessage(HasIdCondition)
 
@@ -553,22 +561,22 @@
   _NAMEDVECTORS_VECTORSENTRY._serialized_options = b'8\001'
   _SCOREDPOINT_PAYLOADENTRY._options = None
   _SCOREDPOINT_PAYLOADENTRY._serialized_options = b'8\001'
   _RETRIEVEDPOINT_PAYLOADENTRY._options = None
   _RETRIEVEDPOINT_PAYLOADENTRY._serialized_options = b'8\001'
   _POINTSTRUCT_PAYLOADENTRY._options = None
   _POINTSTRUCT_PAYLOADENTRY._serialized_options = b'8\001'
-  _WRITEORDERINGTYPE._serialized_start=7909
-  _WRITEORDERINGTYPE._serialized_end=7962
-  _READCONSISTENCYTYPE._serialized_start=7964
-  _READCONSISTENCYTYPE._serialized_end=8020
-  _FIELDTYPE._serialized_start=8022
-  _FIELDTYPE._serialized_end=8134
-  _UPDATESTATUS._serialized_start=8136
-  _UPDATESTATUS._serialized_end=8208
+  _WRITEORDERINGTYPE._serialized_start=7985
+  _WRITEORDERINGTYPE._serialized_end=8038
+  _READCONSISTENCYTYPE._serialized_start=8040
+  _READCONSISTENCYTYPE._serialized_end=8096
+  _FIELDTYPE._serialized_start=8098
+  _FIELDTYPE._serialized_end=8210
+  _UPDATESTATUS._serialized_start=8212
+  _UPDATESTATUS._serialized_end=8284
   _WRITEORDERING._serialized_start=64
   _WRITEORDERING._serialized_end=120
   _READCONSISTENCY._serialized_start=122
   _READCONSISTENCY._serialized_end=211
   _POINTID._serialized_start=213
   _POINTID._serialized_end=273
   _VECTOR._serialized_start=275
@@ -654,39 +662,41 @@
   _RECOMMENDRESPONSE._serialized_start=6076
   _RECOMMENDRESPONSE._serialized_end=6146
   _RECOMMENDBATCHRESPONSE._serialized_start=6148
   _RECOMMENDBATCHRESPONSE._serialized_end=6223
   _FILTER._serialized_start=6225
   _FILTER._serialized_end=6338
   _CONDITION._serialized_start=6341
-  _CONDITION._serialized_end=6535
-  _ISEMPTYCONDITION._serialized_start=6537
-  _ISEMPTYCONDITION._serialized_end=6568
-  _HASIDCONDITION._serialized_start=6570
-  _HASIDCONDITION._serialized_end=6619
-  _FIELDCONDITION._serialized_start=6622
-  _FIELDCONDITION._serialized_end=6843
-  _MATCH._serialized_start=6846
-  _MATCH._serialized_end=7032
-  _REPEATEDSTRINGS._serialized_start=7034
-  _REPEATEDSTRINGS._serialized_end=7068
-  _REPEATEDINTEGERS._serialized_start=7070
-  _REPEATEDINTEGERS._serialized_end=7106
-  _RANGE._serialized_start=7108
-  _RANGE._serialized_end=7215
-  _GEOBOUNDINGBOX._serialized_start=7217
-  _GEOBOUNDINGBOX._serialized_end=7309
-  _GEORADIUS._serialized_start=7311
-  _GEORADIUS._serialized_end=7372
-  _VALUESCOUNT._serialized_start=7374
-  _VALUESCOUNT._serialized_end=7487
-  _POINTSSELECTOR._serialized_start=7489
-  _POINTSSELECTOR._serialized_end=7606
-  _POINTSIDSLIST._serialized_start=7608
-  _POINTSIDSLIST._serialized_end=7653
-  _POINTSTRUCT._serialized_start=7656
-  _POINTSTRUCT._serialized_end=7869
+  _CONDITION._serialized_end=6579
+  _ISEMPTYCONDITION._serialized_start=6581
+  _ISEMPTYCONDITION._serialized_end=6612
+  _ISNULLCONDITION._serialized_start=6614
+  _ISNULLCONDITION._serialized_end=6644
+  _HASIDCONDITION._serialized_start=6646
+  _HASIDCONDITION._serialized_end=6695
+  _FIELDCONDITION._serialized_start=6698
+  _FIELDCONDITION._serialized_end=6919
+  _MATCH._serialized_start=6922
+  _MATCH._serialized_end=7108
+  _REPEATEDSTRINGS._serialized_start=7110
+  _REPEATEDSTRINGS._serialized_end=7144
+  _REPEATEDINTEGERS._serialized_start=7146
+  _REPEATEDINTEGERS._serialized_end=7182
+  _RANGE._serialized_start=7184
+  _RANGE._serialized_end=7291
+  _GEOBOUNDINGBOX._serialized_start=7293
+  _GEOBOUNDINGBOX._serialized_end=7385
+  _GEORADIUS._serialized_start=7387
+  _GEORADIUS._serialized_end=7448
+  _VALUESCOUNT._serialized_start=7450
+  _VALUESCOUNT._serialized_end=7563
+  _POINTSSELECTOR._serialized_start=7565
+  _POINTSSELECTOR._serialized_end=7682
+  _POINTSIDSLIST._serialized_start=7684
+  _POINTSIDSLIST._serialized_end=7729
+  _POINTSTRUCT._serialized_start=7732
+  _POINTSTRUCT._serialized_end=7945
   _POINTSTRUCT_PAYLOADENTRY._serialized_start=1131
   _POINTSTRUCT_PAYLOADENTRY._serialized_end=1192
-  _GEOPOINT._serialized_start=7871
-  _GEOPOINT._serialized_end=7907
+  _GEOPOINT._serialized_start=7947
+  _GEOPOINT._serialized_end=7983
 # @@protoc_insertion_point(module_scope)
```

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/points_service_pb2.py` & `qdrant_client-1.1.4/qdrant_client/grpc/points_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/points_service_pb2_grpc.py` & `qdrant_client-1.1.4/qdrant_client/grpc/points_service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 
 class PointsServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Upsert(self, request, context):
         """
-        Perform insert + updates on points. If point with given ID already exists - it will be overwritten.
+        Perform insert + updates on points. If a point with a given ID already exists - it will be overwritten.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Delete(self, request, context):
         """
```

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/qdrant_pb2.py` & `qdrant_client-1.1.4/qdrant_client/grpc/qdrant_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/qdrant_pb2_grpc.py` & `qdrant_client-1.1.4/qdrant_client/grpc/qdrant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/snapshots_service_pb2.py` & `qdrant_client-1.1.4/qdrant_client/grpc/snapshots_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/grpc/snapshots_service_pb2_grpc.py` & `qdrant_client-1.1.4/qdrant_client/grpc/snapshots_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/http/api/cluster_api.py` & `qdrant_client-1.1.4/qdrant_client/http/api/cluster_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/http/api/collections_api.py` & `qdrant_client-1.1.4/qdrant_client/http/api/collections_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8: noqa E501
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Set, Tuple, Union
+from typing import IO, TYPE_CHECKING, Any, Callable, Dict, List, Set, Tuple, Union
 
 from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.main import BaseModel
 from qdrant_client.http.models import *
 from qdrant_client.http.models import models as m
 
 SetIntStr = Set[Union[int, str]]
@@ -230,27 +230,33 @@
             params=query_params,
             json=body,
         )
 
     def _build_for_create_snapshot(
         self,
         collection_name: str,
+        wait: bool = None,
     ):
         """
         Create new snapshot for a collection
         """
         path_params = {
             "collection_name": str(collection_name),
         }
 
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+
         return self.api_client.request(
             type_=m.InlineResponse20010,
             method="POST",
             url="/collections/{collection_name}/snapshots",
             path_params=path_params,
+            params=query_params,
         )
 
     def _build_for_delete_collection(
         self,
         collection_name: str,
         timeout: int = None,
     ):
@@ -302,28 +308,34 @@
             params=query_params,
         )
 
     def _build_for_delete_snapshot(
         self,
         collection_name: str,
         snapshot_name: str,
+        wait: bool = None,
     ):
         """
         Delete snapshot for a collection
         """
         path_params = {
             "collection_name": str(collection_name),
             "snapshot_name": str(snapshot_name),
         }
 
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+
         return self.api_client.request(
             type_=m.InlineResponse2003,
             method="DELETE",
             url="/collections/{collection_name}/snapshots/{snapshot_name}",
             path_params=path_params,
+            params=query_params,
         )
 
     def _build_for_get_collection(
         self,
         collection_name: str,
     ):
         """
@@ -444,14 +456,49 @@
             method="PUT",
             url="/collections/{collection_name}/snapshots/recover",
             path_params=path_params,
             params=query_params,
             json=body,
         )
 
+    def _build_for_recover_from_uploaded_snapshot(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        priority: SnapshotPriority = None,
+        snapshot: IO[Any] = None,
+    ):
+        """
+        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
+        """
+        path_params = {
+            "collection_name": str(collection_name),
+        }
+
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+        if priority is not None:
+            query_params["priority"] = str(priority)
+
+        files: Dict[str, IO[Any]] = {}  # noqa F841
+        data: Dict[str, Any] = {}  # noqa F841
+        if snapshot is not None:
+            files["snapshot"] = snapshot
+
+        return self.api_client.request(
+            type_=m.InlineResponse2003,
+            method="POST",
+            url="/collections/{collection_name}/snapshots/upload",
+            path_params=path_params,
+            params=query_params,
+            data=data,
+            files=files,
+        )
+
     def _build_for_update_aliases(
         self,
         timeout: int = None,
         change_aliases_operation: m.ChangeAliasesOperation = None,
     ):
         query_params = {}
         if timeout is not None:
@@ -560,20 +607,22 @@
             ordering=ordering,
             create_field_index=create_field_index,
         )
 
     async def create_snapshot(
         self,
         collection_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse20010:
         """
         Create new snapshot for a collection
         """
         return await self._build_for_create_snapshot(
             collection_name=collection_name,
+            wait=wait,
         )
 
     async def delete_collection(
         self,
         collection_name: str,
         timeout: int = None,
     ) -> m.InlineResponse2003:
@@ -602,21 +651,23 @@
             ordering=ordering,
         )
 
     async def delete_snapshot(
         self,
         collection_name: str,
         snapshot_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse2003:
         """
         Delete snapshot for a collection
         """
         return await self._build_for_delete_snapshot(
             collection_name=collection_name,
             snapshot_name=snapshot_name,
+            wait=wait,
         )
 
     async def get_collection(
         self,
         collection_name: str,
     ) -> m.InlineResponse2005:
         """
@@ -688,14 +739,31 @@
         """
         return await self._build_for_recover_from_snapshot(
             collection_name=collection_name,
             wait=wait,
             snapshot_recover=snapshot_recover,
         )
 
+    async def recover_from_uploaded_snapshot(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        priority: SnapshotPriority = None,
+        snapshot: IO[Any] = None,
+    ) -> m.InlineResponse2003:
+        """
+        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
+        """
+        return await self._build_for_recover_from_uploaded_snapshot(
+            collection_name=collection_name,
+            wait=wait,
+            priority=priority,
+            snapshot=snapshot,
+        )
+
     async def update_aliases(
         self,
         timeout: int = None,
         change_aliases_operation: m.ChangeAliasesOperation = None,
     ) -> m.InlineResponse2003:
         return await self._build_for_update_aliases(
             timeout=timeout,
@@ -773,20 +841,22 @@
             ordering=ordering,
             create_field_index=create_field_index,
         )
 
     def create_snapshot(
         self,
         collection_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse20010:
         """
         Create new snapshot for a collection
         """
         return self._build_for_create_snapshot(
             collection_name=collection_name,
+            wait=wait,
         )
 
     def delete_collection(
         self,
         collection_name: str,
         timeout: int = None,
     ) -> m.InlineResponse2003:
@@ -815,21 +885,23 @@
             ordering=ordering,
         )
 
     def delete_snapshot(
         self,
         collection_name: str,
         snapshot_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse2003:
         """
         Delete snapshot for a collection
         """
         return self._build_for_delete_snapshot(
             collection_name=collection_name,
             snapshot_name=snapshot_name,
+            wait=wait,
         )
 
     def get_collection(
         self,
         collection_name: str,
     ) -> m.InlineResponse2005:
         """
@@ -901,14 +973,31 @@
         """
         return self._build_for_recover_from_snapshot(
             collection_name=collection_name,
             wait=wait,
             snapshot_recover=snapshot_recover,
         )
 
+    def recover_from_uploaded_snapshot(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        priority: SnapshotPriority = None,
+        snapshot: IO[Any] = None,
+    ) -> m.InlineResponse2003:
+        """
+        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
+        """
+        return self._build_for_recover_from_uploaded_snapshot(
+            collection_name=collection_name,
+            wait=wait,
+            priority=priority,
+            snapshot=snapshot,
+        )
+
     def update_aliases(
         self,
         timeout: int = None,
         change_aliases_operation: m.ChangeAliasesOperation = None,
     ) -> m.InlineResponse2003:
         return self._build_for_update_aliases(
             timeout=timeout,
```

### Comparing `qdrant_client-1.1.3/qdrant_client/http/api/points_api.py` & `qdrant_client-1.1.4/qdrant_client/http/api/points_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/http/api/service_api.py` & `qdrant_client-1.1.4/qdrant_client/http/api/service_api.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/http/api/snapshots_api.py` & `qdrant_client-1.1.4/qdrant_client/http/api/snapshots_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8: noqa E501
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Set, Tuple, Union
+from typing import IO, TYPE_CHECKING, Any, Callable, Dict, List, Set, Tuple, Union
 
 from pydantic.json import ENCODERS_BY_TYPE
 from pydantic.main import BaseModel
 from qdrant_client.http.models import *
 from qdrant_client.http.models import models as m
 
 SetIntStr = Set[Union[int, str]]
@@ -152,78 +152,102 @@
 
 class _SnapshotsApi:
     def __init__(self, api_client: "Union[ApiClient, AsyncApiClient]"):
         self.api_client = api_client
 
     def _build_for_create_full_snapshot(
         self,
+        wait: bool = None,
     ):
         """
         Create new snapshot of the whole storage
         """
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+
         return self.api_client.request(
             type_=m.InlineResponse20010,
             method="POST",
             url="/snapshots",
+            params=query_params,
         )
 
     def _build_for_create_snapshot(
         self,
         collection_name: str,
+        wait: bool = None,
     ):
         """
         Create new snapshot for a collection
         """
         path_params = {
             "collection_name": str(collection_name),
         }
 
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+
         return self.api_client.request(
             type_=m.InlineResponse20010,
             method="POST",
             url="/collections/{collection_name}/snapshots",
             path_params=path_params,
+            params=query_params,
         )
 
     def _build_for_delete_full_snapshot(
         self,
         snapshot_name: str,
+        wait: bool = None,
     ):
         """
         Delete snapshot of the whole storage
         """
         path_params = {
             "snapshot_name": str(snapshot_name),
         }
 
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+
         return self.api_client.request(
             type_=m.InlineResponse2003,
             method="DELETE",
             url="/snapshots/{snapshot_name}",
             path_params=path_params,
+            params=query_params,
         )
 
     def _build_for_delete_snapshot(
         self,
         collection_name: str,
         snapshot_name: str,
+        wait: bool = None,
     ):
         """
         Delete snapshot for a collection
         """
         path_params = {
             "collection_name": str(collection_name),
             "snapshot_name": str(snapshot_name),
         }
 
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+
         return self.api_client.request(
             type_=m.InlineResponse2003,
             method="DELETE",
             url="/collections/{collection_name}/snapshots/{snapshot_name}",
             path_params=path_params,
+            params=query_params,
         )
 
     def _build_for_get_full_snapshot(
         self,
         snapshot_name: str,
     ):
         """
@@ -314,57 +338,101 @@
             method="PUT",
             url="/collections/{collection_name}/snapshots/recover",
             path_params=path_params,
             params=query_params,
             json=body,
         )
 
+    def _build_for_recover_from_uploaded_snapshot(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        priority: SnapshotPriority = None,
+        snapshot: IO[Any] = None,
+    ):
+        """
+        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
+        """
+        path_params = {
+            "collection_name": str(collection_name),
+        }
+
+        query_params = {}
+        if wait is not None:
+            query_params["wait"] = str(wait).lower()
+        if priority is not None:
+            query_params["priority"] = str(priority)
+
+        files: Dict[str, IO[Any]] = {}  # noqa F841
+        data: Dict[str, Any] = {}  # noqa F841
+        if snapshot is not None:
+            files["snapshot"] = snapshot
+
+        return self.api_client.request(
+            type_=m.InlineResponse2003,
+            method="POST",
+            url="/collections/{collection_name}/snapshots/upload",
+            path_params=path_params,
+            params=query_params,
+            data=data,
+            files=files,
+        )
+
 
 class AsyncSnapshotsApi(_SnapshotsApi):
     async def create_full_snapshot(
         self,
+        wait: bool = None,
     ) -> m.InlineResponse20010:
         """
         Create new snapshot of the whole storage
         """
-        return await self._build_for_create_full_snapshot()
+        return await self._build_for_create_full_snapshot(
+            wait=wait,
+        )
 
     async def create_snapshot(
         self,
         collection_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse20010:
         """
         Create new snapshot for a collection
         """
         return await self._build_for_create_snapshot(
             collection_name=collection_name,
+            wait=wait,
         )
 
     async def delete_full_snapshot(
         self,
         snapshot_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse2003:
         """
         Delete snapshot of the whole storage
         """
         return await self._build_for_delete_full_snapshot(
             snapshot_name=snapshot_name,
+            wait=wait,
         )
 
     async def delete_snapshot(
         self,
         collection_name: str,
         snapshot_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse2003:
         """
         Delete snapshot for a collection
         """
         return await self._build_for_delete_snapshot(
             collection_name=collection_name,
             snapshot_name=snapshot_name,
+            wait=wait,
         )
 
     async def get_full_snapshot(
         self,
         snapshot_name: str,
     ) -> file:
         """
@@ -417,57 +485,83 @@
         """
         return await self._build_for_recover_from_snapshot(
             collection_name=collection_name,
             wait=wait,
             snapshot_recover=snapshot_recover,
         )
 
+    async def recover_from_uploaded_snapshot(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        priority: SnapshotPriority = None,
+        snapshot: IO[Any] = None,
+    ) -> m.InlineResponse2003:
+        """
+        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
+        """
+        return await self._build_for_recover_from_uploaded_snapshot(
+            collection_name=collection_name,
+            wait=wait,
+            priority=priority,
+            snapshot=snapshot,
+        )
+
 
 class SyncSnapshotsApi(_SnapshotsApi):
     def create_full_snapshot(
         self,
+        wait: bool = None,
     ) -> m.InlineResponse20010:
         """
         Create new snapshot of the whole storage
         """
-        return self._build_for_create_full_snapshot()
+        return self._build_for_create_full_snapshot(
+            wait=wait,
+        )
 
     def create_snapshot(
         self,
         collection_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse20010:
         """
         Create new snapshot for a collection
         """
         return self._build_for_create_snapshot(
             collection_name=collection_name,
+            wait=wait,
         )
 
     def delete_full_snapshot(
         self,
         snapshot_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse2003:
         """
         Delete snapshot of the whole storage
         """
         return self._build_for_delete_full_snapshot(
             snapshot_name=snapshot_name,
+            wait=wait,
         )
 
     def delete_snapshot(
         self,
         collection_name: str,
         snapshot_name: str,
+        wait: bool = None,
     ) -> m.InlineResponse2003:
         """
         Delete snapshot for a collection
         """
         return self._build_for_delete_snapshot(
             collection_name=collection_name,
             snapshot_name=snapshot_name,
+            wait=wait,
         )
 
     def get_full_snapshot(
         self,
         snapshot_name: str,
     ) -> file:
         """
@@ -519,7 +613,24 @@
         Recover local collection data from a snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
         """
         return self._build_for_recover_from_snapshot(
             collection_name=collection_name,
             wait=wait,
             snapshot_recover=snapshot_recover,
         )
+
+    def recover_from_uploaded_snapshot(
+        self,
+        collection_name: str,
+        wait: bool = None,
+        priority: SnapshotPriority = None,
+        snapshot: IO[Any] = None,
+    ) -> m.InlineResponse2003:
+        """
+        Recover local collection data from an uploaded snapshot. This will overwrite any data, stored on this node, for the collection. If collection does not exist - it will be created.
+        """
+        return self._build_for_recover_from_uploaded_snapshot(
+            collection_name=collection_name,
+            wait=wait,
+            priority=priority,
+            snapshot=snapshot,
+        )
```

### Comparing `qdrant_client-1.1.3/qdrant_client/http/api_client.py` & `qdrant_client-1.1.4/qdrant_client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/http/exceptions.py` & `qdrant_client-1.1.4/qdrant_client/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/http/models/models.py` & `qdrant_client-1.1.4/qdrant_client/http/models/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 
 class AppBuildTelemetry(BaseModel):
     name: str = Field(..., description="")
     version: str = Field(..., description="")
     features: Optional["AppFeaturesTelemetry"] = Field(default=None, description="")
     system: Optional["RunningEnvironmentTelemetry"] = Field(default=None, description="")
+    startup: datetime = Field(..., description="")
 
 
 class AppFeaturesTelemetry(BaseModel):
     debug: bool = Field(..., description="")
     web_feature: bool = Field(..., description="")
     service_debug_feature: bool = Field(..., description="")
 
@@ -465,27 +466,27 @@
 class HnswConfigDiff(BaseModel):
     m: Optional[int] = Field(
         default=None,
         description="Number of edges per node in the index graph. Larger the value - more accurate the search, more space required.",
     )
     ef_construct: Optional[int] = Field(
         default=None,
-        description="Number of neighbours to consider during the index building. Larger the value - more accurate the search, more time required to build index.",
+        description="Number of neighbours to consider during the index building. Larger the value - more accurate the search, more time required to build the index.",
     )
     full_scan_threshold: Optional[int] = Field(
         default=None,
         description="Minimal size (in KiloBytes) of vectors for additional payload-based indexing. If payload chunk is smaller than `full_scan_threshold_kb` additional indexing won&#x27;t be used - in this case full-scan search should be preferred by query planner and additional indexing is not required. Note: 1Kb = 1 vector of size 256",
     )
     max_indexing_threads: Optional[int] = Field(
         default=None,
         description="Number of parallel threads used for background index building. If 0 - auto selection.",
     )
     on_disk: Optional[bool] = Field(
         default=None,
-        description="Store HNSW index on disk. If set to false, index will be stored in RAM. Default: false",
+        description="Store HNSW index on disk. If set to false, the index will be stored in RAM. Default: false",
     )
     payload_m: Optional[int] = Field(
         default=None,
         description="Custom M param for additional payload-aware HNSW links. If not set, default M will be used.",
     )
 
 
@@ -530,15 +531,15 @@
 
 
 class InlineResponse200(BaseModel):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
-    result: Optional[List["TelemetryData"]] = Field(default=None, description="")
+    result: Optional["TelemetryData"] = Field(default=None, description="")
 
 
 class InlineResponse2001(BaseModel):
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
@@ -661,22 +662,37 @@
     time: Optional[float] = Field(default=None, description="Time spent to process this request")
     status: Literal[
         "ok",
     ] = Field(None, description="")
     result: Optional[List["SnapshotDescription"]] = Field(default=None, description="")
 
 
+class InlineResponse202(BaseModel):
+    time: Optional[float] = Field(default=None, description="Time spent to process this request")
+    status: Literal[
+        "accepted",
+    ] = Field(None, description="")
+
+
 class IsEmptyCondition(BaseModel):
     """
     Select points with empty payload for a specified field
     """
 
     is_empty: "PayloadField" = Field(..., description="Select points with empty payload for a specified field")
 
 
+class IsNullCondition(BaseModel):
+    """
+    Select points with null payload for a specified field
+    """
+
+    is_null: "PayloadField" = Field(..., description="Select points with null payload for a specified field")
+
+
 class LocalShardInfo(BaseModel):
     shard_id: int = Field(..., description="Local shard id")
     points_count: int = Field(..., description="Number of points in the shard")
     state: "ReplicaState" = Field(..., description="")
 
 
 class LocalShardTelemetry(BaseModel):
@@ -756,14 +772,15 @@
 
 class OperationDurationStatistics(BaseModel):
     count: int = Field(..., description="")
     fail_count: Optional[int] = Field(default=None, description="")
     avg_duration_micros: Optional[float] = Field(default=None, description="")
     min_duration_micros: Optional[float] = Field(default=None, description="")
     max_duration_micros: Optional[float] = Field(default=None, description="")
+    last_responded: Optional[datetime] = Field(default=None, description="")
 
 
 class OptimizerTelemetry(BaseModel):
     status: "OptimizersStatus" = Field(..., description="")
     optimizations: "OperationDurationStatistics" = Field(..., description="")
 
 
@@ -773,15 +790,15 @@
         description="The minimal fraction of deleted vectors in a segment, required to perform segment optimization",
     )
     vacuum_min_vector_number: int = Field(
         ..., description="The minimal number of vectors in a segment, required to perform segment optimization"
     )
     default_segment_number: int = Field(
         ...,
-        description="Target amount of segments optimizer will try to keep. Real amount of segments may vary depending on multiple parameters: - Amount of stored points - Current write RPS  It is recommended to select default number of segments as a factor of the number of search threads, so that each segment would be handled evenly by one of the threads If `default_segment_number = 0`, will be automatically selected by the number of available CPUs",
+        description="Target amount of segments optimizer will try to keep. Real amount of segments may vary depending on multiple parameters: - Amount of stored points - Current write RPS  It is recommended to select default number of segments as a factor of the number of search threads, so that each segment would be handled evenly by one of the threads. If `default_segment_number = 0`, will be automatically selected by the number of available CPUs.",
     )
     max_segment_size: Optional[int] = Field(
         default=None,
         description="Do not create segments larger this size (in KiloBytes). Large segments might require disproportionately long indexation times, therefore it makes sense to limit the size of segments.  If indexation speed have more priority for your - make this parameter lower. If search speed is more important - make this parameter higher. Note: 1Kb = 1 vector of size 256 If not set, will be automatically selected considering the number of available CPUs.",
     )
     memmap_threshold: Optional[int] = Field(
         default=None,
@@ -1096,15 +1113,15 @@
     scalar: "ScalarQuantizationConfig" = Field(..., description="")
 
 
 class ScalarQuantizationConfig(BaseModel):
     type: "ScalarType" = Field(..., description="")
     quantile: Optional[float] = Field(
         default=None,
-        description="Quantile for quantization. Expected value range in (0, 1.0]. If not set - use the whole range of values",
+        description="Quantile for quantization. Expected value range in [0.5, 1.0]. If not set - use the whole range of values",
     )
     always_ram: Optional[bool] = Field(
         default=None,
         description="If true - quantized vectors always will be stored in RAM, ignoring the config of main storage",
     )
 
 
@@ -1364,14 +1381,20 @@
 class VectorDataConfig(BaseModel):
     """
     Config of single vector data storage
     """
 
     size: int = Field(..., description="Size of a vectors used")
     distance: "Distance" = Field(..., description="Config of single vector data storage")
+    hnsw_config: Optional["HnswConfig"] = Field(
+        default=None, description="Vector specific HNSW config that overrides collection config"
+    )
+    quantization_config: Optional["QuantizationConfig"] = Field(
+        default=None, description="Vector specific quantization config that overrides collection config"
+    )
 
 
 class VectorIndexSearchesTelemetry(BaseModel):
     index_name: Optional[str] = Field(default=None, description="")
     unfiltered_plain: "OperationDurationStatistics" = Field(..., description="")
     unfiltered_hnsw: "OperationDurationStatistics" = Field(..., description="")
     filtered_plain: "OperationDurationStatistics" = Field(..., description="")
@@ -1384,14 +1407,22 @@
 class VectorParams(BaseModel):
     """
     Params of single vector data storage
     """
 
     size: int = Field(..., description="Size of a vectors used")
     distance: "Distance" = Field(..., description="Params of single vector data storage")
+    hnsw_config: Optional["HnswConfigDiff"] = Field(
+        default=None,
+        description="Custom params for HNSW index. If none - values from collection configuration are used.",
+    )
+    quantization_config: Optional["QuantizationConfig"] = Field(
+        default=None,
+        description="Custom params for quantization. If none - values from collection configuration are used.",
+    )
 
 
 class WalConfig(BaseModel):
     wal_capacity_mb: int = Field(..., description="Size of a single WAL segment in MB")
     wal_segments_ahead: int = Field(..., description="Number of WAL segments to create ahead of actually used ones")
 
 
@@ -1438,14 +1469,15 @@
 CollectionTelemetryEnum = Union[
     CollectionTelemetry,
     CollectionsAggregatedTelemetry,
 ]
 Condition = Union[
     FieldCondition,
     IsEmptyCondition,
+    IsNullCondition,
     HasIdCondition,
     Filter,
 ]
 ConsensusThreadStatus = Union[
     ConsensusThreadStatusOneOf,
     ConsensusThreadStatusOneOf1,
     ConsensusThreadStatusOneOf2,
```

### Comparing `qdrant_client-1.1.3/qdrant_client/local/distances.py` & `qdrant_client-1.1.4/qdrant_client/local/distances.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/local/geo.py` & `qdrant_client-1.1.4/qdrant_client/local/geo.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/local/local_collection.py` & `qdrant_client-1.1.4/qdrant_client/local/local_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,17 @@
         result = []
 
         for point_id in ids:
             if point_id not in self.ids:
                 continue
 
             idx = self.ids[point_id]
+            if self.deleted[idx] == 1:
+                continue
+
             result.append(
                 models.Record(
                     id=point_id,
                     payload=self._get_payload(idx, with_payload),
                     vector=self._get_vectors(idx, with_vectors),
                 )
             )
```

### Comparing `qdrant_client-1.1.3/qdrant_client/local/payload_filters.py` & `qdrant_client-1.1.4/qdrant_client/local/payload_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,17 +73,23 @@
         return value in condition.any
     raise ValueError(f"Unknown match condition: {condition}")
 
 
 def check_condition(
     condition: models.Condition, payload: dict, point_id: models.ExtendedPointId
 ) -> bool:
-    if isinstance(condition, models.IsEmptyCondition):
+    if isinstance(condition, models.IsNullCondition):
+        values = value_by_key(payload, condition.is_null.key)
+        if values is None:
+            return False
+        if any(v is None for v in values):
+            return True
+    elif isinstance(condition, models.IsEmptyCondition):
         values = value_by_key(payload, condition.is_empty.key)
-        if values is None or len(values) == 0:
+        if values is None or len(values) == 0 or all(v is None for v in values):
             return True
     elif isinstance(condition, models.HasIdCondition):
         if point_id in condition.has_id:
             return True
     elif isinstance(condition, models.FieldCondition):
         values = value_by_key(payload, condition.key)
         if condition.match is not None:
```

### Comparing `qdrant_client-1.1.3/qdrant_client/local/payload_value_extractor.py` & `qdrant_client-1.1.4/qdrant_client/local/payload_value_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,21 +68,25 @@
         "address": {
             "city": "New York",
         },
         "location": [
             {"name": "home", "counts": [1, 2, 3]},
             {"name": "work", "counts": [4, 5, 6]},
         ],
+        "nested": [{"empty": []}, {"empty": []}, {"empty": None}],
+        "the_null": None,
     }
     assert value_by_key(payload, "name") == ["John"]
     assert value_by_key(payload, "address.city") == ["New York"]
     assert value_by_key(payload, "location[].name") == ["home", "work"]
     assert value_by_key(payload, "location[0].name") == ["home"]
     assert value_by_key(payload, "location[1].name") == ["work"]
     assert value_by_key(payload, "location[2].name") is None
     assert value_by_key(payload, "location[].name[0]") is None
     assert value_by_key(payload, "location[0]") is None
     assert value_by_key(payload, "not_exits") is None
     assert value_by_key(payload, "address") == [{"city": "New York"}]
     assert value_by_key(payload, "address.city[0]") is None
     assert value_by_key(payload, "counts") == [1, 2, 3]
     assert value_by_key(payload, "location[].counts") == [1, 2, 3, 4, 5, 6]
+    assert value_by_key(payload, "nested[].empty") == [None]
+    assert value_by_key(payload, "the_null") == [None]
```

### Comparing `qdrant_client-1.1.3/qdrant_client/local/persistence.py` & `qdrant_client-1.1.4/qdrant_client/local/persistence.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/local/qdrant_local.py` & `qdrant_client-1.1.4/qdrant_client/local/qdrant_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import logging
 import os
 import shutil
+import numpy as np
 from itertools import zip_longest
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Union
 
 from qdrant_client.client_base import QdrantBase
 from qdrant_client.conversions import common_types as types
 from qdrant_client.http import models as rest_models
 from qdrant_client.local.local_collection import LocalCollection
@@ -81,20 +82,20 @@
     def search_batch(
         self, collection_name: str, requests: Sequence[types.SearchRequest], **kwargs: Any
     ) -> List[List[types.ScoredPoint]]:
         collection = self._get_collection(collection_name)
 
         return [
             collection.search(
-                query_vector=request.query_vector,
-                query_filter=request.query_filter,
+                query_vector=request.vector,
+                query_filter=request.filter,
                 limit=request.limit,
                 offset=request.offset,
                 with_payload=request.with_payload,
-                with_vectors=request.with_vectors,
+                with_vectors=request.with_vector,
                 score_threshold=request.score_threshold,
             )
             for request in requests
         ]
 
     def search(
         self,
@@ -130,19 +131,19 @@
     ) -> List[List[types.ScoredPoint]]:
         collection = self._get_collection(collection_name)
 
         return [
             collection.recommend(
                 positive=request.positive,
                 negative=request.negative,
-                query_filter=request.query_filter,
+                query_filter=request.filter,
                 limit=request.limit,
                 offset=request.offset,
                 with_payload=request.with_payload,
-                with_vectors=request.with_vectors,
+                with_vectors=request.with_vector,
                 score_threshold=request.score_threshold,
             )
             for request in requests
         ]
 
     def recommend(
         self,
@@ -417,19 +418,19 @@
         **kwargs: Any,
     ) -> None:
         collection = self._get_collection(collection_name)
         collection.upsert(
             [
                 rest_models.PointStruct(
                     id=point_id or idx,
-                    vector=vector or {},
+                    vector=(vector.tolist() if isinstance(vector, np.ndarray) else vector) or {},
                     payload=payload or {},
                 )
                 for idx, (point_id, vector, payload) in enumerate(
-                    zip_longest(ids or [], vectors, payload or [])
+                    zip_longest(ids or [], iter(vectors), payload or [])
                 )
             ]
         )
 
     def create_payload_index(
         self,
         collection_name: str,
```

### Comparing `qdrant_client-1.1.3/qdrant_client/parallel_processor.py` & `qdrant_client-1.1.4/qdrant_client/parallel_processor.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/proto/collections.proto` & `qdrant_client-1.1.4/qdrant_client/proto/collections.proto`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 syntax = "proto3";
 package qdrant;
 
 message VectorParams {
   uint64 size = 1; // Size of the vectors
   Distance distance = 2; // Distance function used for comparing vectors
+  optional HnswConfigDiff hnsw_config = 3; // Configuration of vector HNSW graph. If omitted - the collection configuration will be used
+  optional QuantizationConfig quantization_config = 4; // Configuration of vector quantization config. If omitted - the collection configuration will be used
 }
 
 message VectorParamsMap {
   map<string, VectorParams> map = 1;
 }
 
 message VectorsConfig {
@@ -73,30 +75,30 @@
 
 message HnswConfigDiff {
   /*
   Number of edges per node in the index graph. Larger the value - more accurate the search, more space required.
    */
   optional uint64 m = 1;
   /*
-  Number of neighbours to consider during the index building. Larger the value - more accurate the search, more time required to build index.
+  Number of neighbours to consider during the index building. Larger the value - more accurate the search, more time required to build the index.
   */
   optional uint64 ef_construct = 2;
   /*
   Minimal size (in KiloBytes) of vectors for additional payload-based indexing.
-  If payload chunk is smaller than `full_scan_threshold` additional indexing won't be used -
+  If the payload chunk is smaller than `full_scan_threshold` additional indexing won't be used -
   in this case full-scan search should be preferred by query planner and additional indexing is not required.
-  Note: 1Kb = 1 vector of size 256
+  Note: 1 Kb = 1 vector of size 256
   */
   optional uint64 full_scan_threshold = 3;
   /*
   Number of parallel threads used for background index building. If 0 - auto selection.
    */
   optional uint64 max_indexing_threads = 4;
   /*
-  Store HNSW index on disk. If set to false, index will be stored in RAM.
+  Store HNSW index on disk. If set to false, the index will be stored in RAM.
    */
   optional bool on_disk = 5;
   /*
    Number of additional payload-aware links per node in the index graph. If not set - regular M parameter will be used.
    */
   optional uint64 payload_m = 6;
 }
@@ -112,37 +114,37 @@
    */
   optional double deleted_threshold = 1;
   /*
   The minimal number of vectors in a segment, required to perform segment optimization
    */
   optional uint64 vacuum_min_vector_number = 2;
   /*
-  Target amount of segments optimizer will try to keep.
+  Target amount of segments the optimizer will try to keep.
   Real amount of segments may vary depending on multiple parameters:
 
    - Amount of stored points.
    - Current write RPS.
 
-  It is recommended to select default number of segments as a factor of the number of search threads,
+  It is recommended to select the default number of segments as a factor of the number of search threads,
   so that each segment would be handled evenly by one of the threads.
   */
   optional uint64 default_segment_number = 3;
   /*
   Do not create segments larger this size (in KiloBytes).
   Large segments might require disproportionately long indexation times,
   therefore it makes sense to limit the size of segments.
 
-  If indexation speed have more priority for your - make this parameter lower.
+  If indexation speed has more priority for you - make this parameter lower.
   If search speed is more important - make this parameter higher.
   Note: 1Kb = 1 vector of size 256
   */
   optional uint64 max_segment_size = 4;
   /*
   Maximum size (in KiloBytes) of vectors to store in-memory per segment.
-  Segments larger than this threshold will be stored as read-only memmaped file.
+  Segments larger than this threshold will be stored as a read-only memmaped file.
   To enable memmap storage, lower the threshold
   Note: 1Kb = 1 vector of size 256
   */
   optional uint64 memmap_threshold = 5;
   /*
   Maximum size (in KiloBytes) of vectors allowed for plain index.
   Default value based on https://github.com/google-research/google-research/blob/master/scann/docs/algorithms.md
@@ -181,15 +183,15 @@
   optional uint32 shard_number = 7; // Number of shards in the collection, default = 1
   optional bool on_disk_payload = 8; // If true - point's payload will not be stored in memory
   optional uint64 timeout = 9; // Wait timeout for operation commit in seconds, if not specified - default value will be supplied
   optional VectorsConfig vectors_config = 10; // Configuration for vectors
   optional uint32 replication_factor = 11; // Number of replicas of each shard that network tries to maintain, default = 1
   optional uint32 write_consistency_factor = 12; // How many replicas should apply the operation for us to consider it successful, default = 1
   optional string init_from_collection = 13; // Specify name of the other collection to copy data from
-  optional QuantizationConfig quantization_config = 14;
+  optional QuantizationConfig quantization_config = 14; // Quantization configuration of vector
 }
 
 message UpdateCollection {
   string collection_name = 1; // Name of the collection
   optional OptimizersConfigDiff optimizers_config = 2; // New configuration parameters for the collection
   optional uint64 timeout = 3; // Wait timeout for operation commit in seconds, if not specified - default value will be supplied
   optional CollectionParamsDiff params = 4; // New configuration parameters for the collection
@@ -233,15 +235,15 @@
   Prefix = 1;
   Whitespace = 2;
   Word = 3;
 }
 
 message TextIndexParams {
   TokenizerType tokenizer = 1; // Tokenizer type
-  optional bool lowercase = 2; // If true - all tokens will be lowercased
+  optional bool lowercase = 2; // If true - all tokens will be lowercase
   optional uint64 min_token_len = 3; // Minimal token length
   optional uint64 max_token_len = 4; // Maximal token length
 }
 
 message PayloadIndexParams {
   oneof index_params {
     TextIndexParams text_index_params = 1; // Parameters for text index
```

### Comparing `qdrant_client-1.1.3/qdrant_client/proto/collections_service.proto` & `qdrant_client-1.1.4/qdrant_client/proto/collections_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/proto/json_with_int.proto` & `qdrant_client-1.1.4/qdrant_client/proto/json_with_int.proto`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 // `Struct` represents a structured data value, consisting of fields
 // which map to dynamically typed values. In some languages, `Struct`
 // might be supported by a native representation. For example, in
 // scripting languages like JS a struct is represented as an
 // object. The details of that representation are described together
 // with the proto support for the language.
 //
-// The JSON representation for `Struct` is JSON object.
+// The JSON representation for `Struct` is a JSON object.
 message Struct {
   // Unordered map of dynamically typed values.
   map<string, Value> fields = 1;
 }
 
 // `Value` represents a dynamically typed value which can be either
 // null, a number, a string, a boolean, a recursive struct value, or a
-// list of values. A producer of value is expected to set one of that
+// list of values. A producer of value is expected to set one of those
 // variants, absence of any variant indicates an error.
 //
-// The JSON representation for `Value` is JSON value.
+// The JSON representation for `Value` is a JSON value.
 message Value {
   // The kind of value.
   oneof kind {
     // Represents a null value.
     NullValue null_value = 1;
     // Represents a double value.
     double double_value = 2;
@@ -50,12 +50,12 @@
 enum NullValue {
   // Null value.
   NULL_VALUE = 0;
 }
 
 // `ListValue` is a wrapper around a repeated field of values.
 //
-// The JSON representation for `ListValue` is JSON array.
+// The JSON representation for `ListValue` is a JSON array.
 message ListValue {
   // Repeated field of dynamically typed values.
   repeated Value values = 1;
 }
```

### Comparing `qdrant_client-1.1.3/qdrant_client/proto/points.proto` & `qdrant_client-1.1.4/qdrant_client/proto/points.proto`

 * *Files 1% similar despite different names*

```diff
@@ -346,30 +346,35 @@
 
 message Condition {
   oneof condition_one_of {
     FieldCondition field = 1;
     IsEmptyCondition is_empty = 2;
     HasIdCondition has_id = 3;
     Filter filter = 4;
+    IsNullCondition is_null = 5;
   }
 }
 
 message IsEmptyCondition {
   string key = 1;
 }
 
+message IsNullCondition {
+    string key = 1;
+}
+
 message HasIdCondition {
   repeated PointId has_id = 1;
 }
 
 message FieldCondition {
   string key = 1;
   Match match = 2; // Check if point has field with a given value
   Range range = 3; // Check if points value lies in a given range
-  GeoBoundingBox geo_bounding_box = 4; // Check if points geo location lies in a given area
+  GeoBoundingBox geo_bounding_box = 4; // Check if points geolocation lies in a given area
   GeoRadius geo_radius = 5; // Check if geo point is within a given radius
   ValuesCount values_count = 6; // Check number of values for a specific field
 }
 
 message Match {
   oneof match_value {
     string keyword = 1; // Match string keyword
```

### Comparing `qdrant_client-1.1.3/qdrant_client/proto/points_service.proto` & `qdrant_client-1.1.4/qdrant_client/proto/points_service.proto`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 package qdrant;
 
 import "google/protobuf/struct.proto";
 
 service Points {
   /*
-  Perform insert + updates on points. If point with given ID already exists - it will be overwritten.
+  Perform insert + updates on points. If a point with a given ID already exists - it will be overwritten.
    */
   rpc Upsert (UpsertPoints) returns (PointsOperationResponse) {}
   /*
   Delete points
    */
   rpc Delete (DeletePoints) returns (PointsOperationResponse) {}
   /*
@@ -63,8 +63,8 @@
   Look for the points which are closer to stored positive examples and at the same time further to negative examples.
    */
   rpc RecommendBatch (RecommendBatchPoints) returns (RecommendBatchResponse) {}
   /*
    Count points in collection with given filtering conditions
    */
   rpc Count (CountPoints) returns (CountResponse) {}
-}
+}
```

### Comparing `qdrant_client-1.1.3/qdrant_client/proto/snapshots_service.proto` & `qdrant_client-1.1.4/qdrant_client/proto/snapshots_service.proto`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/qdrant_client.py` & `qdrant_client-1.1.4/qdrant_client/qdrant_client.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/qdrant_remote.py` & `qdrant_client-1.1.4/qdrant_client/qdrant_remote.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/uploader/grpc_uploader.py` & `qdrant_client-1.1.4/qdrant_client/uploader/grpc_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/uploader/rest_uploader.py` & `qdrant_client-1.1.4/qdrant_client/uploader/rest_uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/qdrant_client/uploader/uploader.py` & `qdrant_client-1.1.4/qdrant_client/uploader/uploader.py`

 * *Files identical despite different names*

### Comparing `qdrant_client-1.1.3/PKG-INFO` & `qdrant_client-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdrant-client
-Version: 1.1.3
+Version: 1.1.4
 Summary: Client library for the Qdrant vector search engine
 Home-page: https://github.com/qdrant/qdrant-client
 Keywords: vector,search,neural,matching,client
 Author: Andrey Vasnetsov
 Author-email: andrey@qdrant.tech
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.3 Summary: Client
+Metadata-Version: 2.1 Name: qdrant-client Version: 1.1.4 Summary: Client
 library for the Qdrant vector search engine Home-page: https://github.com/
 qdrant/qdrant-client Keywords: vector,search,neural,matching,client Author:
 Andrey Vasnetsov Author-email: andrey@qdrant.tech Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

