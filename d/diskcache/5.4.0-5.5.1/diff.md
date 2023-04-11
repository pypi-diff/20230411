# Comparing `tmp/diskcache-5.4.0.tar.gz` & `tmp/diskcache-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diskcache-5.4.0.tar", last modified: Fri Dec 31 03:54:59 2021, max compression
+gzip compressed data, was "diskcache-5.5.1.tar", last modified: Tue Apr 11 06:56:24 2023, max compression
```

## Comparing `diskcache-5.4.0.tar` & `diskcache-5.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 03:54:59.392383 diskcache-5.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)      559 2021-12-31 03:54:13.000000 diskcache-5.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-12-31 03:54:13.000000 diskcache-5.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    20478 2021-12-31 03:54:59.392383 diskcache-5.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    19292 2021-12-31 03:54:13.000000 diskcache-5.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 03:54:59.388383 diskcache-5.4.0/diskcache/
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-12-31 03:54:13.000000 diskcache-5.4.0/diskcache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-12-31 03:54:13.000000 diskcache-5.4.0/diskcache/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    81956 2021-12-31 03:54:13.000000 diskcache-5.4.0/diskcache/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    16025 2021-12-31 03:54:13.000000 diskcache-5.4.0/diskcache/djangocache.py
--rw-r--r--   0 runner    (1001) docker     (121)    22031 2021-12-31 03:54:13.000000 diskcache-5.4.0/diskcache/fanout.py
--rw-r--r--   0 runner    (1001) docker     (121)    33159 2021-12-31 03:54:13.000000 diskcache-5.4.0/diskcache/persistent.py
--rw-r--r--   0 runner    (1001) docker     (121)    14144 2021-12-31 03:54:13.000000 diskcache-5.4.0/diskcache/recipes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-31 03:54:59.388383 diskcache-5.4.0/diskcache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    20478 2021-12-31 03:54:59.000000 diskcache-5.4.0/diskcache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      318 2021-12-31 03:54:59.000000 diskcache-5.4.0/diskcache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-31 03:54:59.000000 diskcache-5.4.0/diskcache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-31 03:54:59.000000 diskcache-5.4.0/diskcache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-31 03:54:59.392383 diskcache-5.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2021-12-31 03:54:13.000000 diskcache-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:56:24.908393 diskcache-5.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-11 06:54:26.000000 diskcache-5.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 06:54:26.000000 diskcache-5.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-11 06:56:24.908393 diskcache-5.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19292 2023-04-11 06:54:26.000000 diskcache-5.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:56:24.908393 diskcache-5.5.1/diskcache/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81934 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16025 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/djangocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33159 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-04-11 06:54:26.000000 diskcache-5.5.1/diskcache/recipes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 06:56:24.908393 diskcache-5.5.1/diskcache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-04-11 06:56:24.000000 diskcache-5.5.1/diskcache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-11 06:56:24.000000 diskcache-5.5.1/diskcache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 06:56:24.000000 diskcache-5.5.1/diskcache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 06:56:24.000000 diskcache-5.5.1/diskcache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 06:56:24.908393 diskcache-5.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-11 06:54:26.000000 diskcache-5.5.1/setup.py
```

### Comparing `diskcache-5.4.0/LICENSE` & `diskcache-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diskcache-5.4.0/PKG-INFO` & `diskcache-5.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: diskcache
-Version: 5.4.0
+Version: 5.5.1
 Summary: Disk Cache -- Disk and file backed persistent cache.
 Home-page: http://www.grantjenks.com/docs/diskcache/
 Author: Grant Jenks
 Author-email: contact@grantjenks.com
 License: Apache 2.0
 Project-URL: Documentation, http://www.grantjenks.com/docs/diskcache/
 Project-URL: Funding, https://gum.co/diskcache
 Project-URL: Source, https://github.com/grantjenks/python-diskcache
 Project-URL: Tracker, https://github.com/grantjenks/python-diskcache/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -28,15 +27,15 @@
 
 DiskCache: Disk Backed Cache
 ============================
 
 `DiskCache`_ is an Apache2 licensed disk and file backed cache library, written
 in pure-Python, and compatible with Django.
 
-The cloud-based computing of 2021 puts a premium on memory. Gigabytes of empty
+The cloud-based computing of 2023 puts a premium on memory. Gigabytes of empty
 space is left on disks as processes vie for memory. Among these processes is
 Memcached (and sometimes Redis) which is used as a cache. Wouldn't it be nice
 to leverage empty disk space for caching?
 
 Django is Python's most popular web framework and ships with several caching
 backends. Unfortunately the file-based cache in Django is essentially
 broken. The culling method is random and large caches repeatedly scan a cache
@@ -411,23 +410,21 @@
 .. _`DiskCache at PyPI`: https://pypi.python.org/pypi/diskcache/
 .. _`DiskCache at GitHub`: https://github.com/grantjenks/python-diskcache/
 .. _`DiskCache Issue Tracker`: https://github.com/grantjenks/python-diskcache/issues/
 
 License
 -------
 
-Copyright 2016-2022 Grant Jenks
+Copyright 2016-2023 Grant Jenks
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
 this file except in compliance with the License.  You may obtain a copy of the
 License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed
 under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
 CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 
 .. _`DiskCache`: http://www.grantjenks.com/docs/diskcache/
-
-
```

### Comparing `diskcache-5.4.0/README.rst` & `diskcache-5.5.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 DiskCache: Disk Backed Cache
 ============================
 
 `DiskCache`_ is an Apache2 licensed disk and file backed cache library, written
 in pure-Python, and compatible with Django.
 
-The cloud-based computing of 2021 puts a premium on memory. Gigabytes of empty
+The cloud-based computing of 2023 puts a premium on memory. Gigabytes of empty
 space is left on disks as processes vie for memory. Among these processes is
 Memcached (and sometimes Redis) which is used as a cache. Wouldn't it be nice
 to leverage empty disk space for caching?
 
 Django is Python's most popular web framework and ships with several caching
 backends. Unfortunately the file-based cache in Django is essentially
 broken. The culling method is random and large caches repeatedly scan a cache
@@ -383,15 +383,15 @@
 .. _`DiskCache at PyPI`: https://pypi.python.org/pypi/diskcache/
 .. _`DiskCache at GitHub`: https://github.com/grantjenks/python-diskcache/
 .. _`DiskCache Issue Tracker`: https://github.com/grantjenks/python-diskcache/issues/
 
 License
 -------
 
-Copyright 2016-2022 Grant Jenks
+Copyright 2016-2023 Grant Jenks
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
 this file except in compliance with the License.  You may obtain a copy of the
 License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `diskcache-5.4.0/diskcache/__init__.py` & `diskcache-5.5.1/diskcache/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,12 +57,12 @@
 
     __all__.append('DjangoCache')
 except Exception:  # pylint: disable=broad-except  # pragma: no cover
     # Django not installed or not setup so ignore.
     pass
 
 __title__ = 'diskcache'
-__version__ = '5.4.0'
-__build__ = 0x050400
+__version__ = '5.5.1'
+__build__ = 0x050501
 __author__ = 'Grant Jenks'
 __license__ = 'Apache 2.0'
-__copyright__ = 'Copyright 2016-2022 Grant Jenks'
+__copyright__ = 'Copyright 2016-2023 Grant Jenks'
```

### Comparing `diskcache-5.4.0/diskcache/core.py` & `diskcache-5.5.1/diskcache/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,22 @@
 MODE_TEXT = 3
 MODE_PICKLE = 4
 
 DEFAULT_SETTINGS = {
     'statistics': 0,  # False
     'tag_index': 0,  # False
     'eviction_policy': 'least-recently-stored',
-    'size_limit': 2 ** 30,  # 1gb
+    'size_limit': 2**30,  # 1gb
     'cull_limit': 10,
     'sqlite_auto_vacuum': 1,  # FULL
-    'sqlite_cache_size': 2 ** 13,  # 8,192 pages
+    'sqlite_cache_size': 2**13,  # 8,192 pages
     'sqlite_journal_mode': 'wal',
-    'sqlite_mmap_size': 2 ** 26,  # 64mb
+    'sqlite_mmap_size': 2**26,  # 64mb
     'sqlite_synchronous': 1,  # NORMAL
-    'disk_min_file_size': 2 ** 15,  # 32kb
+    'disk_min_file_size': 2**15,  # 32kb
     'disk_pickle_protocol': pickle.HIGHEST_PROTOCOL,
 }
 
 METADATA = {
     'count': 0,
     'size': 0,
     'hits': 0,
@@ -166,15 +166,15 @@
         """Convert fields `key` and `raw` from Cache table to key.
 
         :param key: database key to convert
         :param bool raw: flag indicating raw database storage
         :return: corresponding Python key
 
         """
-        # pylint: disable=no-self-use,unidiomatic-typecheck
+        # pylint: disable=unidiomatic-typecheck
         if raw:
             return bytes(key) if type(key) is sqlite3.Binary else key
         else:
             return pickle.load(io.BytesIO(key))
 
     def store(self, value, read, key=UNKNOWN):
         """Convert `value` to fields size, mode, filename, and value for Cache
@@ -208,15 +208,15 @@
                 return len(value), MODE_BINARY, filename, None
         elif type_value is str:
             filename, full_path = self.filename(key, value)
             self._write(full_path, io.StringIO(value), 'x', 'UTF-8')
             size = op.getsize(full_path)
             return size, MODE_TEXT, filename, None
         elif read:
-            reader = ft.partial(value.read, 2 ** 22)
+            reader = ft.partial(value.read, 2**22)
             filename, full_path = self.filename(key, value)
             iterator = iter(reader, b'')
             size = self._write(full_path, iterator, 'xb')
             return size, MODE_BINARY, filename, None
         else:
             result = pickle.dumps(value, protocol=self.pickle_protocol)
 
@@ -224,15 +224,14 @@
                 return 0, MODE_PICKLE, None, sqlite3.Binary(result)
             else:
                 filename, full_path = self.filename(key, value)
                 self._write(full_path, io.BytesIO(result), 'xb')
                 return len(result), MODE_PICKLE, filename, None
 
     def _write(self, full_path, iterator, mode, encoding=None):
-        # pylint: disable=no-self-use
         full_dir, _ = op.split(full_path)
 
         for count in range(1, 11):
             with cl.suppress(OSError):
                 os.makedirs(full_dir)
 
             try:
@@ -260,15 +259,15 @@
         :param str filename: filename of corresponding value
         :param value: database value
         :param bool read: when True, return an open file handle
         :return: corresponding Python value
         :raises: IOError if the value cannot be read
 
         """
-        # pylint: disable=no-self-use,unidiomatic-typecheck,consider-using-with
+        # pylint: disable=unidiomatic-typecheck,consider-using-with
         if mode == MODE_RAW:
             return bytes(value) if type(value) is sqlite3.Binary else value
         elif mode == MODE_BINARY:
             if read:
                 return open(op.join(self._directory, filename), 'rb')
             else:
                 with open(op.join(self._directory, filename), 'rb') as reader:
@@ -1374,14 +1373,15 @@
 
         :param key: key matching item
         :param bool retry: retry if database timeout occurs (default False)
         :return: True if item was deleted
         :raises Timeout: if database timeout occurs
 
         """
+        # pylint: disable=unnecessary-dunder-call
         try:
             return self.__delitem__(key, retry=retry)
         except KeyError:
             return False
 
     def push(
         self,
```

### Comparing `diskcache-5.4.0/diskcache/djangocache.py` & `diskcache-5.5.1/diskcache/djangocache.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.4.0/diskcache/fanout.py` & `diskcache-5.5.1/diskcache/fanout.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self._disk = disk
         self._shards = tuple(
             Cache(
                 directory=op.join(directory, '%03d' % num),
                 timeout=timeout,
                 disk=disk,
                 size_limit=size_limit,
-                **settings
+                **settings,
             )
             for num in range(shards)
         )
         self._hash = self._shards[0].disk.hash
         self._caches = {}
         self._deques = {}
         self._indexes = {}
@@ -569,40 +569,50 @@
                     result = shard.reset(key, value)
                 except Timeout:
                     pass
                 else:
                     break
         return result
 
-    def cache(self, name):
+    def cache(self, name, timeout=60, disk=None, **settings):
         """Return Cache with given `name` in subdirectory.
 
+        If disk is none (default), uses the fanout cache disk.
+
         >>> fanout_cache = FanoutCache()
         >>> cache = fanout_cache.cache('test')
         >>> cache.set('abc', 123)
         True
         >>> cache.get('abc')
         123
         >>> len(cache)
         1
         >>> cache.delete('abc')
         True
 
         :param str name: subdirectory name for Cache
+        :param float timeout: SQLite connection timeout
+        :param disk: Disk type or subclass for serialization
+        :param settings: any of DEFAULT_SETTINGS
         :return: Cache with given name
 
         """
         _caches = self._caches
 
         try:
             return _caches[name]
         except KeyError:
             parts = name.split('/')
             directory = op.join(self._directory, 'cache', *parts)
-            temp = Cache(directory=directory, disk=self._disk)
+            temp = Cache(
+                directory=directory,
+                timeout=timeout,
+                disk=self._disk if disk is None else Disk,
+                **settings,
+            )
             _caches[name] = temp
             return temp
 
     def deque(self, name):
         """Return Deque with given `name` in subdirectory.
 
         >>> cache = FanoutCache()
@@ -622,15 +632,19 @@
         _deques = self._deques
 
         try:
             return _deques[name]
         except KeyError:
             parts = name.split('/')
             directory = op.join(self._directory, 'deque', *parts)
-            cache = Cache(directory=directory, disk=self._disk)
+            cache = Cache(
+                directory=directory,
+                disk=self._disk,
+                eviction_policy='none',
+            )
             deque = Deque.fromcache(cache)
             _deques[name] = deque
             return deque
 
     def index(self, name):
         """Return Index with given `name` in subdirectory.
 
@@ -654,14 +668,18 @@
         _indexes = self._indexes
 
         try:
             return _indexes[name]
         except KeyError:
             parts = name.split('/')
             directory = op.join(self._directory, 'index', *parts)
-            cache = Cache(directory=directory, disk=self._disk)
+            cache = Cache(
+                directory=directory,
+                disk=self._disk,
+                eviction_policy='none',
+            )
             index = Index.fromcache(cache)
             _indexes[name] = index
             return index
 
 
 FanoutCache.memoize = Cache.memoize  # type: ignore
```

### Comparing `diskcache-5.4.0/diskcache/persistent.py` & `diskcache-5.5.1/diskcache/persistent.py`

 * *Files identical despite different names*

### Comparing `diskcache-5.4.0/diskcache/recipes.py` & `diskcache-5.5.1/diskcache/recipes.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 class Averager:
     """Recipe for calculating a running average.
 
     Sometimes known as "online statistics," the running average maintains the
     total and count. The average can then be calculated at any time.
 
+    Assumes the key will not be evicted. Set the eviction policy to 'none' on
+    the cache to guarantee the key is not evicted.
+
     >>> import diskcache
     >>> cache = diskcache.FanoutCache()
     >>> ave = Averager(cache, 'latency')
     >>> ave.add(0.080)
     >>> ave.add(0.120)
     >>> ave.get()
     0.1
@@ -61,14 +64,17 @@
         total, count = self._cache.pop(self._key, default=(0.0, 0), retry=True)
         return None if count == 0 else total / count
 
 
 class Lock:
     """Recipe for cross-process and cross-thread lock.
 
+    Assumes the key will not be evicted. Set the eviction policy to 'none' on
+    the cache to guarantee the key is not evicted.
+
     >>> import diskcache
     >>> cache = diskcache.Cache()
     >>> lock = Lock(cache, 'report-123')
     >>> lock.acquire()
     >>> lock.release()
     >>> with lock:
     ...     pass
@@ -109,14 +115,17 @@
     def __exit__(self, *exc_info):
         self.release()
 
 
 class RLock:
     """Recipe for cross-process and cross-thread re-entrant lock.
 
+    Assumes the key will not be evicted. Set the eviction policy to 'none' on
+    the cache to guarantee the key is not evicted.
+
     >>> import diskcache
     >>> cache = diskcache.Cache()
     >>> rlock = RLock(cache, 'user-123')
     >>> rlock.acquire()
     >>> rlock.acquire()
     >>> rlock.release()
     >>> with rlock:
@@ -177,14 +186,17 @@
     def __exit__(self, *exc_info):
         self.release()
 
 
 class BoundedSemaphore:
     """Recipe for cross-process and cross-thread bounded semaphore.
 
+    Assumes the key will not be evicted. Set the eviction policy to 'none' on
+    the cache to guarantee the key is not evicted.
+
     >>> import diskcache
     >>> cache = diskcache.Cache()
     >>> semaphore = BoundedSemaphore(cache, 'max-cons', value=2)
     >>> semaphore.acquire()
     >>> semaphore.acquire()
     >>> semaphore.release()
     >>> with semaphore:
@@ -247,14 +259,17 @@
     expire=None,
     tag=None,
     time_func=time.time,
     sleep_func=time.sleep,
 ):
     """Decorator to throttle calls to function.
 
+    Assumes keys will not be evicted. Set the eviction policy to 'none' on the
+    cache to guarantee the keys are not evicted.
+
     >>> import diskcache, time
     >>> cache = diskcache.Cache()
     >>> count = 0
     >>> @throttle(cache, 2, 1)  # 2 calls per 1 second
     ... def increment():
     ...     global count
     ...     count += 1
@@ -301,14 +316,17 @@
 
 
 def barrier(cache, lock_factory, name=None, expire=None, tag=None):
     """Barrier to calling decorated function.
 
     Supports different kinds of locks: Lock, RLock, BoundedSemaphore.
 
+    Assumes keys will not be evicted. Set the eviction policy to 'none' on the
+    cache to guarantee the keys are not evicted.
+
     >>> import diskcache, time
     >>> cache = diskcache.Cache()
     >>> @barrier(cache, Lock)
     ... def work(num):
     ...     print('worker started')
     ...     time.sleep(1)
     ...     print('worker finished')
```

### Comparing `diskcache-5.4.0/diskcache.egg-info/PKG-INFO` & `diskcache-5.5.1/diskcache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: diskcache
-Version: 5.4.0
+Version: 5.5.1
 Summary: Disk Cache -- Disk and file backed persistent cache.
 Home-page: http://www.grantjenks.com/docs/diskcache/
 Author: Grant Jenks
 Author-email: contact@grantjenks.com
 License: Apache 2.0
 Project-URL: Documentation, http://www.grantjenks.com/docs/diskcache/
 Project-URL: Funding, https://gum.co/diskcache
 Project-URL: Source, https://github.com/grantjenks/python-diskcache
 Project-URL: Tracker, https://github.com/grantjenks/python-diskcache/issues
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
@@ -28,15 +27,15 @@
 
 DiskCache: Disk Backed Cache
 ============================
 
 `DiskCache`_ is an Apache2 licensed disk and file backed cache library, written
 in pure-Python, and compatible with Django.
 
-The cloud-based computing of 2021 puts a premium on memory. Gigabytes of empty
+The cloud-based computing of 2023 puts a premium on memory. Gigabytes of empty
 space is left on disks as processes vie for memory. Among these processes is
 Memcached (and sometimes Redis) which is used as a cache. Wouldn't it be nice
 to leverage empty disk space for caching?
 
 Django is Python's most popular web framework and ships with several caching
 backends. Unfortunately the file-based cache in Django is essentially
 broken. The culling method is random and large caches repeatedly scan a cache
@@ -411,23 +410,21 @@
 .. _`DiskCache at PyPI`: https://pypi.python.org/pypi/diskcache/
 .. _`DiskCache at GitHub`: https://github.com/grantjenks/python-diskcache/
 .. _`DiskCache Issue Tracker`: https://github.com/grantjenks/python-diskcache/issues/
 
 License
 -------
 
-Copyright 2016-2022 Grant Jenks
+Copyright 2016-2023 Grant Jenks
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
 this file except in compliance with the License.  You may obtain a copy of the
 License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software distributed
 under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
 CONDITIONS OF ANY KIND, either express or implied. See the License for the
 specific language governing permissions and limitations under the License.
 
 .. _`DiskCache`: http://www.grantjenks.com/docs/diskcache/
-
-
```

### Comparing `diskcache-5.4.0/setup.py` & `diskcache-5.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from io import open
-
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 
 import diskcache
 
 
 class Tox(TestCommand):
```

