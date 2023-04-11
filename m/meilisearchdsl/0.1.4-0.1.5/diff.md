# Comparing `tmp/meilisearchdsl-0.1.4.tar.gz` & `tmp/meilisearchdsl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearchdsl-0.1.4.tar", last modified: Fri Mar 31 18:36:57 2023, max compression
+gzip compressed data, was "meilisearchdsl-0.1.5.tar", last modified: Tue Apr 11 16:15:17 2023, max compression
```

## Comparing `meilisearchdsl-0.1.4.tar` & `meilisearchdsl-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:36:57.466149 meilisearchdsl-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-31 18:36:42.000000 meilisearchdsl-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-31 18:36:57.466149 meilisearchdsl-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-03-31 18:36:42.000000 meilisearchdsl-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:36:57.466149 meilisearchdsl-0.1.4/meilisearchdsl/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-31 18:36:42.000000 meilisearchdsl-0.1.4/meilisearchdsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-03-31 18:36:42.000000 meilisearchdsl-0.1.4/meilisearchdsl/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21570 2023-03-31 18:36:42.000000 meilisearchdsl-0.1.4/meilisearchdsl/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-03-31 18:36:42.000000 meilisearchdsl-0.1.4/meilisearchdsl/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-03-31 18:36:42.000000 meilisearchdsl-0.1.4/meilisearchdsl/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:36:57.466149 meilisearchdsl-0.1.4/meilisearchdsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-03-31 18:36:57.000000 meilisearchdsl-0.1.4/meilisearchdsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-31 18:36:57.000000 meilisearchdsl-0.1.4/meilisearchdsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 18:36:57.000000 meilisearchdsl-0.1.4/meilisearchdsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-31 18:36:57.000000 meilisearchdsl-0.1.4/meilisearchdsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-31 18:36:57.000000 meilisearchdsl-0.1.4/meilisearchdsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 18:36:57.466149 meilisearchdsl-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-03-31 18:36:49.000000 meilisearchdsl-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/meilisearchdsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22432 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-11 16:15:08.000000 meilisearchdsl-0.1.5/setup.py
```

### Comparing `meilisearchdsl-0.1.4/LICENSE` & `meilisearchdsl-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.4/PKG-INFO` & `meilisearchdsl-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearchdsl
-Version: 0.1.4
+Version: 0.1.5
 Summary: MeiliSearch DSL is a Python package providing a Django-like Q object syntax for querying MeiliSearch, an open-source search engine. It simplifies search query building and offers a convenient wrapper for MeiliSearch indexes and clients, streamlining search interactions and improving maintainability.
 Home-page: https://github.com/UnattendedFlight/meilisearch-dsl
 Author: Adrian Leo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `meilisearchdsl-0.1.4/README.md` & `meilisearchdsl-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.4/meilisearchdsl/client.py` & `meilisearchdsl-0.1.5/meilisearchdsl/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
             assert self.config is not None, "MeiliClient config not set"
             assert "host" in self.config, "MeiliClient config missing host"
             assert "master_key" in self.config, "MeiliClient config missing master_key"
             self.client = Client(
                 self.config["host"], self.config["master_key"])
         return self.client
 
-    def get_index(self, index_name: str) -> MeiliIndex:
+    def get_index(self, index_name: str, primary_key: str) -> MeiliIndex:
         """Get an index by name. If it doesn't exist, create it."""
         self.client = self.get_client()
         assert self.client is not None, ModuleNotFoundError(
             "No Meilisearch client")
 
         if index_name not in self.indexes:
-            self.indexes[index_name] = MeiliIndex(index_name, self.client)
+            self.indexes[index_name] = MeiliIndex(index_name, self.client, primary_key)
         return self.indexes[index_name]
 
     def delete_index(self, index_name: str):
         """Delete an index by name."""
         self.client = self.get_client()
         assert self.client is not None, ModuleNotFoundError(
             "No Meilisearch client")
```

### Comparing `meilisearchdsl-0.1.4/meilisearchdsl/index.py` & `meilisearchdsl-0.1.5/meilisearchdsl/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,30 +10,33 @@
 
 from .query import Q
 
 
 class MeiliIndex:
     """MeiliIndex class."""
 
-    def __init__(self, index_name: str, client: meilisearch.Client):
+    def __init__(self, index_name: str, client: meilisearch.Client, primary_key: str):
         self.index_name = index_name
         self.client: meilisearch.Client = client
-        self._index: Index = self.get_index(index_name)
+        try:
+            self._index: Index = self.get_index(index_name, primary_key)
+        except Exception:
+            self._index: Index = self.create_index(index_name, primary_key)
 
     def get_index(
         self,
         index_name: str,
         primary_key: Optional[str] = None,
         options: Union[Dict[str, Any], None] = None,
     ) -> Index:
         """Get an index from Meilisearch."""
         assert self.client is not None, "No Meilisearch client"
         try:
             self._index = self.client.get_index(index_name)
-        except MeiliSearchApiError:
+        except Exception:
             index_options = {}
             if options is not None:
                 assert isinstance(
                     options, dict), "Options must be a dictionary"
             if primary_key is not None:
                 index_options["primaryKey"] = primary_key
             if options is not None:
@@ -41,14 +44,37 @@
 
             self._call_long_index_method(
                 self.client.create_index, index_name, index_options
             )
 
             self._index = self.client.get_index(index_name)
         return self._index
+    
+    def create_index(
+        self,
+        index_name: str,
+        primary_key: Optional[str] = None,
+        options: Union[Dict[str, Any], None] = None,
+    ) -> Index:
+        """Create an index in Meilisearch."""
+        assert self.client is not None, "No Meilisearch client"
+        index_options = {}
+        if options is not None:
+            assert isinstance(options, dict), "Options must be a dictionary"
+        if primary_key is not None:
+            index_options["primaryKey"] = primary_key
+        if options is not None:
+            index_options.update(options)
+
+        self._call_long_index_method(
+            self.client.create_index, index_name, index_options
+        )
+
+        self._index = self.client.get_index(index_name)
+        return self._index
 
     def update_filterable_attributes(self, attributes: List[str]) -> Union[TaskInfo, Task]:
         """Update filterable attributes of the index.
 
         Parameters
         ----------
         body:
@@ -596,10 +622,9 @@
                 )
             sleep(0.5)
             count += 0.5
         return None
 
     def _call_long_index_method(self, function, *args, **kwargs) -> Any:
         """Call a method that returns a taskInfo object and wait for the task to complete."""
-        assert self._index is not None, "No Meilisearch index"
         task_info: TaskInfo = function(*args, **kwargs)
         return self._await_running_task(task_info)
```

### Comparing `meilisearchdsl-0.1.4/meilisearchdsl/query.py` & `meilisearchdsl-0.1.5/meilisearchdsl/query.py`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.4/meilisearchdsl/test.py` & `meilisearchdsl-0.1.5/meilisearchdsl/test.py`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.4/meilisearchdsl.egg-info/PKG-INFO` & `meilisearchdsl-0.1.5/meilisearchdsl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearchdsl
-Version: 0.1.4
+Version: 0.1.5
 Summary: MeiliSearch DSL is a Python package providing a Django-like Q object syntax for querying MeiliSearch, an open-source search engine. It simplifies search query building and offers a convenient wrapper for MeiliSearch indexes and clients, streamlining search interactions and improving maintainability.
 Home-page: https://github.com/UnattendedFlight/meilisearch-dsl
 Author: Adrian Leo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `meilisearchdsl-0.1.4/setup.py` & `meilisearchdsl-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=missing-docstring, invalid-name, line-too-long, R1732
 from setuptools import setup, find_packages
 
 setup(
     name="meilisearchdsl",
-    version="0.1.4",
+    version="0.1.5",
     description="MeiliSearch DSL is a Python package providing a Django-like Q object syntax for"
     + " querying MeiliSearch, an open-source search engine."
     + " It simplifies search query building and offers a convenient wrapper"
     + " for MeiliSearch indexes and clients, streamlining search interactions"
     + " and improving maintainability.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
```

