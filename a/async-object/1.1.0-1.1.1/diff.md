# Comparing `tmp/async-object-1.1.0.tar.gz` & `tmp/async-object-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async-object-1.1.0.tar", last modified: Mon Jan  2 06:21:27 2023, max compression
+gzip compressed data, was "async-object-1.1.1.tar", last modified: Tue Apr 11 21:22:01 2023, max compression
```

## Comparing `async-object-1.1.0.tar` & `async-object-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      366 2023-01-02 06:21:27.000000 async-object-1.1.0/.flake8
--rw-r--r--   0        0        0     1097 2023-01-02 06:21:27.000000 async-object-1.1.0/LICENSE
--rw-r--r--   0        0        0     3189 2023-01-02 06:21:27.000000 async-object-1.1.0/README.md
--rw-r--r--   0        0        0     2329 2023-01-02 06:21:27.000000 async-object-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4576 2023-01-02 06:21:27.000000 async-object-1.1.0/src/async_object/__init__.py
--rw-r--r--   0        0        0        0 2023-01-02 06:21:27.000000 async-object-1.1.0/src/async_object/py.typed
--rw-r--r--   0        0        0     4109 1970-01-01 00:00:00.000000 async-object-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      366 2023-04-11 21:22:01.000000 async-object-1.1.1/.flake8
+-rw-r--r--   0        0        0     1097 2023-04-11 21:22:01.000000 async-object-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5447 2023-04-11 21:22:01.000000 async-object-1.1.1/README.md
+-rw-r--r--   0        0        0     2367 2023-04-11 21:22:01.000000 async-object-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4522 2023-04-11 21:22:01.000000 async-object-1.1.1/src/async_object/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 21:22:01.000000 async-object-1.1.1/src/async_object/py.typed
+-rw-r--r--   0        0        0     6396 1970-01-01 00:00:00.000000 async-object-1.1.1/PKG-INFO
```

### Comparing `async-object-1.1.0/LICENSE` & `async-object-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async-object-1.1.0/pyproject.toml` & `async-object-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 
 [project]
 name = "async-object"
 authors = [{name = "FrankySnow9", email = "clairicia.rcj.francis@gmail.com"}]
 requires-python = ">=3.8"
 readme = "README.md"
 license = {file = "LICENSE"}
-dependencies = [
-
-]
+dependencies = []
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
@@ -22,14 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Typing :: Typed"
 ]
 dynamic = ["version", "description"]
+keywords = ["async", "init", "asyncio"]
 
 [project.urls]
 Home = "https://github.com/francis-clairicia/async-object"
 
 ############################ Flit configuration ############################
 [tool.flit.sdist]
 include = [
```

### Comparing `async-object-1.1.0/src/async_object/__init__.py` & `async-object-1.1.1/src/async_object/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,27 +16,28 @@
 __copyright__ = "Copyright (c) 2023, Francis Clairicia-Rose-Claire-Josephine"
 __credits__ = ["FrankySnow9"]
 __deprecated__ = False
 __email__ = "clairicia.rcj.francis@gmail.com"
 __license__ = "MIT"
 __maintainer__ = "FrankySnow9"
 __status__ = "Production"
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 import abc
 import inspect
 from functools import partialmethod
-from typing import TYPE_CHECKING, Any, Callable, Generator, TypeVar
+from typing import TYPE_CHECKING, Any, Callable, Generator, TypeVar, final
 
 
 def _validate_constructor(func: Any, name: str) -> None:
     if isinstance(func, (staticmethod, classmethod)):
-        func = func.__func__
-    elif isinstance(func, partialmethod):
-        func = func.func
+        return _validate_constructor(func.__func__, name)
+    if isinstance(func, partialmethod):  # pragma: no cover
+        return _validate_constructor(func.func, name)
+
     if not inspect.iscoroutinefunction(func):
         raise TypeError(f"{name!r} must be a coroutine function (using 'async def')")
 
 
 class AsyncObjectMeta(type):
     if TYPE_CHECKING:
         __Self = TypeVar("__Self", bound="AsyncObjectMeta")
@@ -55,25 +56,23 @@
             if name == "AsyncObject" and namespace.get("__module__") == __name__:
                 return super().__new__(mcs, name, bases, namespace, **kwargs)
             raise
 
         if "__await__" in namespace:
             raise TypeError("__await__() cannot be overriden")
 
-        if not bases:
-            raise TypeError(f"{name} must explicitly derive from {absolute_base_class.__name__}")
         if not any(issubclass(b, absolute_base_class) for b in bases):
-            raise TypeError(f"All base classes must be a subclass of {absolute_base_class.__name__}")
+            raise TypeError(f"{name} must explicitly derive from {absolute_base_class.__name__}")
         if invalid_bases := [
             b.__name__
             for b in bases
             if not issubclass(b, absolute_base_class) and (b.__new__ is not object.__new__ or b.__init__ is not object.__init__)
         ]:
             raise TypeError(
-                f"These non-async base classes defines a custom __new__ or __init__: {', '.join(map(repr, invalid_bases))}"
+                f"These non-async base classes define a custom __new__ or __init__: {', '.join(map(repr, invalid_bases))}"
             )
         return super().__new__(mcs, name, bases, namespace, **kwargs)
 
     def __setattr__(cls, name: str, value: Any, /) -> None:
         if cls is AsyncObject:
             raise AttributeError("AsyncObject is immutable")
         if name == "__await__":
@@ -110,18 +109,17 @@
     async def __new__(cls: type[__Self]) -> __Self:  # type: ignore[misc]
         return object.__new__(cls)
 
     async def __init__(self) -> None:  # type: ignore[misc]
         pass
 
     if TYPE_CHECKING:
-
-        # Static type checkers like mypy think 'await AsyncObject()' is
-        # 'await instanciated object'
-        def __await__(self: __Self) -> Generator[Any, None, __Self]:
+        # mypy think 'await AsyncObject()' is 'await (already instanciated object)'
+        @final
+        def __await__(self: __Self) -> Generator[Any, Any, __Self]:
             ...
 
 
 class AsyncABCMeta(AsyncObjectMeta, abc.ABCMeta):
     pass
```

### Comparing `async-object-1.1.0/PKG-INFO` & `async-object-1.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: async-object
-Version: 1.1.0
+Version: 1.1.1
 Summary: async-object let you write classes with async def __init__.
+Keywords: async,init,asyncio
 Author-email: FrankySnow9 <clairicia.rcj.francis@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +32,15 @@
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 `async-object` let you write classes with `async def __init__`
 
 ## Usage
-It is simple, with `async-object` you can do this :
+It is simple, with `async-object` you can do this:
 ```py
 from async_object import AsyncObject
 
 
 class MyObject(AsyncObject):
     async def __new__(cls) -> "MyObject":
         self = await super().__new__(cls)
@@ -60,15 +61,81 @@
     async def main() -> None:
         instance = await MyObject()
         assert isinstance(instance, MyObject)
 
     asyncio.run(main())
 ```
 
+This example uses `asyncio`, but it is compatible with all runner libraries, since this package only uses the language syntax.
+
+## Description
+`async-object` provides a base class `AsyncObject` using `AsyncObjectMeta` metaclass.
+
+`AsyncObjectMeta` overrides the default `type` constructor in order to return a coroutine, which must be `await`-ed to get the instance.
+
+```py
+async def main() -> None:
+    coroutine = MyObject()
+    print(coroutine)
+    instance = await coroutine
+    print(instance)
+```
+
+Replace the `main` in the [Usage](#usage) example by this one and run it. You should see something like this in your console:
+```
+<coroutine object AsyncObjectMeta.__call__ at 0x7ff1f28eb300>
+<__main__.MyObject object at 0x7ff1f21a4fd0>
+```
+
+### Arguments
+Obviously, arguments can be given to `__init__` and `__new__`.
+The inheritance logic with "normal" constructors is the same here:
+```py
+class MyObjectOnlyNew(AsyncObject):
+    async def __new__(cls, *args: Any, **kwargs: Any) -> "MyObject":
+        self = await super().__new__(cls)
+
+        print(args)
+        print(kwargs)
+
+        return self
+
+
+class MyObjectOnlyInit(AsyncObject):
+    async def __init__(self, *args: Any, **kwargs: Any) -> None:
+        await super().__init__()
+
+        print(args)
+        print(kwargs)
+
+
+class MyObjectBothNewAndInit(AsyncObject):
+    async def __new__(cls, *args: Any, **kwargs: Any) -> "MyObject":
+        self = await super().__new__(cls)
+
+        print(args)
+        print(kwargs)
+
+        return self
+
+    async def __init__(self, *args: Any, **kwargs: Any) -> None:
+        await super().__init__()
+
+        print(args)
+        print(kwargs)
+```
+
+### Inheritance
+Talking about inheritance, there are a few rules to follow:
+- `AsyncObject` or a subclass must appear at least once in the base classes declaration.
+- Non-`AsyncObject` classes can be used as base classes if they do not override `__new__` or `__init__` (in order not to break the [MRO](https://docs.python.org/3/glossary.html#term-method-resolution-order)).
+- To avoid confusion with [awaitable objects](https://docs.python.org/3/glossary.html#term-awaitable), overriding `__await__` is forbidden.
+
 ### Abstract base classes
+There is a metaclass `AsyncABCMeta` deriving from `AsyncObjectMeta` and `abc.ABCMeta` which allows you to declare abstract base classes
 ```py
 import abc
 
 from async_object import AsyncObject, AsyncABCMeta
 
 
 class MyAbstractObject(AsyncObject, metaclass=AsyncABCMeta):
@@ -78,15 +145,15 @@
 
     @abc.abstractmethod
     async def async_method(self) -> None:
         raise NotImplementedError
 
 
 class MyObject(MyAbstractObject):
-    async def __init__(self, arg1: int, arg2: str) -> None:
+    async def __init__(self) -> None:
         await super().__init__()
 
     def method(self) -> None:
         pass
 
     async def async_method(self) -> None:
         pass
@@ -109,15 +176,15 @@
         raise NotImplementedError
 ```
 
 ## Troubleshoots
 
 ### Static type checking
 
-Static type checkers like `mypy` do not like having `async def` for `__new__` and `__init__`. You can use `# type: ignore[misc]` comment to mask these errors when overriding these methods.
+`mypy` does not like having `async def` for `__new__` and `__init__`. You can use `# type: ignore[misc]` comment to mask these errors when overriding these methods.
 ```py
 class MyObject(AsyncObject):
     async def __new__(cls) -> "MyObject":  # type: ignore[misc]
         return await super().__new__(cls)
 
     async def __init__(self) -> None:  # type: ignore[misc]
         await super().__init__()
```

