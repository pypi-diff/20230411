# Comparing `tmp/adt_cache-0.0.1.tar.gz` & `tmp/adt_cache-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adt_cache-0.0.1.tar", last modified: Mon Apr 10 13:47:25 2023, max compression
+gzip compressed data, was "dist/adt_cache-0.0.2.tar", last modified: Tue Apr 11 08:43:56 2023, max compression
```

## Comparing `adt_cache-0.0.1.tar` & `adt_cache-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-10 13:47:25.000000 adt_cache-0.0.1/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-10 13:47:25.000000 adt_cache-0.0.1/PKG-INFO
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-10 13:47:25.000000 adt_cache-0.0.1/cache/
--rw-r--r--   0 nezah      (501) staff       (20)     1416 2023-04-10 13:46:41.000000 adt_cache-0.0.1/cache/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.1/LICENSE
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-10 13:47:25.000000 adt_cache-0.0.1/adt_cache.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-10 13:47:25.000000 adt_cache-0.0.1/adt_cache.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-10 13:47:25.000000 adt_cache-0.0.1/adt_cache.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-10 13:47:25.000000 adt_cache-0.0.1/adt_cache.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-10 13:47:25.000000 adt_cache-0.0.1/adt_cache.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.1/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-04 15:20:44.000000 adt_cache-0.0.1/setup.py
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-10 13:47:25.000000 adt_cache-0.0.1/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:43:56.000000 adt_cache-0.0.2/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-11 08:43:56.000000 adt_cache-0.0.2/PKG-INFO
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:43:56.000000 adt_cache-0.0.2/cache/
+-rw-r--r--   0 nezah      (501) staff       (20)     1879 2023-04-10 16:52:00.000000 adt_cache-0.0.2/cache/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)     1071 2023-04-05 05:19:07.000000 adt_cache-0.0.2/LICENSE
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-04-11 08:43:56.000000 adt_cache-0.0.2/adt_cache.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)      597 2023-04-11 08:43:56.000000 adt_cache-0.0.2/adt_cache.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      176 2023-04-11 08:43:56.000000 adt_cache-0.0.2/adt_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        6 2023-04-11 08:43:56.000000 adt_cache-0.0.2/adt_cache.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-04-11 08:43:56.000000 adt_cache-0.0.2/adt_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)      172 2023-04-05 05:18:33.000000 adt_cache-0.0.2/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      548 2023-04-11 08:42:38.000000 adt_cache-0.0.2/setup.py
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-04-11 08:43:56.000000 adt_cache-0.0.2/setup.cfg
```

### Comparing `adt_cache-0.0.1/PKG-INFO` & `adt_cache-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt_cache
-Version: 0.0.1
+Version: 0.0.2
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.1/cache/__init__.py` & `adt_cache-0.0.2/cache/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import logging
 from abc import abstractmethod, ABCMeta
 from typing import List
 import redis
 
+logger = logging.getLogger("adt_cache")
 
 class AdtCache(metaclass=ABCMeta):
     def __init__(self):
         pass
 
     @abstractmethod
     def intersect(self, key: str, vals: List):
@@ -15,29 +17,41 @@
     def differential(self, key: str, vals: List):
         pass
 
     @abstractmethod
     def push_values(self, key: str, vals: List):
         pass
 
+    @abstractmethod
+    def keys(self):
+        pass
+
 
 class RedisCache(AdtCache):
-    def __init__(self, host: str, port, db):
+    def __init__(self, host: str, port, db, expire_mins=60*24, clear_cache=False):
+        logger.info(f"init redis cache with {host}:{port}:{db}")
         super().__init__()
         self.redis = redis.Redis(host=host, port=port, db=db)
+        self.expire_mins=expire_mins
+        if clear_cache:
+            self.redis.flushdb()
 
     def intersect(self, key, vals: List):
         return [val for val in vals if self.redis.sismember(key, val)]
 
     def differential(self, key, vals: List):
         return [val for val in vals if not self.redis.sismember(key, val)]
 
     def push_values(self, key, vals: List):
+        self.redis.expire(key, 60 * self.expire_mins)
         return self.redis.sadd(key, *set(vals))
 
+    def keys(self):
+        return self.redis.keys()
+
 
 class MemoryCache(AdtCache):
     def __init__(self):
         super().__init__()
         self.cache = {}
 
     def intersect(self, key, vals: List):
@@ -47,8 +61,11 @@
         return [val for val in vals if val not in self.cache.get(key, [])]
 
     def push_values(self, key, vals: List):
         c = self.cache.get(key)
         if c is None:
             self.cache[key] = set(vals)
         else:
-            c.extend(set(vals))
+            c.update(vals)
+
+    def keys(self):
+        return self.cache.keys()
```

### Comparing `adt_cache-0.0.1/LICENSE` & `adt_cache-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adt_cache-0.0.1/adt_cache.egg-info/PKG-INFO` & `adt_cache-0.0.2/adt_cache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adt-cache
-Version: 0.0.1
+Version: 0.0.2
 Summary: abstract cache with in memory cache or redis (sentinel)
 Home-page: https://github.com/cheddars/pypi_adt_cache
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `adt_cache-0.0.1/setup.py` & `adt_cache-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="adt_cache",
-    version="0.0.1",
+    version="0.0.2",
     license='MIT',
     author="cheddars",
     author_email="nezahrish@gmail.com",
     description="abstract cache with in memory cache or redis (sentinel)",
     long_description=open('README.md').read(),
     url="https://github.com/cheddars/pypi_adt_cache",
     packages=setuptools.find_packages(),
```

