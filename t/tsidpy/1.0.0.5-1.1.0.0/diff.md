# Comparing `tmp/tsidpy-1.0.0.5.tar.gz` & `tmp/tsidpy-1.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsidpy-1.0.0.5.tar", last modified: Sun Apr  9 08:10:53 2023, max compression
+gzip compressed data, was "tsidpy-1.1.0.0.tar", last modified: Mon Apr 10 22:29:21 2023, max compression
```

## Comparing `tsidpy-1.0.0.5.tar` & `tsidpy-1.1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 08:10:53.966089 tsidpy-1.0.0.5/
--rw-r--r--   0 luis       (504) staff       (20)     1066 2023-04-09 01:27:26.000000 tsidpy-1.0.0.5/LICENSE
--rw-r--r--   0 luis       (504) staff       (20)    10340 2023-04-09 08:10:53.965292 tsidpy-1.0.0.5/PKG-INFO
--rw-r--r--   0 luis       (504) staff       (20)     9823 2023-04-09 08:06:43.000000 tsidpy-1.0.0.5/README.md
--rw-r--r--   0 luis       (504) staff       (20)      594 2023-04-09 08:10:40.000000 tsidpy-1.0.0.5/pyproject.toml
--rw-r--r--   0 luis       (504) staff       (20)       38 2023-04-09 08:10:53.966261 tsidpy-1.0.0.5/setup.cfg
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 08:10:53.955942 tsidpy-1.0.0.5/src/
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 08:10:53.961152 tsidpy-1.0.0.5/src/tsidpy/
--rw-r--r--   0 luis       (504) staff       (20)       51 2023-04-08 23:04:41.000000 tsidpy-1.0.0.5/src/tsidpy/__init__.py
--rw-r--r--   0 luis       (504) staff       (20)      690 2023-04-07 23:41:36.000000 tsidpy-1.0.0.5/src/tsidpy/basen.py
--rw-r--r--   0 luis       (504) staff       (20)    14728 2023-04-09 00:00:39.000000 tsidpy-1.0.0.5/src/tsidpy/tsid.py
-drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-09 08:10:53.964490 tsidpy-1.0.0.5/src/tsidpy.egg-info/
--rw-r--r--   0 luis       (504) staff       (20)    10340 2023-04-09 08:10:53.000000 tsidpy-1.0.0.5/src/tsidpy.egg-info/PKG-INFO
--rw-r--r--   0 luis       (504) staff       (20)      230 2023-04-09 08:10:53.000000 tsidpy-1.0.0.5/src/tsidpy.egg-info/SOURCES.txt
--rw-r--r--   0 luis       (504) staff       (20)        1 2023-04-09 08:10:53.000000 tsidpy-1.0.0.5/src/tsidpy.egg-info/dependency_links.txt
--rw-r--r--   0 luis       (504) staff       (20)        7 2023-04-09 08:10:53.000000 tsidpy-1.0.0.5/src/tsidpy.egg-info/top_level.txt
+drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-10 22:29:21.347532 tsidpy-1.1.0.0/
+-rw-r--r--   0 luis       (504) staff       (20)     1066 2023-04-09 01:27:26.000000 tsidpy-1.1.0.0/LICENSE
+-rw-r--r--   0 luis       (504) staff       (20)    10499 2023-04-10 22:29:21.346385 tsidpy-1.1.0.0/PKG-INFO
+-rw-r--r--   0 luis       (504) staff       (20)     9982 2023-04-10 22:16:17.000000 tsidpy-1.1.0.0/README.md
+-rw-r--r--   0 luis       (504) staff       (20)      594 2023-04-10 22:17:00.000000 tsidpy-1.1.0.0/pyproject.toml
+-rw-r--r--   0 luis       (504) staff       (20)       38 2023-04-10 22:29:21.347854 tsidpy-1.1.0.0/setup.cfg
+drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-10 22:29:21.335232 tsidpy-1.1.0.0/src/
+drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-10 22:29:21.341328 tsidpy-1.1.0.0/src/tsidpy/
+-rw-r--r--   0 luis       (504) staff       (20)       63 2023-04-10 20:20:01.000000 tsidpy-1.1.0.0/src/tsidpy/__init__.py
+-rw-r--r--   0 luis       (504) staff       (20)      690 2023-04-07 23:41:36.000000 tsidpy-1.1.0.0/src/tsidpy/basen.py
+-rw-r--r--   0 luis       (504) staff       (20)    15237 2023-04-10 21:52:42.000000 tsidpy-1.1.0.0/src/tsidpy/tsid.py
+drwxr-xr-x   0 luis       (504) staff       (20)        0 2023-04-10 22:29:21.345124 tsidpy-1.1.0.0/src/tsidpy.egg-info/
+-rw-r--r--   0 luis       (504) staff       (20)    10499 2023-04-10 22:29:21.000000 tsidpy-1.1.0.0/src/tsidpy.egg-info/PKG-INFO
+-rw-r--r--   0 luis       (504) staff       (20)      230 2023-04-10 22:29:21.000000 tsidpy-1.1.0.0/src/tsidpy.egg-info/SOURCES.txt
+-rw-r--r--   0 luis       (504) staff       (20)        1 2023-04-10 22:29:21.000000 tsidpy-1.1.0.0/src/tsidpy.egg-info/dependency_links.txt
+-rw-r--r--   0 luis       (504) staff       (20)        7 2023-04-10 22:29:21.000000 tsidpy-1.1.0.0/src/tsidpy.egg-info/top_level.txt
```

### Comparing `tsidpy-1.0.0.5/LICENSE` & `tsidpy-1.1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsidpy-1.0.0.5/PKG-INFO` & `tsidpy-1.1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsidpy
-Version: 1.0.0.5
+Version: 1.1.0.0
 Summary: A Python library for generating Time-Sorted Unique Identifiers (TSID)
 Author-email: Luis Medel <luis@luismedel.com>
 Project-URL: Homepage, https://github.com/luismedel/tsid-python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -235,19 +235,19 @@
 ```python
 >>> tsid.to_string('s')
 '0123456789abc'
 ```
 
 ---
 
-Get the creation `datetime` of a TSID:
+Get the creation `timestamp` of a TSID:
 
 ```python
->>> tsid.datetime
-datetime.datetime(2023, 4, 8, 12, 6, 58, 241000)
+>>> tsid.timestamp
+1680948418241.0  # datetime.datetime(2023, 4, 8, 12, 6, 58, 241000)
 ```
 
 ---
 
 Encode a TSID to base-62:
 
 ```python
@@ -268,16 +268,16 @@
 
 datacenter: int = 1
 worker: int = 1
 node: int = datacenter << 5 | worker
 epoch: datetime = datetime.fromisoformat('2010-11-04T01:42:54.657Z')
 
 twitter_generator: TSIDGenerator = TSIDGenerator(node=node, node_bits=10,
-                                                 epoch=epoch,
-                                                 random_fn=lambda: 0)
+                                                 epoch=epoch.timestamp() * 1000,
+                                                 random_fn=lambda n: 0)
 
 # use the generator
 tsid: TSID = twitter_generator.create()
 ```
 
 ---
 
@@ -292,15 +292,15 @@
 
 worker: int = 1
 process: int = 1
 node: int = worker << 5 | process
 epoch: datetime = datetime.fromisoformat("2015-01-01T00:00:00.000Z")
 
 discord_generator: TSIDGenerator = TSIDGenerator(node=node, node_bits=10,
-                                                 epoch=epoch)
+                                                 epoch=epoch.timestamp() * 1000)
 
 # use the generator
 tsid: TSID = discord_generator.create()
 ```
 
 ---
 
@@ -337,14 +337,15 @@
 
 ## Other ports, forks and OSS
 
 ### Ports and forks
 
 | Language | Name |
 | -------- | ---- |
+| Java (by original author)     | [f4b6a3/tsid-creator](https://github.com/f4b6a3/tsid-creator) |
 | Java     | [vladmihalcea/hypersistence-tsid](https://github.com/vladmihalcea/hypersistence-tsid) |
 | .NET     | [kgkoutis/TSID.Creator.NET](https://github.com/kgkoutis/TSID.Creator.NET) |
 | PHP      | [odan/tsid](https://github.com/odan/tsid) |
 
 ### OSS
 
 | Language | Name |
```

### Comparing `tsidpy-1.0.0.5/README.md` & `tsidpy-1.1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -221,19 +221,19 @@
 ```python
 >>> tsid.to_string('s')
 '0123456789abc'
 ```
 
 ---
 
-Get the creation `datetime` of a TSID:
+Get the creation `timestamp` of a TSID:
 
 ```python
->>> tsid.datetime
-datetime.datetime(2023, 4, 8, 12, 6, 58, 241000)
+>>> tsid.timestamp
+1680948418241.0  # datetime.datetime(2023, 4, 8, 12, 6, 58, 241000)
 ```
 
 ---
 
 Encode a TSID to base-62:
 
 ```python
@@ -254,16 +254,16 @@
 
 datacenter: int = 1
 worker: int = 1
 node: int = datacenter << 5 | worker
 epoch: datetime = datetime.fromisoformat('2010-11-04T01:42:54.657Z')
 
 twitter_generator: TSIDGenerator = TSIDGenerator(node=node, node_bits=10,
-                                                 epoch=epoch,
-                                                 random_fn=lambda: 0)
+                                                 epoch=epoch.timestamp() * 1000,
+                                                 random_fn=lambda n: 0)
 
 # use the generator
 tsid: TSID = twitter_generator.create()
 ```
 
 ---
 
@@ -278,15 +278,15 @@
 
 worker: int = 1
 process: int = 1
 node: int = worker << 5 | process
 epoch: datetime = datetime.fromisoformat("2015-01-01T00:00:00.000Z")
 
 discord_generator: TSIDGenerator = TSIDGenerator(node=node, node_bits=10,
-                                                 epoch=epoch)
+                                                 epoch=epoch.timestamp() * 1000)
 
 # use the generator
 tsid: TSID = discord_generator.create()
 ```
 
 ---
 
@@ -323,14 +323,15 @@
 
 ## Other ports, forks and OSS
 
 ### Ports and forks
 
 | Language | Name |
 | -------- | ---- |
+| Java (by original author)     | [f4b6a3/tsid-creator](https://github.com/f4b6a3/tsid-creator) |
 | Java     | [vladmihalcea/hypersistence-tsid](https://github.com/vladmihalcea/hypersistence-tsid) |
 | .NET     | [kgkoutis/TSID.Creator.NET](https://github.com/kgkoutis/TSID.Creator.NET) |
 | PHP      | [odan/tsid](https://github.com/odan/tsid) |
 
 ### OSS
 
 | Language | Name |
```

### Comparing `tsidpy-1.0.0.5/pyproject.toml` & `tsidpy-1.1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tsidpy"
-version = "1.0.0.5"
+version = "1.1.0.0"
 authors = [
   { name="Luis Medel", email="luis@luismedel.com" },
 ]
 description = "A Python library for generating Time-Sorted Unique Identifiers (TSID)"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tsidpy-1.0.0.5/src/tsidpy/basen.py` & `tsidpy-1.1.0.0/src/tsidpy/basen.py`

 * *Files identical despite different names*

### Comparing `tsidpy-1.0.0.5/src/tsidpy/tsid.py` & `tsidpy-1.1.0.0/src/tsidpy/tsid.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 
 import functools
+import random
 import threading
+import time
 import typing as t
 
-from datetime import datetime, timedelta
-from random import random
+from datetime import datetime
 
 from .basen import decode, encode
 
-
 TSID_BYTES: int = 8
 TSID_CHARS: int = 13
 
-TSID_EPOCH: datetime = datetime.fromisoformat("2020-01-01")
-_TSID_EPOCH_MILLIS = int(TSID_EPOCH.timestamp() * 1000)
+_EPOCH_ISO: str = '2020-01-01 00:00:00+00:00'
+TSID_EPOCH: float = datetime.fromisoformat(_EPOCH_ISO).timestamp() * 1000
 
 RANDOM_BITS: int = 22
 RANDOM_MASK: int = 0x3fffff
 
 TSID_DEFAULT_NODE_BITS = 10
 
 ALPHABET: str = '0123456789ABCDEFGHJKMNPQRSTVWXYZ'
@@ -68,45 +68,49 @@
 
     def __init__(self, number: int) -> None:
         """
         >>> TSID(0x10000000000000000).number == 0
         True
         """
         self.__number: int = number & 0xffffffffffffffff  # 64-bit
+        self._epoch: float = TSID_EPOCH
 
     @property
-    def datetime(self, epoch: datetime | None = None) -> datetime:
-        """Returns the time component of the TSID.
+    def timestamp(self) -> float:
+        """Returns the timestamp component of the TSID.
+           The timestamp is the number of milliseconds elapsed
+           since the TSID epoch.
 
-        >>> TSID(0).datetime == TSID_EPOCH
+        >>> TSID(0).timestamp == TSID_EPOCH
+        True
+        >>> TSID.create().timestamp - time.time() * 1000 < 1
         True
-        >>> delta = timedelta(milliseconds=1)
-        >>> TSID(1 << RANDOM_BITS).datetime == TSID_EPOCH + delta
+        >>> TSID(1 << RANDOM_BITS).timestamp == TSID_EPOCH + 1
         True
         """
-        epoch = epoch or TSID_EPOCH
-        return epoch + timedelta(milliseconds=self.__number >> RANDOM_BITS)
+        return self._epoch + (self.__number >> RANDOM_BITS)
 
     @property
     def random(self) -> int:
         """Returns the random component of the TSID.
+           This compomnent contains the node and counter
+           bits.
 
         >>> TSID(0).random == 0
         True
         >>> TSID(1).random == 1
         True
         >>> TSID((0xffffffff << RANDOM_BITS) + 255).random == 255
         True
         """
         return self.__number & RANDOM_MASK
 
     @property
     def number(self) -> int:
         """Converts the TSID into a 64-bit number.
-
            This simply unwraps the internal value
 
         >>> TSID(0xffff0000000000000000).number == 0
         True
         >>> TSID(0x0000000000000000).number == 0
         True
         >>> TSID(0xffff).number == 0xffff
@@ -204,22 +208,23 @@
             case 'S':  # canonical string in upper case
                 result = self._to_canonical_string()
             case 's':  # canonical string in lower case
                 result = self._to_canonical_string().lower()
             case 'X':  # hexadecimal in upper case
                 result = encode(self.number, 16, min_length=TSID_BYTES*2)
             case 'x':  # hexadecimal in lower case
-                result = encode(self.number, 16, min_length=TSID_BYTES*2).lower()
+                result = encode(self.number, 16, min_length=TSID_BYTES*2)
+                result = result.lower()
             case 'd':  # base-10
                 result = encode(self.number, 10)
             case 'z':  # base-62
                 result = encode(self.number, 62)
             case _:
                 raise ValueError(f"Invalid format: '{fmt}'")
-        
+
         return result
 
     def _to_canonical_string(self) -> str:
         return ''.join(ALPHABET[self.__number >> i & 0x1f]
                        for i in range(60, -5, -5))
 
     @staticmethod
@@ -239,18 +244,14 @@
            TSIDGenerator responsibility to ensure thread safety.
 
         >>> a = TSID.create()
         >>> b = TSID.create()
         >>> c = TSID.create()
         >>> a.number < b.number < c.number
         True
-        >>> a.datetime == b.datetime == c.datetime
-        True
-        >>> a.random < b.random < c.random
-        True
         """
         return _default_generator.create()
 
     @staticmethod
     def from_bytes(bytes: bytes) -> 'TSID':
         r"""Converts a byte array into a TSID.
 
@@ -290,15 +291,15 @@
         number: int
 
         match fmt:
             case 'S' | 's':
                 if len(value) != TSID_CHARS:
                     raise ValueError("Invalid TSID string")
                 number = sum(ALPHABET_VALUES[ord(value[i])] << h
-                            for i, h in enumerate(range(60, -5, -5), 0))
+                             for i, h in enumerate(range(60, -5, -5), 0))
             case 'X':  # hexadecimal in upper case
                 number = decode(value, 16)
             case 'x':  # hexadecimal in lower case
                 number = decode(value.upper(), 16)
             case 'd':  # base-10
                 number = decode(value, 10)
             case 'z':  # base-62
@@ -320,29 +321,29 @@
 
 
 class TSIDGenerator:
     def __init__(
         self,
         node: int | None = None,
         node_bits: int = TSID_DEFAULT_NODE_BITS,
-        epoch: datetime = TSID_EPOCH,
-        random_fn: t.Callable[[], int] | None = None
+        epoch: float = TSID_EPOCH,
+        random_fn: t.Callable[[int], int] | None = None
     ) -> None:
         """Creates a new TSID generator.
 
         Args:
         - `node` int | None: Node identifier. Defaults to a random integer
                              within the range of `node_bits`.
         - `node_bits` int:   Number of bytes used to repesent the node id.
                              Defaults to `TSID_DEFAULT_NODE_BITS`.
-        - `epoch` datetime:  Epoch start. Defaults to `TSID_EPOCH`.
+        - `epoch` int:       Epoch start in milliseconds. Defaults to
+                             `TSID_EPOCH`.
         - `random_fn`:       Function to use to randomize the counter.
-                             Must return a 32-bit integer. If None, the
-                             stdlib `random.random()` is used to return a
-                             random integer.
+                             Must return a n-bit integer. If None, the
+                             stdlib `random.getrandbits()` is used.
 
         >>> generator = TSIDGenerator(node=1, node_bits=21)
         Traceback (most recent call last):
         ...
         ValueError: Invalid node_bits: 21
 
         >>> generator = TSIDGenerator(node=1, node_bits=0)
@@ -355,40 +356,38 @@
         ...
         ValueError: Invalid node_bits: -1
 
         >>> generator = TSIDGenerator(node=1, node_bits=1)
         >>> generator.node
         1
         """
-
         if node is not None and node < 0:
             raise ValueError(f'Invalid node: {node}')
 
         if node_bits < 0 or node_bits > 20:
             raise ValueError(f'Invalid node_bits: {node_bits}')
 
-        self.random_fn = random_fn or (lambda: int(random() * 0xffffffff))
-
-        self.counter: int = self.random_fn()
+        self.random_fn = random_fn or random.getrandbits
 
         self.node: int
         if node is None:
-            self.node = int(random() * 0xffff) >> (20 - node_bits)
+            self.node = random.getrandbits(20) >> (20 - node_bits)
         else:
             self.node = node
 
         if self.node >> node_bits > 0:
             raise ValueError(f'Node {self.node} too large for '
                              f'node_bits=={node_bits}')
 
+        self._epoch: float = epoch
         self._node_bits: int = node_bits
         self._counter_bits: int = RANDOM_BITS - node_bits
+        self.counter: int = self.random_fn(self._counter_bits)
 
-        self.epoch: datetime = epoch or TSID_EPOCH
-        self._millis: float = datetime.now().timestamp() * 1000
+        self._millis: float = time.time() * 1000
         self._counter_mask: int = RANDOM_MASK >> node_bits
         self._node_mask: int = RANDOM_MASK >> self._counter_bits
 
         self._lock = threading.Lock()
 
     def create(self) -> TSID:
         """
@@ -403,52 +402,65 @@
         True
         >>> tc = TSIDGenerator(node=512, node_bits=10)
         >>> t = tc.create()
         >>> ((t.number & RANDOM_MASK) >> tc._counter_bits) == 512
         True
 
         >>> ### Test counter extraction ------------------------------
-        >>> tc = TSIDGenerator(node=64, node_bits=8, random_fn=lambda: 0)
+        >>> tc = TSIDGenerator(node=64, node_bits=8, random_fn=lambda n: 0)
         >>> t = tc.create()
         >>> t.number & tc._counter_mask == 1
         True
         >>> t = tc.create()
         >>> t.number & tc._counter_mask == 2
         True
 
         >>> ### Test random extraction ------------------------------
-        >>> tc = TSIDGenerator(node=0, node_bits=0, random_fn=lambda: 0)
+        >>> tc = TSIDGenerator(node=0, node_bits=0, random_fn=lambda n: 0)
         >>> t = tc.create()
         >>> t.random == 1
         True
         >>> t = tc.create()
         >>> t.random == 2
         True
 
-        >>> ### Test datetime extraction ------------------------------
+        >>> ### Test timestamp extraction ------------------------------
+        >>> t = tc.create()
+        >>> t.timestamp - (time.time() * 1000) <= 1
+        True
+
+        >>> ### Test custom epoch ------------------------------
         >>> from datetime import datetime
+        >>> UNIX_EPOCH = datetime.fromisoformat('1970-01-01 00:00:00+00:00')
+        >>> EPOCH_MS = UNIX_EPOCH.timestamp() * 1000
+        >>> now_without_unix_epoch: float = time.time() * 1000 - EPOCH_MS
+        >>> tc = TSIDGenerator(node=0, epoch=0)
         >>> t = tc.create()
-        >>> (t.datetime - datetime.now()).total_seconds() < 1
+        >>> t.timestamp - now_without_unix_epoch <= 1
         True
         """
         with self._lock:
-            current_millis: float = datetime.now().timestamp() * 1000
+            current_millis: float = time.time() * 1000
 
             # If same millisecond, increment counter
-            if int(current_millis) == int(self._millis):
+            if current_millis - self._millis < 1:
                 self.counter += 1
 
                 # If the counter overflows, go to the next millisecond
                 if self.counter >> self._counter_bits != 0:
                     self._millis += 1
                     self.counter = 0
             else:
                 self._millis = current_millis
-                self.counter = self.random_fn() & self._counter_mask
+                rnd: int = self.random_fn(self._counter_bits)
+                self.counter = rnd & self._counter_mask
 
-            millis = int(self._millis - _TSID_EPOCH_MILLIS) << RANDOM_BITS
+            millis = int(self._millis - self._epoch) << RANDOM_BITS
             node = (self.node & self._node_mask) << self._counter_bits
             counter = self.counter & self._counter_mask
-            return TSID(millis + node + counter)
+
+            result = TSID(millis + node + counter)
+            result._epoch = self._epoch
+            return result
 
 
 _default_generator = TSIDGenerator(node_bits=0)
```

### Comparing `tsidpy-1.0.0.5/src/tsidpy.egg-info/PKG-INFO` & `tsidpy-1.1.0.0/src/tsidpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsidpy
-Version: 1.0.0.5
+Version: 1.1.0.0
 Summary: A Python library for generating Time-Sorted Unique Identifiers (TSID)
 Author-email: Luis Medel <luis@luismedel.com>
 Project-URL: Homepage, https://github.com/luismedel/tsid-python
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -235,19 +235,19 @@
 ```python
 >>> tsid.to_string('s')
 '0123456789abc'
 ```
 
 ---
 
-Get the creation `datetime` of a TSID:
+Get the creation `timestamp` of a TSID:
 
 ```python
->>> tsid.datetime
-datetime.datetime(2023, 4, 8, 12, 6, 58, 241000)
+>>> tsid.timestamp
+1680948418241.0  # datetime.datetime(2023, 4, 8, 12, 6, 58, 241000)
 ```
 
 ---
 
 Encode a TSID to base-62:
 
 ```python
@@ -268,16 +268,16 @@
 
 datacenter: int = 1
 worker: int = 1
 node: int = datacenter << 5 | worker
 epoch: datetime = datetime.fromisoformat('2010-11-04T01:42:54.657Z')
 
 twitter_generator: TSIDGenerator = TSIDGenerator(node=node, node_bits=10,
-                                                 epoch=epoch,
-                                                 random_fn=lambda: 0)
+                                                 epoch=epoch.timestamp() * 1000,
+                                                 random_fn=lambda n: 0)
 
 # use the generator
 tsid: TSID = twitter_generator.create()
 ```
 
 ---
 
@@ -292,15 +292,15 @@
 
 worker: int = 1
 process: int = 1
 node: int = worker << 5 | process
 epoch: datetime = datetime.fromisoformat("2015-01-01T00:00:00.000Z")
 
 discord_generator: TSIDGenerator = TSIDGenerator(node=node, node_bits=10,
-                                                 epoch=epoch)
+                                                 epoch=epoch.timestamp() * 1000)
 
 # use the generator
 tsid: TSID = discord_generator.create()
 ```
 
 ---
 
@@ -337,14 +337,15 @@
 
 ## Other ports, forks and OSS
 
 ### Ports and forks
 
 | Language | Name |
 | -------- | ---- |
+| Java (by original author)     | [f4b6a3/tsid-creator](https://github.com/f4b6a3/tsid-creator) |
 | Java     | [vladmihalcea/hypersistence-tsid](https://github.com/vladmihalcea/hypersistence-tsid) |
 | .NET     | [kgkoutis/TSID.Creator.NET](https://github.com/kgkoutis/TSID.Creator.NET) |
 | PHP      | [odan/tsid](https://github.com/odan/tsid) |
 
 ### OSS
 
 | Language | Name |
```

