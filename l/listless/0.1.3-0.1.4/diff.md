# Comparing `tmp/listless-0.1.3.tar.gz` & `tmp/listless-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "listless-0.1.3.tar", max compression
+gzip compressed data, was "listless-0.1.4.tar", max compression
```

## Comparing `listless-0.1.3.tar` & `listless-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.425545 listless-0.1.3/LICENSE
--rw-r--r--   0        0        0    19036 2023-03-02 16:13:30.455324 listless-0.1.3/listless/__init__.py
--rw-r--r--   0        0        0      237 2022-02-10 17:32:26.246958 listless-0.1.3/listless/__main__.py
--rw-r--r--   0        0        0      209 2023-03-02 16:15:00.368307 listless-0.1.3/listless/_meta.py
--rw-r--r--   0        0        0        0 2022-02-01 22:06:04.830952 listless-0.1.3/listless/py.typed
--rw-r--r--   0        0        0     2112 2023-03-02 16:14:31.318976 listless-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      816 2022-05-03 21:42:21.354967 listless-0.1.3/README.md
--rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 listless-0.1.3/setup.py
--rw-r--r--   0        0        0     1957 1970-01-01 00:00:00.000000 listless-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1056 2022-02-11 23:27:58.165586 listless-0.1.4/LICENSE
+-rw-r--r--   0        0        0    19482 2023-04-11 21:27:29.161305 listless-0.1.4/listless/__init__.py
+-rw-r--r--   0        0        0      381 2023-04-11 21:27:29.161305 listless-0.1.4/listless/__main__.py
+-rw-r--r--   0        0        0      209 2023-04-11 21:27:29.162305 listless-0.1.4/listless/_meta.py
+-rw-r--r--   0        0        0        0 2022-02-01 20:37:20.181695 listless-0.1.4/listless/py.typed
+-rw-r--r--   0        0        0     2156 2023-04-11 21:27:29.162305 listless-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      816 2022-06-02 17:33:59.763392 listless-0.1.4/README.md
+-rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 listless-0.1.4/PKG-INFO
```

### Comparing `listless-0.1.3/LICENSE` & `listless-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `listless-0.1.3/listless/__init__.py` & `listless-0.1.4/listless/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # pyright: reportInvalidTypeVarUse=false
 """Listless generator utils"""
 import asyncio
 
 from collections import deque
 from functools import reduce
-from itertools import count, islice, tee, zip_longest
+from itertools import chain, count, islice, tee, zip_longest
 from operator import iconcat, mul
 from typing import (
     Any,
     AsyncIterable,
     AsyncIterator,
     Callable,
     Deque,
@@ -120,15 +120,14 @@
 
 def partition(
     it: Sequence[_T],
     n: int,
     *,
     pad: bool = False,
     padval: Any = None,
-    zip_strict: bool = False,
 ) -> Iterable[Sequence[_T]]:
     """Partition an iterable into chunks of size n
 
     Args:
         it: Iterable to partition
         n (int): Size of the partition chunks
         pad (bool): Pad parts with padval if True, else do not pad
@@ -186,15 +185,21 @@
     if pad:
         return zip_longest(*args, fillvalue=padval)
     else:
         return zip(*args)
 
 
 def nyield(it: Sequence[_T], n: int) -> Iterable[_T]:
-    """Yield the first n items of an iterable"""
+    """Yield the first n items of an iterable
+
+    Examples:
+        >>> list(nyield([1, 2, 3, 4, 5, 6], 3))
+        [1, 2, 3]
+
+    """
     return islice(it, n)
 
 
 def is_sequence(seq: Any) -> bool:
     """Check if an object is a sequence
 
     Examples:
@@ -276,15 +281,21 @@
             _chunk = tuple(islice(it, chunk_size))
             if not _chunk:
                 break
             yield _chunk
 
 
 def chunk(it: Sequence[_T], n: int) -> Iterable[Sequence[_T]]:
-    """Yield chunks of size n from a Sequence"""
+    """Yield chunks of size n from a Sequence
+
+    Examples:
+        >>> list(chunk([1, 2, 3, 4, 5, 6], 3))
+        [[1, 2, 3], [4, 5, 6]]
+
+    """
     return chunks(it, n)
 
 
 def exhaust(it: Iterable[_T], *, maxlen: Optional[int] = 0) -> Deque[_T]:
     """Exhaust an interable; useful for evaluating a map object.
 
     Args:
@@ -318,14 +329,15 @@
     func: Callable[[_T], _R], it: Iterable[_T], *, maxlen: Optional[int] = 0
 ) -> Deque[_R]:
     """Apply a function to each element of an iterable immediately
 
     Args:
         func: Function to apply to each element
         it: iterable to apply func to
+        maxlen: Maximum length of the deque; if 0, deque is unbounded
 
     Returns:
         Deque of the possible results if maxlen is greater than 0
 
     Examples:
         >>> xmap(lambda x: x*2, list(range(1, 7)))
         deque([], maxlen=0)
@@ -416,68 +428,68 @@
         [-1, 0, 1, '', 's', [], ['s'], {}]
 
 
     """
     return filter(None.__ne__, it)  # type: ignore[arg-type]
 
 
-def flatten(*args: Union[_T, List[_T], Tuple[_T, ...]]) -> List[_T]:
+def flatten(*args: Union[_T, Iterable[_T]], anystr: bool = False) -> Iterable[_T]:
     """Flatten possibly nested iterables of sequences to a flat list
 
     Examples:
         >>> list(flatten("cmd", ["uno", "dos", "tres"]))
         ['cmd', 'uno', 'dos', 'tres']
         >>> list(flatten("cmd", ["uno", "dos", "tres", ["4444", "five"]]))
         ['cmd', 'uno', 'dos', 'tres', '4444', 'five']
 
     """
+    return chain(
+        *(flatten(*arg) if isinstance(arg, (list, tuple)) else (arg,) for arg in args)
+    )
+
+
+def flatten_seq(*args: Union[_T, Sequence[_T]], anystr: bool = False) -> Iterable[_T]:
+    """Flatten possibly nested iterables of sequences to a flat list
+
+    Examples:
+        >>> list(flatten_seq("cmd", ["uno", "dos", "tres"]))
+        ['cmd', 'uno', 'dos', 'tres']
+        >>> list(flatten_seq("cmd", ["uno", "dos", "tres", ["4444", "five"]]))
+        ['cmd', 'uno', 'dos', 'tres', '4444', 'five']
+
+    """
     return list(
         reduce(
             iconcat,
             [
-                flatten(*arg) if isinstance(arg, (list, tuple)) else (arg,)
+                flatten_seq(*arg) if isinstance(arg, (list, tuple)) else (arg,)
                 for arg in args
             ],
             [],
         )
     )
 
 
 def flatten_strings(
     *args: Union[
-        Sequence[Union[str, int, float]],
-        str,
-        int,
-        float,
+        _T,
+        Iterable[_T],
     ]
-) -> List[str]:
+) -> Iterable[str]:
     """Flatten possibly nested iterables of sequences to a list of strings
 
     Examples:
         >>> from listless import flatten_strings
         >>> list(flatten_strings("cmd", ["uno", "dos", "tres"]))
         ['cmd', 'uno', 'dos', 'tres']
-        >>> list(flatten_strings("cmd", ["uno", "dos", "tres", ["4444", "five"]]))
-        ['cmd', 'uno', 'dos', 'tres', '4444', 'five']
+        >>> list(flatten_strings("cmd", ["uno", "dos", "tres", ["4444", "five", 123]]))
+        ['cmd', 'uno', 'dos', 'tres', '4444', 'five', '123']
 
     """
-    return list(
-        reduce(
-            iconcat,
-            [
-                flatten_strings(*arg)
-                if isinstance(arg, (list, tuple))
-                else (str(arg),)
-                if isinstance(arg, (int, float))
-                else (arg,)
-                for arg in args
-            ],
-            [],
-        )
-    )
+    return (str(arg) for arg in flatten(*args))
 
 
 def itlen(iterable: Iterable[Any], unique: bool = False) -> int:
     """Return the length/num-items in an iterable
 
     This consumes the iterable.
```

### Comparing `listless-0.1.3/pyproject.toml` & `listless-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "listless"
-version = "0.1.3"
+version = "0.1.4"
 description = "generator utils; aka listless"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/listless"
 readme = 'README.md'
 packages = [
@@ -15,28 +15,29 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
 ]
 keywords = [
   "generators",
   "itertools",
   "dgpy",
   "typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.1"
+pytest = "^7.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
```

### Comparing `listless-0.1.3/README.md` & `listless-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `listless-0.1.3/PKG-INFO` & `listless-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: listless
-Version: 0.1.3
+Version: 0.1.4
 Summary: generator utils; aka listless
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/listless
 License: MIT
 Keywords: generators,itertools,dgpy,typed
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: listless Version: 0.1.3 Summary: generator utils;
+Metadata-Version: 2.1 Name: listless Version: 0.1.4 Summary: generator utils;
 aka listless Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/
 main/libs/listless License: MIT Keywords: generators,itertools,dgpy,typed
 Author: jesse Author-email: jesse@dgi.com Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Typing :: Typed Project-URL: Repository, https://
-github.com/dynamic-graphics-inc/dgpy-libs Description-Content-Type: text/
-markdown [drawing] # listless [![Wheel](https://img.shields.io/pypi/wheel/
-listless.svg)](https://img.shields.io/pypi/wheel/listless.svg) [![Version]
-(https://img.shields.io/pypi/v/listless.svg)](https://img.shields.io/pypi/v/
-listless.svg) [![py_versions](https://img.shields.io/pypi/pyversions/
-listless.svg)](https://img.shields.io/pypi/pyversions/listless.svg) [![Code
-style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
-(https://github.com/psf/black) **Install:** `pip install listless` OR `poetry
-add listless` **What:** typed & tested python itertools/generators-utils
-library
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Typing :: Typed Project-URL: Repository, https://github.com/dynamic-graphics-
+inc/dgpy-libs Description-Content-Type: text/markdown [drawing] # listless [!
+[Wheel](https://img.shields.io/pypi/wheel/listless.svg)](https://
+img.shields.io/pypi/wheel/listless.svg) [![Version](https://img.shields.io/
+pypi/v/listless.svg)](https://img.shields.io/pypi/v/listless.svg) [!
+[py_versions](https://img.shields.io/pypi/pyversions/listless.svg)](https://
+img.shields.io/pypi/pyversions/listless.svg) [![Code style: black](https://
+img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
+black) **Install:** `pip install listless` OR `poetry add listless` **What:**
+typed & tested python itertools/generators-utils library
```

