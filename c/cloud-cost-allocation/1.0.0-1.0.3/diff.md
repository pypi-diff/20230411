# Comparing `tmp/cloud-cost-allocation-1.0.0.tar.gz` & `tmp/cloud-cost-allocation-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-cost-allocation-1.0.0.tar", last modified: Tue Mar 14 17:30:47 2023, max compression
+gzip compressed data, was "cloud-cost-allocation-1.0.3.tar", last modified: Tue Apr 11 07:31:03 2023, max compression
```

## Comparing `cloud-cost-allocation-1.0.0.tar` & `cloud-cost-allocation-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:47.760381 cloud-cost-allocation-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1078 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       57 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    20967 2023-03-14 17:30:47.760381 cloud-cost-allocation-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    19754 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:47.756381 cloud-cost-allocation-1.0.0/cloud_cost_allocation/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    23784 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/cloud_cost_allocator.py
--rw-r--r--   0 runner    (1001) docker     (116)    10177 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/config.py
--rw-r--r--   0 runner    (1001) docker     (116)    40093 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/cost_items.py
--rw-r--r--   0 runner    (1001) docker     (116)      394 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3248 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:47.756381 cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4399 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)     1659 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/base_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)     5564 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
--rw-r--r--   0 runner    (1001) docker     (116)    10325 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:47.760381 cloud-cost-allocation-1.0.0/cloud_cost_allocation/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1191 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:47.760381 cloud-cost-allocation-1.0.0/cloud_cost_allocation/writer/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/writer/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (116)     6668 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:47.756381 cloud-cost-allocation-1.0.0/cloud_cost_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    20967 2023-03-14 17:30:47.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1219 2023-03-14 17:30:47.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-14 17:30:47.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       22 2023-03-14 17:30:47.000000 cloud-cost-allocation-1.0.0/cloud_cost_allocation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:47.760381 cloud-cost-allocation-1.0.0/puml/
--rw-r--r--   0 runner    (1001) docker     (116)      968 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/puml/cost-allocation-model.puml
--rw-r--r--   0 runner    (1001) docker     (116)    23813 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/puml/cost-allocation-model.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/puml/hierarchical-service-consumption-example.puml
--rw-r--r--   0 runner    (1001) docker     (116)    16917 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/puml/hierarchical-service-consumption-example.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1160 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/puml/hierarchical-service-cost-allocation-example.puml
--rw-r--r--   0 runner    (1001) docker     (116)    15996 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/puml/hierarchical-service-cost-allocation-example.svg
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2023-03-14 17:30:47.760381 cloud-cost-allocation-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1446 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-14 17:30:47.760381 cloud-cost-allocation-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     5812 2023-03-14 17:30:31.000000 cloud-cost-allocation-1.0.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19754 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23784 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/cloud_cost_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40095 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/cost_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/base_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/csv_allocated_cost_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/csv_allocated_cost_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20967 2023-04-11 07:31:02.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 07:31:03.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 07:31:02.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-11 07:31:02.000000 cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/puml/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/cost-allocation-model.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    23813 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/cost-allocation-model.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/hierarchical-service-consumption-example.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/hierarchical-service-consumption-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/hierarchical-service-cost-allocation-example.puml
+-rw-r--r--   0 runner    (1001) docker     (123)    15996 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/puml/hierarchical-service-cost-allocation-example.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-04-11 07:31:03.013227 cloud-cost-allocation-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 07:31:03.009227 cloud-cost-allocation-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-11 07:30:45.000000 cloud-cost-allocation-1.0.3/tests/test.py
```

### Comparing `cloud-cost-allocation-1.0.0/LICENSE` & `cloud-cost-allocation-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/PKG-INFO` & `cloud-cost-allocation-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.0
+Version: 1.0.3
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
```

### Comparing `cloud-cost-allocation-1.0.0/README.md` & `cloud-cost-allocation-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/cloud_cost_allocator.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/cloud_cost_allocator.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/config.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/config.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/cost_items.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/cost_items.py`

 * *Files 0% similar despite different names*

```diff
@@ -838,15 +838,15 @@
     def __init__(self, config: Config):
 
         # Config and factory
         self.config = config
 
     def create_cloud_cost_item(self) -> CloudCostItem:
         cloud_cost_item = CloudCostItem()
-        CloudCostItem.initialize(self.config)
+        cloud_cost_item.initialize(self.config)
         return cloud_cost_item
 
     def create_consumer_cost_item(self) -> ConsumerCostItem:
         consumer_cost_item = ConsumerCostItem()
         consumer_cost_item.initialize(self.config)
         return consumer_cost_item
```

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/main.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,18 +72,23 @@
     cost_allocation_reader = CSV_CostAllocationKeysReader(cost_item_factory)
     for key in options.keys:
         info("Reading cost allocation keys: " + key)
         read_csv(key, cost_allocation_reader, consumer_cost_items)
 
     # Allocate costs
     cloud_cost_allocator = CloudCostAllocator(cost_item_factory)
+    cloud_cost_allocator.currency = cloud_cost_items[0].currency
+    cloud_cost_allocator.date_str = cloud_cost_items[0].date_str
+    info("Allocating costs with currency " + cloud_cost_allocator.currency +
+         " for date " + cloud_cost_allocator.date_str)
     if not cloud_cost_allocator.allocate(consumer_cost_items, cloud_cost_items):
         error("Cost allocation failed")
         exit(3)
 
     # Write allocated costs
+    info("Writing allocated costs: " + options.output)
     allocated_cost_writer = CSV_AllocatedCostWriter(cloud_cost_allocator.service_instances, config)
     write_csv_file(options.output, allocated_cost_writer)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/azure_ea_amortized_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/base_reader.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/base_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/csv_allocated_cost_reader.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/csv_allocated_cost_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/reader/csv_cost_allocation_keys_reader.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/utils/utils.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/writer/base_writer.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/base_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 '''
 Created on 21.04.2022
 
 @author: marc.diensberg
 '''
 from abc import ABC, abstractmethod
-from configparser import ConfigParser
 from logging import error
 
-from cloud_cost_allocation.cost_items import ServiceInstance, ConsumerCostItem, CloudCostItem, CostItem
+from cloud_cost_allocation.cost_items import Config, ServiceInstance, ConsumerCostItem, CloudCostItem, CostItem
 
 
 class GenericWriter(ABC):
     '''
     classdocs
     '''
 
     __slots__ = (
-        'config',               # type: ConfigParser
+        'config',               # type: Config
         'service_instances',    # type: ServiceInstance
         'exporters',            # type: dict[type -> method]
     )
 
-    def __init__(self, service_instances: list[ServiceInstance], config: ConfigParser):
+    def __init__(self, service_instances: list[ServiceInstance], config: Config):
         '''
         Constructor
         '''
         self.service_instances = service_instances
         self.config = config
         self.exporters = {}
         self.exporters[CostItem] = self.export_item_base
```

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation/writer/csv_allocated_cost_writer.py` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation/writer/csv_allocated_cost_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 '''
 Created on 21.04.2022
 
 @author: marc.diensberg
 '''
 from io import StringIO
-from configparser import ConfigParser
 
-from cloud_cost_allocation.cost_items import ServiceInstance
+from cloud_cost_allocation.cost_items import Config, ServiceInstance
 from cloud_cost_allocation.writer.base_writer import GenericWriter
 
 
 class CSV_AllocatedCostWriter(GenericWriter):
     '''
     classdocs
     '''
 
-    def __init__(self, service_instances: list[ServiceInstance], config: ConfigParser):
+    def __init__(self, service_instances: list[ServiceInstance], config: Config):
         super().__init__(service_instances, config)
 
     def get_headers(self) -> list[str]:
 
         # Column order is historical
 
         # Initialize
```

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation.egg-info/PKG-INFO` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-cost-allocation
-Version: 1.0.0
+Version: 1.0.3
 Summary: Python library for shared, hierarchical cost allocation based on user-defined usage metrics.
 Home-page: https://github.com/AmadeusITGroup/cloud-cost-allocation
 Author: Marc Perreaut
 Author-email: marc.perreaut@amadeus.com
 Maintainer: Amadeus IT Group
 Maintainer-email: opensource@amadeus.com
 License: MIT license
```

### Comparing `cloud-cost-allocation-1.0.0/cloud_cost_allocation.egg-info/SOURCES.txt` & `cloud-cost-allocation-1.0.3/cloud_cost_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/puml/cost-allocation-model.puml` & `cloud-cost-allocation-1.0.3/puml/cost-allocation-model.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/puml/cost-allocation-model.svg` & `cloud-cost-allocation-1.0.3/puml/cost-allocation-model.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/puml/hierarchical-service-consumption-example.puml` & `cloud-cost-allocation-1.0.3/puml/hierarchical-service-consumption-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/puml/hierarchical-service-consumption-example.svg` & `cloud-cost-allocation-1.0.3/puml/hierarchical-service-consumption-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/puml/hierarchical-service-cost-allocation-example.puml` & `cloud-cost-allocation-1.0.3/puml/hierarchical-service-cost-allocation-example.puml`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/puml/hierarchical-service-cost-allocation-example.svg` & `cloud-cost-allocation-1.0.3/puml/hierarchical-service-cost-allocation-example.svg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/setup.cfg` & `cloud-cost-allocation-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloud-cost-allocation-1.0.0/setup.py` & `cloud-cost-allocation-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Import readme
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme_file:
     readme = readme_file.read()
 
 # Setup
 setup(
     name='cloud-cost-allocation',
-    version='1.0.0',
+    version='1.0.3',
     description='Python library for shared, hierarchical cost allocation based on user-defined usage metrics.',
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=['cloud_cost_allocation',
               'cloud_cost_allocation.reader',
               'cloud_cost_allocation.utils',
               'cloud_cost_allocation.writer'],
```

### Comparing `cloud-cost-allocation-1.0.0/tests/test.py` & `cloud-cost-allocation-1.0.3/tests/test.py`

 * *Files identical despite different names*

