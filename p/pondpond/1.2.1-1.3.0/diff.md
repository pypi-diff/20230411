# Comparing `tmp/pondpond-1.2.1.tar.gz` & `tmp/pondpond-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pondpond-1.2.1.tar", last modified: Tue Nov 22 07:44:14 2022, max compression
+gzip compressed data, was "pondpond-1.3.0.tar", last modified: Tue Apr 11 09:39:29 2023, max compression
```

## Comparing `pondpond-1.2.1.tar` & `pondpond-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0 andy       (501) staff       (20)    11358 2022-08-06 06:58:54.027681 pondpond-1.2.1/LICENSE
--rw-r--r--   0 andy       (501) staff       (20)     5793 2022-11-09 06:03:02.378902 pondpond-1.2.1/README.md
--rw-r--r--   0 andy       (501) staff       (20)      750 2022-11-08 09:31:43.378365 pondpond-1.2.1/pond/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     4929 2022-11-08 06:26:59.900339 pondpond-1.2.1/pond/count_min_sketch.py
--rw-r--r--   0 andy       (501) staff       (20)    14720 2022-11-22 07:35:31.357099 pondpond-1.2.1/pond/pond_class.py
--rw-r--r--   0 andy       (501) staff       (20)     1116 2022-11-08 07:16:32.733609 pondpond-1.2.1/pond/pooled_object.py
--rw-r--r--   0 andy       (501) staff       (20)     1309 2022-11-08 06:30:28.188665 pondpond-1.2.1/pond/pooled_object_factory.py
--rw-r--r--   0 andy       (501) staff       (20)        0 2022-10-18 06:53:42.469389 pondpond-1.2.1/pond/py.typed
--rw-r--r--   0 andy       (501) staff       (20)        0 2022-11-22 07:43:18.709303 pondpond-1.2.1/pond-stubs/__init__.pyi
--rw-r--r--   0 andy       (501) staff       (20)      395 2022-11-22 07:43:18.709584 pondpond-1.2.1/pond-stubs/count_min_sketch.pyi
--rw-r--r--   0 andy       (501) staff       (20)     2070 2022-11-22 07:43:18.709461 pondpond-1.2.1/pond-stubs/pond_class.pyi
--rw-r--r--   0 andy       (501) staff       (20)      247 2022-11-22 07:43:18.709773 pondpond-1.2.1/pond-stubs/pooled_object.pyi
--rw-r--r--   0 andy       (501) staff       (20)      678 2022-11-22 07:43:18.709684 pondpond-1.2.1/pond-stubs/pooled_object_factory.pyi
--rw-r--r--   0 andy       (501) staff       (20)     1201 2022-11-22 07:37:07.062761 pondpond-1.2.1/pyproject.toml
--rw-r--r--   0 andy       (501) staff       (20)       37 2022-08-02 09:08:23.046400 pondpond-1.2.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0 andy       (501) staff       (20)      191 2022-08-02 09:08:23.046470 pondpond-1.2.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 andy       (501) staff       (20)      302 2022-08-02 09:08:23.046298 pondpond-1.2.1/tests/.pytest_cache/README.md
--rw-r--r--   0 andy       (501) staff       (20)        2 2022-08-02 09:08:23.046548 pondpond-1.2.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 andy       (501) staff       (20)        2 2022-08-02 09:08:23.046645 pondpond-1.2.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 andy       (501) staff       (20)        0 2022-08-02 08:15:47.024533 pondpond-1.2.1/tests/__init__.py
--rw-r--r--   0 andy       (501) staff       (20)     1406 2022-11-08 09:46:48.635768 pondpond-1.2.1/tests/test_aysnc_pond.py
--rw-r--r--   0 andy       (501) staff       (20)     4925 2022-11-22 07:33:32.430732 pondpond-1.2.1/tests/test_pond.py
--rw-------   0 andy       (501) staff       (20)     6182 2022-11-22 07:44:14.640416 pondpond-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-08-06 06:58:54.027681 pondpond-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5793 2022-11-09 06:03:02.378902 pondpond-1.3.0/README.md
+-rw-r--r--   0        0        0      750 2023-03-28 02:08:30.764284 pondpond-1.3.0/pond/__init__.py
+-rw-r--r--   0        0        0     3213 2023-04-11 08:25:05.994200 pondpond-1.3.0/pond/count_min_sketch.py
+-rw-r--r--   0        0        0    14526 2023-04-11 09:25:51.262228 pondpond-1.3.0/pond/pond_class.py
+-rw-r--r--   0        0        0     1116 2022-11-08 07:16:32.733609 pondpond-1.3.0/pond/pooled_object.py
+-rw-r--r--   0        0        0     1309 2022-11-08 06:30:28.188665 pondpond-1.3.0/pond/pooled_object_factory.py
+-rw-r--r--   0        0        0        0 2022-10-18 06:53:42.469389 pondpond-1.3.0/pond/py.typed
+-rw-r--r--   0        0        0        0 2023-04-11 09:24:33.812741 pondpond-1.3.0/pond-stubs/__init__.pyi
+-rw-r--r--   0        0        0      402 2023-04-11 09:24:33.813127 pondpond-1.3.0/pond-stubs/count_min_sketch.pyi
+-rw-r--r--   0        0        0     2070 2023-04-11 09:24:33.812960 pondpond-1.3.0/pond-stubs/pond_class.pyi
+-rw-r--r--   0        0        0      247 2023-04-11 09:24:33.813478 pondpond-1.3.0/pond-stubs/pooled_object.pyi
+-rw-r--r--   0        0        0      678 2023-04-11 09:24:33.813326 pondpond-1.3.0/pond-stubs/pooled_object_factory.pyi
+-rw-r--r--   0        0        0     1223 2023-04-11 08:27:17.371984 pondpond-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2022-08-02 09:08:23.046400 pondpond-1.3.0/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-08-02 09:08:23.046470 pondpond-1.3.0/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-08-02 09:08:23.046298 pondpond-1.3.0/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2022-08-02 09:08:23.046548 pondpond-1.3.0/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-08-02 09:08:23.046645 pondpond-1.3.0/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-08-02 08:15:47.024533 pondpond-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1033 2023-04-11 07:34:01.539120 pondpond-1.3.0/tests/draw.py
+-rw-r--r--   0        0        0     1374 2023-04-11 06:56:38.551526 pondpond-1.3.0/tests/test_aysnc_pond.py
+-rw-r--r--   0        0        0     1168 2023-04-11 08:37:53.522729 pondpond-1.3.0/tests/test_cprofile.py
+-rw-r--r--   0        0        0     4926 2023-04-11 09:20:34.424503 pondpond-1.3.0/tests/test_pond.py
+-rw-r--r--   0        0        0     6182 1970-01-01 00:00:00.000000 pondpond-1.3.0/PKG-INFO
```

### Comparing `pondpond-1.2.1/LICENSE` & `pondpond-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pondpond-1.2.1/README.md` & `pondpond-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pondpond-1.2.1/pond/__init__.py` & `pondpond-1.3.0/pond/__init__.py`

 * *Files identical despite different names*

### Comparing `pondpond-1.2.1/pond/pond_class.py` & `pondpond-1.3.0/pond/pond_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import asyncio
 import math
 import time
 from asyncio import AbstractEventLoop
-from queue import Queue
+from collections import deque
 from threading import Thread
-from typing import TYPE_CHECKING, Any, Coroutine, Dict, Final, Optional
+from typing import TYPE_CHECKING, Any, Coroutine, Deque, Dict, Final, Optional
 
 from .count_min_sketch import CountMinSketch
 from .pooled_object import PooledObject
 from .pooled_object_factory import PooledObjectFactory
 
 
 class Pond(object):
@@ -38,49 +38,50 @@
             a smaller memory usage and a higher hit rate.For more details,
             see our user's guide or my blog(https://qin.news).
 
         Args:
             borrowed_timeout (int, optional): The maximum duration of the
                 borrowed object. Defaults to 60.
             time_between_eviction_runs (int, optional): The interval for
-                automatic recycling. Defaults to 300.
+                automatic recycling. Defaults to 300. If its value is -1,
+                the recycling is turned off.
             eviction_weight (float, optional): Automatic recycling weight.
                 Defaults to 0.8.
             thread_daemon (bool, optional): A boolean value indicating whether
                 the pond's thread is a daemon thread. Defaults to True.
         """
         self.__borrowed_timeout: int = borrowed_timeout
         if loop is not None:
             self.__loop = loop
         else:
             self.__loop = asyncio.new_event_loop()
         self.__time_between_eviction_runs = time_between_eviction_runs
         self.__eviction_weight = eviction_weight
         self.__async_lock = asyncio.Lock()
         self.__class_dict: Final[Dict[str, PooledObjectFactory]] = dict()
-        # In Python 3.8 and earlier, there are several examples within the standard library,
-        # for instance, os.PathLike and queue.Queue.
+
         if TYPE_CHECKING:
-            self.__pooled_object_tree: Final[Dict[str, Queue[PooledObject]]] = dict()
+            self.__pooled_object_tree: Final[Dict[str, Deque[PooledObject]]] = dict()
         else:
-            self.__pooled_object_tree: Final[Dict[str, Queue]] = dict()
+            self.__pooled_object_tree: Final[Dict[str, Deque]] = dict()
         self.counter: CountMinSketch = CountMinSketch(28, 3)
 
         def loop_runner(
             loop: AbstractEventLoop, function: Coroutine[Any, Any, None]
         ) -> None:
             asyncio.set_event_loop(loop)
             loop.create_task(function)
             loop.run_forever()
 
-        self.__thread = Thread(
-            target=loop_runner, args=(self.__loop, self.__eviction())
-        )
-        self.__thread.daemon = thread_daemon
-        self.__thread.start()
+        if self.__time_between_eviction_runs > -1:
+            self.__thread = Thread(
+                target=loop_runner, args=(self.__loop, self.__eviction())
+            )
+            self.__thread.daemon = thread_daemon
+            self.__thread.start()
 
     def register(
         self, factory: Optional[PooledObjectFactory] = None, name: Optional[str] = None
     ) -> None:
         """Registering the factory object with Pond will use the class name of
             the factory as the key for the PooledObjectTree by default.After
             successful registration, Pond will automatically start creating
@@ -100,20 +101,20 @@
         if name is None:
             assert factory is not None
             name = factory.factory_name()
         assert factory is not None
         if self.__pooled_object_tree.__contains__(name):
             raise ValueError("The factoryClass existed in the PooledObjectTree!")
         self.__class_dict[name] = factory
-        self.__pooled_object_tree[name] = Queue(maxsize=factory.pooled_maxsize)
+        self.__pooled_object_tree[name] = deque(maxlen=factory.pooled_maxsize)
         for i in range(factory.pooled_maxsize):
             instance = self.__class_dict[name].creatInstantce()
             if instance is None:
                 raise ValueError("The instance must not be null!")
-            self.__pooled_object_tree[name].put(instance)
+            self.__pooled_object_tree[name].appendleft(instance)
 
     def borrow(
         self, factory: Optional[PooledObjectFactory] = None, name: Optional[str] = None
     ) -> PooledObject:
         """You can use factory object or factory name to borrow and return
             objects from the object pool.
 
@@ -126,24 +127,26 @@
         Returns:
             PooledObject: The pooled object you want to borrow.
         """
         if not name:
             assert factory is not None
             name = factory.factory_name()
         if self.is_empty(name=name):
-            self.counter.add(name)
+            if self.__time_between_eviction_runs > -1:
+                self.counter.add(name)
             return self.__class_dict[name].creatInstantce()
-        pooled_object = self.__pooled_object_tree[name].get()
+        pooled_object = self.__pooled_object_tree[name].pop()
         while not self.__class_dict[name].validate(pooled_object):
             self.__clear_one_object(pooled_object, name=name)
             if self.is_empty(name=name):
                 pooled_object = self.__class_dict[name].creatInstantce()
             else:
-                pooled_object = self.__pooled_object_tree[name].get()
-        self.counter.add(name)
+                pooled_object = self.__pooled_object_tree[name].pop()
+        if self.__time_between_eviction_runs > -1:
+            self.counter.add(name)
         return pooled_object.update_brrow_time()
 
     def recycle(
         self,
         pooled_object: PooledObject,
         factory: Optional[PooledObjectFactory] = None,
         name: Optional[str] = None,
@@ -165,15 +168,15 @@
         if self.is_full(name=name):
             self.__clear_one_object(pooled_object, name=name)
             return
         if (time.time() - pooled_object.last_borrow_time) > self.__borrowed_timeout:
             self.__clear_one_object(pooled_object, name=name)
             return
 
-        self.__pooled_object_tree[name].put(
+        self.__pooled_object_tree[name].appendleft(
             self.__class_dict[name].reset(pooled_object)
         )
 
     def clear(
         self, factory: Optional[PooledObjectFactory] = None, name: Optional[str] = None
     ) -> None:
         """You can use factory object or factory name to clear the object pool.
@@ -184,15 +187,15 @@
             name (Optional[str], optional): The factory name you want to register.
                 Defaults to None.
         """
         if not name:
             assert factory is not None
             name = factory.factory_name()
         while not self.is_empty(name=name):
-            pooled_object = self.__pooled_object_tree[name].get()
+            pooled_object = self.__pooled_object_tree[name].pop()
             self.__clear_one_object(pooled_object, name=name)
 
     def __clear_one_object(
         self,
         pooled_object: PooledObject,
         factory: Optional[PooledObjectFactory] = None,
         name: Optional[str] = None,
@@ -207,15 +210,15 @@
         """Query how many object pools there are in pooled_object_tree."""
         return len(self.__pooled_object_tree)
 
     def count_total_objects(self) -> int:
         """Query how many objects there are in pooled_object_tree."""
         total_number = 0
         for k, v in self.__pooled_object_tree.items():
-            total_number = total_number + v.qsize()
+            total_number = total_number + len(v)
         return total_number
 
     def contains(
         self, factory: Optional[PooledObjectFactory] = None, name: Optional[str] = None
     ) -> bool:
         """Return true if the specified factory has been registered in the pond.
 
@@ -242,15 +245,15 @@
 
         Returns:
             int: Size of the specified object pool.
         """
         if not name:
             assert factory is not None
             name = factory.factory_name()
-        return self.__pooled_object_tree[name].qsize()
+        return len(self.__pooled_object_tree[name])
 
     def is_full(
         self, factory: Optional[PooledObjectFactory] = None, name: Optional[str] = None
     ) -> bool:
         """Check to see if the supplied object pool is filled.
 
         Args:
@@ -259,15 +262,17 @@
 
         Returns:
             bool: Whether the object pool is full.
         """
         if not name:
             assert factory is not None
             name = factory.factory_name()
-        return self.__pooled_object_tree[name].full()
+        return len(self.__pooled_object_tree[name]) >= (
+            self.__pooled_object_tree[name].maxlen or 0
+        )
 
     def is_empty(
         self, factory: Optional[PooledObjectFactory] = None, name: Optional[str] = None
     ) -> bool:
         """Check to see if the supplied object pool is emptied.
 
         Args:
@@ -276,15 +281,15 @@
 
         Returns:
             bool: Whether the object pool is empty.
         """
         if not name:
             assert factory is not None
             name = factory.factory_name()
-        return self.__pooled_object_tree[name].empty()
+        return len(self.__pooled_object_tree[name]) == 0
 
     def __reset_counter(self) -> None:
         n = self.size()
         if n == 0:
             epsilon = 0.1
         else:
             epsilon = 10 / n
@@ -306,35 +311,28 @@
         first_run = True
         while self.__time_between_eviction_runs > 0:
             if first_run:
                 first_run = False
                 await asyncio.sleep(self.__time_between_eviction_runs)
                 continue
             pooled_object_borrow_count: Dict[str, int] = {}
-            max_count = 0
-            for key in self.__pooled_object_tree.keys():
-                pooled_object_borrow_count[key] = self.counter[key]
-                if max_count <= pooled_object_borrow_count[key]:
-                    max_count = pooled_object_borrow_count[key]
+            max_count = 8
             boundary = int(max_count * self.__eviction_weight)
             for key, value in pooled_object_borrow_count.items():
-                size = self.__pooled_object_tree[key].qsize()
-                try:
-                    if value < boundary and size > 0:
-                        if size > 1:
-                            for i in range(int(size / 2)):
-                                self.__clear_one_object(
-                                    self.__pooled_object_tree[key].get(),
-                                    name=key,
-                                )
-                        else:
-                            if not self.__class_dict[key].least_one:
-                                self.clear(name=key)
-                except asyncio.QueueEmpty:
-                    continue
+                size = len(self.__pooled_object_tree[key])
+                if value < boundary and size > 0:
+                    if size > 1:
+                        for i in range(int(size / 2)):
+                            self.__clear_one_object(
+                                self.__pooled_object_tree[key].pop(),
+                                name=key,
+                            )
+                    else:
+                        if not self.__class_dict[key].least_one:
+                            self.clear(name=key)
             self.__reset_counter()
             if debug:
                 self.__time_between_eviction_runs = -1
             await asyncio.sleep(self.__time_between_eviction_runs)
 
     async def async_register(
         self, factory: Optional[PooledObjectFactory] = None, name: Optional[str] = None
```

### Comparing `pondpond-1.2.1/pond/pooled_object.py` & `pondpond-1.3.0/pond/pooled_object.py`

 * *Files identical despite different names*

### Comparing `pondpond-1.2.1/pond/pooled_object_factory.py` & `pondpond-1.3.0/pond/pooled_object_factory.py`

 * *Files identical despite different names*

### Comparing `pondpond-1.2.1/pond-stubs/pond_class.pyi` & `pondpond-1.3.0/pond-stubs/pond_class.pyi`

 * *Files identical despite different names*

### Comparing `pondpond-1.2.1/pond-stubs/pooled_object_factory.pyi` & `pondpond-1.3.0/pond-stubs/pooled_object_factory.pyi`

 * *Files identical despite different names*

### Comparing `pondpond-1.2.1/pyproject.toml` & `pondpond-1.3.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -4,20 +4,22 @@
     "pdm-pep517>=1.0.0",
 ]
 
 [project]
 authors = [
     { name = "Andy Qin", email = "dr.qin@protonmail.com" },
 ]
-dependencies = []
+dependencies = [
+    "madoka>=0.7.1",
+]
 description = "Pond is a high performance object-pooling library for Python."
 name = "pondpond"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "1.2.1"
+version = "1.3.0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Blog = "https://qin.news"
 "Bug Tracker" = "https://github.com/t-baby/pond/issues"
```

### Comparing `pondpond-1.2.1/tests/test_aysnc_pond.py` & `pondpond-1.3.0/tests/test_aysnc_pond.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 import time
-from distutils.log import debug
 
 import pytest
 
 from pond import Pond, PooledObject, PooledObjectFactory
 
 
 class Dog:
```

### Comparing `pondpond-1.2.1/tests/test_pond.py` & `pondpond-1.3.0/tests/test_pond.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def validate(self, pooled_object: PooledObject) -> bool:
         return pooled_object.keeped_object.validate_result
 
 
 pooled_maxsize = 10
 pond = Pond(
     borrowed_timeout=2,
-    time_between_eviction_runs=-1,
+    time_between_eviction_runs=300,
     thread_daemon=True,
     eviction_weight=0.8,
 )
 factory = PooledDogFactory(pooled_maxsize=10, least_one=False)
 
 
 @pytest.mark.run(order=1)
```

### Comparing `pondpond-1.2.1/PKG-INFO` & `pondpond-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pondpond
-Version: 1.2.1
+Version: 1.3.0
 Summary: Pond is a high performance object-pooling library for Python.
 Author-email: Andy Qin <dr.qin@protonmail.com>
 Requires-Python: >=3.8
 Project-URL: Blog, https://qin.news
 Project-URL: Bug Tracker, https://github.com/t-baby/pond/issues
 Project-URL: Homepage, https://github.com/t-baby/pond
 Description-Content-Type: text/markdown
```

