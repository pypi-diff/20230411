# Comparing `tmp/alibabacloud_fc-open20210406-2.0.6.tar.gz` & `tmp/alibabacloud_fc-open20210406-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_fc-open20210406-2.0.6.tar", last modified: Tue Mar 28 02:57:08 2023, max compression
+gzip compressed data, was "dist/alibabacloud_fc-open20210406-2.0.8.tar", last modified: Tue Apr 11 06:50:21 2023, max compression
```

## Comparing `alibabacloud_fc-open20210406-2.0.6.tar` & `alibabacloud_fc-open20210406-2.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/
--rw-r--r--   0 root         (0) root         (0)     2152 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406/__init__.py
--rw-r--r--   0 root         (0) root         (0)   352899 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406/client.py
--rw-r--r--   0 root         (0) root         (0)   600131 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      262 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2762 2023-03-28 02:57:08.000000 alibabacloud_fc-open20210406-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/
+-rw-r--r--   0 root         (0) root         (0)     2205 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   352899 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/client.py
+-rw-r--r--   0 root         (0) root         (0)   600025 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      262 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-04-11 06:50:21.000000 alibabacloud_fc-open20210406-2.0.8/setup.py
```

### Comparing `alibabacloud_fc-open20210406-2.0.6/ChangeLog.md` & `alibabacloud_fc-open20210406-2.0.8/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-03-28 Version: 2.0.6
+- Change policyItem type.
+
 2023-03-01 Version: 2.0.5
 - Support NAS with TLS.
 
 2023-02-09 Version: 2.0.4
 - Support NAS with TLS.
 
 2023-01-13 Version: 2.0.3
```

### Comparing `alibabacloud_fc-open20210406-2.0.6/LICENSE` & `alibabacloud_fc-open20210406-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406-2.0.6/PKG-INFO` & `alibabacloud_fc-open20210406-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_fc-open20210406
-Version: 2.0.6
+Version: 2.0.8
 Summary: Alibaba Cloud FC-Open (20210406) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc-open20210406-2.0.6/README-CN.md` & `alibabacloud_fc-open20210406-2.0.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406-2.0.6/README.md` & `alibabacloud_fc-open20210406-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406/client.py` & `alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406/models.py` & `alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2139,18 +2139,18 @@
             self.service_name = m.get('serviceName')
         return self
 
 
 class PolicyItem(TeaModel):
     def __init__(
         self,
-        key: bytes = None,
-        operator: bytes = None,
-        type: bytes = None,
-        value: bytes = None,
+        key: str = None,
+        operator: str = None,
+        type: str = None,
+        value: str = None,
     ):
         self.key = key
         self.operator = operator
         self.type = type
         self.value = value
 
     def validate(self):
@@ -2363,15 +2363,15 @@
                 self.routes.append(temp_model.from_map(k))
         return self
 
 
 class RoutePolicy(TeaModel):
     def __init__(
         self,
-        condition: bytes = None,
+        condition: str = None,
         policy_items: List[PolicyItem] = None,
     ):
         self.condition = condition
         self.policy_items = policy_items
 
     def validate(self):
         if self.policy_items:
@@ -3851,15 +3851,15 @@
         self.function_name = function_name
         # The GPU memory capacity for the function. Unit: MB. The value must be a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size
         # The handler of the function. The format varies based on the programming language. For more information, see [Function handlers](~~157704~~).
         self.handler = handler
         # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period expires, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout
-        # The handler of the Initializer hook. For more information, see [Initializer hook](~~157704~~).
+        # The handler of the Initializer hook. For more information, see [Initializer hooks](~~157704~~).
         self.initializer = initializer
         # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency
         # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config
         # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
         # 
@@ -3871,17 +3871,17 @@
         # *   **c1**: performance instance
         # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
         # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
         # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type
         # The information about layers.
         # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file with the same name as a layer with a larger subscript.
+        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers
-        # The memory size for the function. Unit: MB. The memory size must be a multiple of 64 MB. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
+        # The memory size for the function. Unit: MB. The value must be a multiple of 64. The memory size varies based on the function instance type. For more information, see [Instance types](~~179379~~).
         self.memory_size = memory_size
         # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime
         # The timeout period for the execution of the function. Unit: seconds. Default value: 3. Minimum value: 1. When the period ends, the execution of the function is terminated.
         self.timeout = timeout
 
     def validate(self):
@@ -4092,15 +4092,15 @@
         # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
         # *   **g1**: same as **fc.gpu.tesla.1**\
         self.instance_type = instance_type
         # The time when the function was last modified.
         self.last_modified_time = last_modified_time
         # An array that consists of the information of layers.
         # 
-        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file with the same name as a layer with a larger subscript.
+        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers
         # The memory size that is configured for the function. Unit: MB.
         self.memory_size = memory_size
         # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime
         # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
         self.timeout = timeout
@@ -8113,15 +8113,15 @@
         x_fc_account_id: str = None,
         x_fc_date: str = None,
         x_fc_trace_id: str = None,
     ):
         self.common_headers = common_headers
         # The ID of your Alibaba Cloud account.
         self.x_fc_account_id = x_fc_account_id
-        # The time when the function is invoked. The format is **EEE,d MMM yyyy HH:mm:ss GMT**.
+        # The time on which the function is invoked. The format of the value is: **EEE,d MMM yyyy HH:mm:ss GMT**.
         self.x_fc_date = x_fc_date
         # The custom request ID.
         self.x_fc_trace_id = x_fc_trace_id
 
     def validate(self):
         pass
 
@@ -8201,34 +8201,34 @@
         # The time when the service was created.
         self.created_time = created_time
         # The description of the service.
         self.description = description
         # Specifies whether to allow functions to access the Internet. Valid values:
         # 
         # *   **true**: allows functions in the specified service to access the Internet.
-        # *   **false**: does not allow functions in the specified service to access the Internet.
+        # *   **false**: does not allow functions to access the Internet.
         self.internet_access = internet_access
         # The time when the service was last modified.
         self.last_modified_time = last_modified_time
         # The log configuration, which specifies a Logstore to store function execution logs.
         self.log_config = log_config
-        # The configuration of the NAS file system. The configuration allows functions in the specified service in Function Compute to access the NAS file system.
+        # The configurations of the NAS file system. The configuration allows functions in the specified service in Function Compute to access the NAS file system.
         self.nas_config = nas_config
         # The OSS mount configurations.
         self.oss_mount_config = oss_mount_config
         # The RAM role that is used to grant required permissions to Function Compute. Scenarios:
         # 
         # *   Sends function execution logs to your Logstore.
         # *   Generates a token for a function to access other cloud resources during function execution.
         self.role = role
         # The unique ID generated by the system for the service.
         self.service_id = service_id
         # The name of the service.
         self.service_name = service_name
-        # The configurations of Tracing Analysis. After you configure Tracing Analysis for a service in Function Compute, you can record the execution duration of a request, view the amount of cold start time for a function, and record the execution duration of a function. For more information, see [Overview](~~189804~~).
+        # The configuration of Tracing Analysis. After you configure Tracing Analysis for a service in Function Compute, you can record the execution duration of a request, view the amount of cold start time for a function, and record the execution duration of a function. For more information, see [Overview](~~189804~~).
         self.tracing_config = tracing_config
         # The VPC configuration. The configuration allows a function to access the specified VPC.
         self.vpc_config = vpc_config
 
     def validate(self):
         if self.log_config:
             self.log_config.validate()
@@ -9954,15 +9954,15 @@
         self.limit = limit
         # The token required to obtain more results. If the number of resources exceeds the limit, the nextToken parameter is returned. You can include the parameter in subsequent calls to obtain more results. You do not need to provide this parameter in the first call.
         self.next_token = next_token
         # The prefix that the names of returned resources must contain.
         self.prefix = prefix
         # The version or alias of the service.
         self.qualifier = qualifier
-        # The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned.
+        # The starting position of the result list. The returned resources are sorted in alphabetical order, and the resources that include and follow the resource specified by the startKey parameter are returned.
         self.start_key = start_key
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10026,19 +10026,19 @@
         runtime: str = None,
         timeout: int = None,
     ):
         # The port on which the HTTP server listens for the custom runtime or custom container runtime.
         self.ca_port = ca_port
         # The CRC-64 value of the function code package.
         self.code_checksum = code_checksum
-        # The size of the function code package that is returned by the system. Unit: byte.
+        # The size of the function code package that is returned by the system. Unit: bytes.
         self.code_size = code_size
         # The number of vCPUs of the function. The value must be a multiple of 0.05.
         self.cpu = cpu
-        # The time when the function is created.
+        # The time when the function was created.
         self.created_time = created_time
         # The configurations of the custom container runtime.
         self.custom_container_config = custom_container_config
         # The custom health check configuration of the function. This parameter is applicable only to custom runtimes and custom containers.
         self.custom_health_check_config = custom_health_check_config
         # The description of the function.
         self.description = description
@@ -10046,43 +10046,43 @@
         self.disk_size = disk_size
         # The environment variables that you configured for the function. You can obtain the values of the environment variables from the function.
         self.environment_variables = environment_variables
         # The unique ID that is generated by the system for the function.
         self.function_id = function_id
         # The name of the function.
         self.function_name = function_name
-        # The GPU memory capacity for the function. Unit: MB. The memory capacity must be a multiple of 1024 MB.
+        # The GPU memory capacity for the function. Unit: MB. The value is a multiple of 1,024.
         self.gpu_memory_size = gpu_memory_size
         # The handler of the function.
         self.handler = handler
-        # The timeout period for the execution of the initializer function. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period ends, the execution of the initializer function is terminated.
+        # The timeout period for the execution of the Initializer hook. Unit: seconds. Default value: 3. Valid values: 1 to 300. When this period ends, the execution of the Initializer hook is terminated.
         self.initialization_timeout = initialization_timeout
-        # The handler of the initializer function. The format of the value is determined by the programming language that you use. For more information, see [Initializer function](~~157704~~).
+        # The handler of the Initializer hook. The format of the value is determined by the programming language that you use. For more information, see [Initializer hook](~~157704~~).
         self.initializer = initializer
         # The number of requests that can be concurrently processed by a single instance.
         self.instance_concurrency = instance_concurrency
         # The lifecycle configurations of the instance.
         self.instance_lifecycle_config = instance_lifecycle_config
-        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the number of the soft concurrency, the instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
+        # The soft concurrency of the instance. You can use this parameter to implement graceful scale-up of instances. If the number of concurrent requests on an instance is greater than the value of soft concurrency, an instance scale-up is triggered. For example, if your instance requires a long time to start, you can specify a suitable soft concurrency to start the instance in advance.
         # 
         # The value must be less than or equal to that of the **instanceConcurrency** parameter.
         self.instance_soft_concurrency = instance_soft_concurrency
         # The instance type of the function. Valid values:
         # 
         # *   **e1**: elastic instance
         # *   **c1**: performance instance
-        # *   **fc.gpu.tesla.1**: GPU-accelerated instances (Tesla T4)
-        # *   **fc.gpu.ampere.1**: GPU-accelerated instances (Ampere A10)
-        # *   **g1**: same fc.gpu.tesla.1
+        # *   **fc.gpu.tesla.1**: GPU-accelerated instance (Tesla T4)
+        # *   **fc.gpu.ampere.1**: GPU-accelerated instance (Ampere A10)
+        # *   **g1**: same as fc.gpu.tesla.1
         self.instance_type = instance_type
         # The time when the function was last modified.
         self.last_modified_time = last_modified_time
-        # An array that consists of the information of layers.
+        # The information about layers.
         # 
-        # > If multiple layers exist, the layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name and a larger subscript in the layer.
+        # > Multiple layers are merged based on the order of array subscripts. The content of a layer with a smaller subscript overwrites the file that has the same name as a layer with a larger subscript.
         self.layers = layers
         # The memory size that is configured for the function. Unit: MB.
         self.memory_size = memory_size
         # The runtime environment of the function. Valid values: **nodejs16**, **nodejs14**, **nodejs12**, **nodejs10**, **nodejs8**, **nodejs6**, **nodejs4.4**, **python3.9**, **python3**, **python2.7**, **java11**, **java8**, **go1**, **php7.2**, **dotnetcore3.1**, **dotnetcore2.1**, **custom** and **custom-container**. For more information, see [Supported function runtime environments](~~73338~~).
         self.runtime = runtime
         # The timeout period for the execution of the function. Unit: seconds. Default value: 60. Valid values: 1 to 600. When this period expires, the execution of the function is terminated.
         self.timeout = timeout
@@ -10215,15 +10215,15 @@
     def __init__(
         self,
         functions: List[ListFunctionsResponseBodyFunctions] = None,
         next_token: str = None,
     ):
         # The information about functions.
         self.functions = functions
-        # The token used to obtain more results. If this parameter is left empty, all the results are returned.
+        # The token used to obtain more results. If this parameter is not returned, all the layers are returned.
         self.next_token = next_token
 
     def validate(self):
         if self.functions:
             for k in self.functions:
                 if k:
                     k.validate()
@@ -15722,15 +15722,15 @@
         vpc_config: VPCConfig = None,
     ):
         # The description of the service.
         self.description = description
         # Specifies whether to allow functions to access the Internet. Valid values:
         # 
         # *   **true**: allows functions in the specified service to access the Internet.
-        # *   **false**: does not allow functions in the specified service to access the Internet.
+        # *   **false**: does not allow functions to access the Internet.
         self.internet_access = internet_access
         # The log configuration. Function Compute writes function execution logs to the specified Logstore.
         self.log_config = log_config
         # The configurations of the NAS file system. The configurations allow functions to access the specified NAS resources.
         self.nas_config = nas_config
         # The OSS mount configurations.
         self.oss_mount_config = oss_mount_config
@@ -15825,15 +15825,15 @@
         # The time when the service was created.
         self.created_time = created_time
         # The description of the service.
         self.description = description
         # Specifies whether to allow functions to access the Internet. Valid values:
         # 
         # *   **true**: allows functions in the specified service to access the Internet.
-        # *   **false**: does not allow functions in the specified service to access the Internet.
+        # *   **false**: does not allow functions to access the Internet.
         self.internet_access = internet_access
         # The time when the service was last modified.
         self.last_modified_time = last_modified_time
         # The log configuration, which specifies a Logstore to store function execution logs.
         self.log_config = log_config
         # The configurations of the NAS file system. The configuration allows functions in the specified service in Function Compute to access the NAS file system.
         self.nas_config = nas_config
@@ -15844,15 +15844,15 @@
         # *   Sends function execution logs to your Logstore.
         # *   Generates a token for a function to access other cloud resources during function execution.
         self.role = role
         # The unique ID generated by the system for the service.
         self.service_id = service_id
         # The name of the service.
         self.service_name = service_name
-        # The configurations of Tracing Analysis. After you configure Tracing Analysis for a service in Function Compute, you can record the execution duration of a request, view the amount of cold start time for a function, and record the execution duration of a function. For more information, see [Overview](~~189804~~).
+        # The configuration of Tracing Analysis. After you configure Tracing Analysis for a service in Function Compute, you can record the execution duration of a request, view the amount of cold start time for a function, and record the execution duration of a function. For more information, see [Overview](~~189804~~).
         self.tracing_config = tracing_config
         # The VPC configuration. The configuration allows a function to access the specified VPC.
         self.vpc_config = vpc_config
 
     def validate(self):
         if self.log_config:
             self.log_config.validate()
```

### Comparing `alibabacloud_fc-open20210406-2.0.6/alibabacloud_fc_open20210406.egg-info/PKG-INFO` & `alibabacloud_fc-open20210406-2.0.8/alibabacloud_fc_open20210406.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-fc-open20210406
-Version: 2.0.6
+Version: 2.0.8
 Summary: Alibaba Cloud FC-Open (20210406) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_fc-open20210406-2.0.6/setup.py` & `alibabacloud_fc-open20210406-2.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_fc-open20210406.
 
-Created on 28/03/2023
+Created on 11/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_fc_open20210406"
 NAME = "alibabacloud_fc-open20210406" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud FC-Open (20210406) SDK Library for Python"
@@ -39,15 +39,15 @@
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.8, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0",
     "alibabacloud_credentials>=0.3.1, <1.0.0",
     "requests>=2.21.0, <3.0.0",
-    "alibabacloud_gateway_fc_util>=0.0.3, <1.0.0"
+    "alibabacloud_gateway_fc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

