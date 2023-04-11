# Comparing `tmp/tarina-0.1.2.tar.gz` & `tmp/tarina-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarina-0.1.2.tar", last modified: Sat Apr  8 11:38:36 2023, max compression
+gzip compressed data, was "tarina-0.2.1.tar", last modified: Tue Apr 11 12:28:17 2023, max compression
```

## Comparing `tarina-0.1.2.tar` & `tarina-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,33 @@
--rw-r--r--   0        0        0     1084 2023-03-31 17:52:21.141288 tarina-0.1.2/LICENSE
--rw-r--r--   0        0        0      612 2023-04-08 11:38:09.521232 tarina-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      260 2023-03-31 18:46:25.479039 tarina-0.1.2/README.md
--rw-r--r--   0        0        0      333 2023-04-08 06:09:34.164271 tarina-0.1.2/tarina/__init__.py
--rw-r--r--   0        0        0       51 2023-03-31 18:04:27.301935 tarina-0.1.2/tarina/const.py
--rw-r--r--   0        0        0      748 2023-03-31 18:04:27.273976 tarina-0.1.2/tarina/context.py
--rw-r--r--   0        0        0     3086 2023-03-31 18:39:45.584975 tarina-0.1.2/tarina/generic.py
--rw-r--r--   0        0        0      611 2023-03-31 18:15:19.556651 tarina-0.1.2/tarina/guard.py
--rw-r--r--   0        0        0     3210 2023-04-08 11:28:51.693384 tarina-0.1.2/tarina/lru.py
--rw-r--r--   0        0        0     1787 2023-04-08 11:25:25.420295 tarina-0.1.2/tarina/lru.pyi
--rw-r--r--   0        0        0     2451 2023-03-31 18:35:50.245999 tarina-0.1.2/tarina/signature.py
--rw-r--r--   0        0        0     1936 2023-03-31 18:29:53.375743 tarina-0.1.2/tarina/tools.py
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 tarina-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:17.486463 tarina-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 12:28:01.000000 tarina-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-11 12:28:01.000000 tarina-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 12:28:17.486463 tarina-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-11 12:28:01.000000 tarina-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-11 12:28:01.000000 tarina-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 12:28:17.486463 tarina-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-11 12:28:01.000000 tarina-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:17.482463 tarina-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:17.482463 tarina-0.2.1/src/tarina/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23032 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_lru_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_lru_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_lru_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)   195090 2023-04-11 12:28:08.000000 tarina-0.2.1/src/tarina/_string_c.c
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_string_c.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_string_c.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/_string_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/guard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/lru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/lru.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-11 12:28:01.000000 tarina-0.2.1/src/tarina/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 12:28:17.486463 tarina-0.2.1/src/tarina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 12:28:17.000000 tarina-0.2.1/src/tarina.egg-info/top_level.txt
```

### Comparing `tarina-0.1.2/LICENSE` & `tarina-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 ARCLET
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 ARCLET
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tarina-0.1.2/tarina/context.py` & `tarina-0.2.1/src/tarina/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from __future__ import annotations
-
-from contextlib import contextmanager
-from contextvars import ContextVar, Token
-from typing import Generic, TypeVar
-
-T = TypeVar("T")
-D = TypeVar("D")
-
-class ContextModel(Generic[T]):
-    current_ctx: ContextVar[T]
-
-    def __init__(self, name: str) -> None:
-        self.current_ctx = ContextVar(name)
-
-    def get(self, default: T | D | None = None) -> T | D:
-        return self.current_ctx.get(default)
-
-    def set(self, value: T):
-        return self.current_ctx.set(value)
-
-    def reset(self, token: Token):
-        return self.current_ctx.reset(token)
-
-    @contextmanager
-    def use(self, value: T):
-        token = self.set(value)
-        yield
-        self.reset(token)
+from __future__ import annotations
+
+from contextlib import contextmanager
+from contextvars import ContextVar, Token
+from typing import Generic, TypeVar
+
+T = TypeVar("T")
+D = TypeVar("D")
+
+
+class ContextModel(Generic[T]):
+    current_ctx: ContextVar[T]
+
+    def __init__(self, name: str) -> None:
+        self.current_ctx = ContextVar(name)
+
+    def get(self, default: T | D | None = None) -> T | D:
+        return self.current_ctx.get(default)
+
+    def set(self, value: T):
+        return self.current_ctx.set(value)
+
+    def reset(self, token: Token):
+        return self.current_ctx.reset(token)
+
+    @contextmanager
+    def use(self, value: T):
+        token = self.set(value)
+        yield
+        self.reset(token)
```

### Comparing `tarina-0.1.2/tarina/generic.py` & `tarina-0.2.1/src/tarina/generic.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,82 @@
-from __future__ import annotations
-
-import contextlib
-import sys
-import types
-from typing import Any, List, TypeVar, Literal, Union, TYPE_CHECKING
-
-from typing_extensions import Annotated, get_args, get_origin as typing_ext_get_origin
-
-if TYPE_CHECKING:
-    from types import GenericAlias  # noqa
-else:
-    GenericAlias: type = type(List[int])
-
-AnnotatedType: type = type(Annotated[int, lambda x: x > 0])
-Unions = (Union, types.UnionType) if sys.version_info >= (3, 10) else (Union,)  # pragma: no cover
-
-
-def get_origin(obj: Any) -> Any:
-    return typing_ext_get_origin(obj) or obj
-
-
-def generic_isinstance(obj: Any, par: type | Any | tuple[type, ...]) -> bool:
-    """检查 obj 是否是 args 中的一个类型, 支持泛型, Any, Union
-    Args:
-        obj (Any): 要检查的对象
-        par (Union[type, Any, Tuple[type, ...]]): 要检查的对象的类型
-    Returns:
-        bool: 是否是类型
-    """
-    if par is Any:
-        return True
-    with contextlib.suppress(TypeError):
-        if isinstance(par, AnnotatedType):
-            return generic_isinstance(obj, get_args(par)[0])
-        if isinstance(par, type):
-            return isinstance(obj, par)
-        if get_origin(par) is Literal:
-            return obj in get_args(par)
-        if get_origin(par) in Unions:  # pragma: no cover
-            return any(generic_isinstance(obj, p) for p in get_args(par))
-        if isinstance(par, TypeVar):  # pragma: no cover
-            if par.__constraints__:
-                return any(generic_isinstance(obj, p) for p in par.__constraints__)
-            return generic_isinstance(obj, par.__bound__) if par.__bound__ else True
-        if isinstance(par, tuple):
-            return any(generic_isinstance(obj, p) for p in par)
-        if isinstance(obj, get_origin(par)):  # type: ignore
-            return True
-    return False
-
-
-def generic_issubclass(cls: type, par: Union[type, Any, tuple[type, ...]]) -> bool:
-    """检查 cls 是否是 args 中的一个子类, 支持泛型, Any, Union
-    Args:
-        cls (type): 要检查的类
-        par (Union[type, Any, Tuple[type, ...]]): 要检查的类的父类
-    Returns:
-        bool: 是否是父类
-    """
-    if par is Any:
-        return True
-    with contextlib.suppress(TypeError):
-        if isinstance(par, AnnotatedType):
-            return generic_issubclass(cls, get_args(par)[0])
-        if isinstance(par, type):
-            return issubclass(cls, par)
-        if get_origin(par) in Unions:
-            return any(generic_issubclass(cls, p) for p in get_args(par))
-        if isinstance(par, TypeVar):
-            if par.__constraints__:
-                return any(generic_issubclass(cls, p) for p in par.__constraints__)
-            if par.__bound__:
-                return generic_issubclass(cls, par.__bound__)
-        if isinstance(par, tuple):
-            return any(generic_issubclass(cls, p) for p in par)
-        if issubclass(cls, get_origin(par)):  # type: ignore
-            return True
-    return False
+from __future__ import annotations
+
+import contextlib
+import sys
+import types
+from typing import TYPE_CHECKING, Any, List, Literal, TypeVar, Union
+
+from typing_extensions import Annotated, get_args
+from typing_extensions import get_origin as typing_ext_get_origin
+
+if TYPE_CHECKING:
+    from types import GenericAlias  # noqa
+else:
+    GenericAlias: type = type(List[int])
+
+AnnotatedType: type = type(Annotated[int, lambda x: x > 0])
+Unions = (
+    (Union, types.UnionType) if sys.version_info >= (3, 10) else (Union,)  # pragma: no cover
+)
+
+
+def get_origin(obj: Any) -> Any:
+    return typing_ext_get_origin(obj) or obj
+
+
+def generic_isinstance(obj: Any, par: type | Any | tuple[type, ...]) -> bool:
+    """检查 obj 是否是 args 中的一个类型, 支持泛型, Any, Union
+    Args:
+        obj (Any): 要检查的对象
+        par (Union[type, Any, Tuple[type, ...]]): 要检查的对象的类型
+    Returns:
+        bool: 是否是类型
+    """
+    if par is Any:
+        return True
+    with contextlib.suppress(TypeError):
+        if isinstance(par, AnnotatedType):
+            return generic_isinstance(obj, get_args(par)[0])
+        if isinstance(par, type):
+            return isinstance(obj, par)
+        if get_origin(par) is Literal:
+            return obj in get_args(par)
+        if get_origin(par) in Unions:  # pragma: no cover
+            return any(generic_isinstance(obj, p) for p in get_args(par))
+        if isinstance(par, TypeVar):  # pragma: no cover
+            if par.__constraints__:
+                return any(generic_isinstance(obj, p) for p in par.__constraints__)
+            return generic_isinstance(obj, par.__bound__) if par.__bound__ else True
+        if isinstance(par, tuple):
+            return any(generic_isinstance(obj, p) for p in par)
+        if isinstance(obj, get_origin(par)):  # type: ignore
+            return True
+    return False
+
+
+def generic_issubclass(cls: type, par: Union[type, Any, tuple[type, ...]]) -> bool:
+    """检查 cls 是否是 args 中的一个子类, 支持泛型, Any, Union
+    Args:
+        cls (type): 要检查的类
+        par (Union[type, Any, Tuple[type, ...]]): 要检查的类的父类
+    Returns:
+        bool: 是否是父类
+    """
+    if par is Any:
+        return True
+    with contextlib.suppress(TypeError):
+        if isinstance(par, AnnotatedType):
+            return generic_issubclass(cls, get_args(par)[0])
+        if isinstance(par, type):
+            return issubclass(cls, par)
+        if get_origin(par) in Unions:
+            return any(generic_issubclass(cls, p) for p in get_args(par))
+        if isinstance(par, TypeVar):
+            if par.__constraints__:
+                return any(generic_issubclass(cls, p) for p in par.__constraints__)
+            if par.__bound__:
+                return generic_issubclass(cls, par.__bound__)
+        if isinstance(par, tuple):
+            return any(generic_issubclass(cls, p) for p in par)
+        if issubclass(cls, get_origin(par)):  # type: ignore
+            return True
+    return False
```

### Comparing `tarina-0.1.2/tarina/lru.pyi` & `tarina-0.2.1/src/tarina/_lru_c.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-from typing import (
-    Any,
-    Callable,
-    Generic,
-    Hashable,
-    Iterable,
-    TypeVar,
-    overload,
-)
-
-_KT = TypeVar("_KT", bound=Hashable)
-_VT = TypeVar("_VT")
-_T = TypeVar("_T")
-
-class LRU(Generic[_KT, _VT]):
-    __slots__ = ("__max", "__cache", "__size", "__callback")
-
-    def __init__(
-        self, size: int, callback: Callable[[_KT, _VT], Any] | None = ...
-    ) -> None: ...
-    def clear(self) -> None: ...
-    def get(self, __key: _KT, default: _VT | _T) -> _VT | _T: ...
-    def has_key(self, key: _KT) -> bool: ...
-    def keys(self) -> list[_KT]: ...
-    def values(self) -> list[_VT]: ...
-    def items(self, size: int = -1) -> list[tuple[_KT, _VT]]: ...
-    def peek_first_item(self) -> tuple[_KT, _VT] | None: ...
-    def peek_last_item(self) -> tuple[_KT, _VT] | None: ...
-    @overload
-    def pop(self, __key: _KT) -> _VT: ...
-    @overload
-    def pop(self, __key: _KT, default: _VT | _T) -> _VT | _T: ...
-    def popitem(self, least_recent: bool = ...) -> tuple[_KT, _VT]: ...
-    @overload
-    def setdefault(self: LRU[_KT, _T | None], __key: _KT) -> _T | None: ...
-    @overload
-    def setdefault(self, __key: _KT, __default: _VT) -> _VT: ...
-    def set_callback(self, callback: Callable[[_KT, _VT], Any]) -> None: ...
-    def set_size(self, size: int) -> None: ...
-    @overload
-    def update(self, __m: Iterable[tuple[_KT, _VT]], **kwargs: _VT) -> None: ...
-    @overload
-    def update(self, **kwargs: _VT) -> None: ...
-    def __contains__(self, __o: Any) -> bool: ...
-    def __delitem__(self, __v: _KT) -> None: ...
-    def __getitem__(self, item: _KT) -> _VT: ...
-    def __len__(self) -> int: ...
-    def __repr__(self) -> str: ...
-    def __setitem__(self, __k: _KT, __v: _VT) -> None: ...
+from typing import (
+    Any,
+    Callable,
+    Generic,
+    Hashable,
+    Iterable,
+    TypeVar,
+    overload,
+)
+
+_KT = TypeVar("_KT", bound=Hashable)
+_VT = TypeVar("_VT")
+_T = TypeVar("_T")
+
+class LRU(Generic[_KT, _VT]):
+
+    def __init__(
+        self, size: int, callback: Callable[[_KT, _VT], Any] | None = ...
+    ) -> None: ...
+    def clear(self) -> None: ...
+    def get(self, key: _KT, default: _VT | _T) -> _VT | _T: ...
+
+    def get_size(self) -> int: ...
+    def has_key(self, key: _KT) -> bool: ...
+    def keys(self) -> list[_KT]: ...
+    def values(self) -> list[_VT]: ...
+    def items(self) -> list[tuple[_KT, _VT]]: ...
+    def peek_first_item(self) -> tuple[_KT, _VT] | None: ...
+    def peek_last_item(self) -> tuple[_KT, _VT] | None: ...
+    @overload
+    def pop(self, key: _KT) -> _VT: ...
+    @overload
+    def pop(self, key: _KT, default: _VT | _T) -> _VT | _T: ...
+    def popitem(self, least_recent: bool = ...) -> tuple[_KT, _VT]: ...
+    @overload
+    def setdefault(self: LRU[_KT, _T | None], key: _KT) -> _T | None: ...
+    @overload
+    def setdefault(self, key: _KT, default: _VT) -> _VT: ...
+    def set_callback(self, callback: Callable[[_KT, _VT], Any]) -> None: ...
+    def set_size(self, size: int) -> None: ...
+    @overload
+    def update(self, __m: Iterable[tuple[_KT, _VT]], **kwargs: _VT) -> None: ...
+    @overload
+    def update(self, **kwargs: _VT) -> None: ...
+    def __contains__(self, __o: Any) -> bool: ...
+    def __delitem__(self, key: _KT) -> None: ...
+    def __getitem__(self, item: _KT) -> _VT: ...
+    def __len__(self) -> int: ...
+    def __repr__(self) -> str: ...
+    def __setitem__(self, key: _KT, value: _VT) -> None: ...
```

### Comparing `tarina-0.1.2/tarina/signature.py` & `tarina-0.2.1/src/tarina/signature.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,82 @@
-from __future__ import annotations
-
-import functools
-import inspect
-from typing import Callable, Any, Mapping
-
-
-@functools.lru_cache(4096)
-def get_signature(target: Callable):
-    return inspect.signature(target).parameters.values()
-
-
-try:
-    from inspect import get_annotations  # type: ignore
-except ImportError:
-
-    def get_annotations(
-        obj: Callable,
-        *,
-        _globals: Mapping[str, Any] | None = None,
-        _locals: Mapping[str, Any] | None = None,
-        eval_str: bool = False,
-    ) -> dict[str, Any]:  # sourcery skip: avoid-builtin-shadow
-        if not callable(obj):
-            raise TypeError(f"{obj!r} is not a module, class, or callable.")
-
-        ann = getattr(obj, "__annotations__", None)
-        obj_globals = getattr(obj, "__globals__", None)
-        obj_locals = None
-        unwrap = obj
-        if ann is None:
-            return {}
-
-        if not isinstance(ann, dict):
-            raise ValueError(f"{unwrap!r}.__annotations__ is neither a dict nor None")
-        if not ann:
-            return {}
-
-        if not eval_str:
-            return dict(ann)
-
-        if unwrap is not None:
-            while True:
-                if hasattr(unwrap, "__wrapped__"):
-                    unwrap = unwrap.__wrapped__
-                    continue
-                if isinstance(unwrap, functools.partial):
-                    unwrap = unwrap.func
-                    continue
-                break
-            if hasattr(unwrap, "__globals__"):
-                obj_globals = unwrap.__globals__
-
-        if _globals is None:
-            _globals = obj_globals
-        if _locals is None:
-            _locals = obj_locals
-
-        return {key: eval(value, _globals, _locals) if isinstance(value, str) else value for key, value in ann.items()}  # type: ignore
-
-
-@functools.lru_cache(4096)
-def signatures(callable_target: Callable) -> list[tuple[str, Any, Any]]:
-    callable_annotation = get_annotations(callable_target, eval_str=True)
-    return [
-        (
-            param.name,
-            (
-                callable_annotation.get(param.name)
-                if isinstance(param.annotation, str)
-                else param.annotation
-            )
-            if param.annotation is not inspect.Signature.empty
-            else None,
-            param.default,
-        )
-        for param in get_signature(callable_target)
-    ]
+from __future__ import annotations
+
+import functools
+import inspect
+from typing import Callable, Any, Mapping
+
+
+@functools.lru_cache(4096)
+def get_signature(target: Callable):
+    return inspect.signature(target).parameters.values()
+
+
+try:
+    from inspect import get_annotations  # type: ignore
+except ImportError:
+
+    def get_annotations(
+        obj: Callable,
+        *,
+        _globals: Mapping[str, Any] | None = None,
+        _locals: Mapping[str, Any] | None = None,
+        eval_str: bool = False,
+    ) -> dict[str, Any]:  # sourcery skip: avoid-builtin-shadow
+        if not callable(obj):
+            raise TypeError(f"{obj!r} is not a module, class, or callable.")
+
+        ann = getattr(obj, "__annotations__", None)
+        obj_globals = getattr(obj, "__globals__", None)
+        obj_locals = None
+        unwrap = obj
+        if ann is None:
+            return {}
+
+        if not isinstance(ann, dict):
+            raise ValueError(f"{unwrap!r}.__annotations__ is neither a dict nor None")
+        if not ann:
+            return {}
+
+        if not eval_str:
+            return dict(ann)
+
+        if unwrap is not None:
+            while True:
+                if hasattr(unwrap, "__wrapped__"):
+                    unwrap = unwrap.__wrapped__
+                    continue
+                if isinstance(unwrap, functools.partial):
+                    unwrap = unwrap.func
+                    continue
+                break
+            if hasattr(unwrap, "__globals__"):
+                obj_globals = unwrap.__globals__
+
+        if _globals is None:
+            _globals = obj_globals
+        if _locals is None:
+            _locals = obj_locals
+
+        return {
+            key: eval(value, _globals, _locals)  # type: ignore
+            if isinstance(value, str) else value
+            for key, value in ann.items()
+        }
+
+
+@functools.lru_cache(4096)
+def signatures(callable_target: Callable) -> list[tuple[str, Any, Any]]:
+    callable_annotation = get_annotations(callable_target, eval_str=True)
+    return [
+        (
+            param.name,
+            (
+                callable_annotation.get(param.name)
+                if isinstance(param.annotation, str)
+                else param.annotation
+            )
+            if param.annotation is not inspect.Signature.empty
+            else None,
+            param.default,
+        )
+        for param in get_signature(callable_target)
+    ]
```

### Comparing `tarina-0.1.2/tarina/tools.py` & `tarina-0.2.1/src/tarina/tools.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from __future__ import annotations
-
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Awaitable,
-    Callable,
-    Generator,
-    Iterable,
-    Literal,
-    TypeVar,
-    overload,
-)
-
-from typing_extensions import ParamSpec
-
-from .guard import is_async
-
-T = TypeVar("T")
-
-
-def group_dict(iterable: Iterable, key_callable: Callable[[Any], Any]):
-    temp = {}
-    for i in iterable:
-        k = key_callable(i)
-        temp.setdefault(k, []).append(i)
-    return temp
-
-
-async def run_always_await(
-    target: Callable[..., Any] | Callable[..., Awaitable[Any]], *args, **kwargs
-) -> Any:
-    obj = target(*args, **kwargs)
-    if is_async(target) or is_async(obj):
-        obj = await obj
-    return obj
-
-
-def gen_subclass(cls: type[T]) -> Generator[type[T], None, None]:
-    """生成某个类的所有子类 (包括其自身)
-    Args:
-        cls (Type[T]): 类
-    Yields:
-        Type[T]: 子类
-    """
-    yield cls
-    for sub_cls in cls.__subclasses__():
-        if TYPE_CHECKING:
-            assert issubclass(sub_cls, cls)
-        yield from gen_subclass(sub_cls)
-
-
-R = TypeVar("R")
-P = ParamSpec("P")
-
-
-@overload
-def init_spec(fn: Callable[P, T]) -> Callable[[Callable[[T], R]], Callable[P, R]]:
-    ...
-
-
-@overload
-def init_spec(
-    fn: Callable[P, T], is_method: Literal[True]
-) -> Callable[[Callable[[Any, T], R]], Callable[P, R]]:
-    ...
-
-
-def init_spec(  # type: ignore
-    fn: Callable[P, T], is_method: bool = False
-) -> Callable[[Callable[[T], R] | Callable[[Any, T], R]], Callable[P, R]]:
-    def wrapper(func: Callable[[T], R] | Callable[[Any, T], R]) -> Callable[P, R]:
-        def inner(*args: P.args, **kwargs: P.kwargs):
-            if is_method:
-                return func(args[0], fn(*args[1:], **kwargs))  # type: ignore
-            return func(fn(*args, **kwargs))  # type: ignore
-
-        return inner
-
-    return wrapper
+from __future__ import annotations
+
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Awaitable,
+    Callable,
+    Generator,
+    Iterable,
+    Literal,
+    TypeVar,
+    overload,
+)
+
+from typing_extensions import ParamSpec
+
+from .guard import is_async
+
+T = TypeVar("T")
+
+
+def group_dict(iterable: Iterable, key_callable: Callable[[Any], Any]):
+    temp = {}
+    for i in iterable:
+        k = key_callable(i)
+        temp.setdefault(k, []).append(i)
+    return temp
+
+
+async def run_always_await(
+    target: Callable[..., Any] | Callable[..., Awaitable[Any]], *args, **kwargs
+) -> Any:
+    obj = target(*args, **kwargs)
+    if is_async(target) or is_async(obj):
+        obj = await obj
+    return obj
+
+
+def gen_subclass(cls: type[T]) -> Generator[type[T], None, None]:
+    """生成某个类的所有子类 (包括其自身)
+    Args:
+        cls (Type[T]): 类
+    Yields:
+        Type[T]: 子类
+    """
+    yield cls
+    for sub_cls in cls.__subclasses__():
+        if TYPE_CHECKING:
+            assert issubclass(sub_cls, cls)
+        yield from gen_subclass(sub_cls)
+
+
+R = TypeVar("R")
+P = ParamSpec("P")
+
+
+@overload
+def init_spec(fn: Callable[P, T]) -> Callable[[Callable[[T], R]], Callable[P, R]]:
+    ...
+
+
+@overload
+def init_spec(
+    fn: Callable[P, T], is_method: Literal[True]
+) -> Callable[[Callable[[Any, T], R]], Callable[P, R]]:
+    ...
+
+
+def init_spec(  # type: ignore
+    fn: Callable[P, T], is_method: bool = False
+) -> Callable[[Callable[[T], R] | Callable[[Any, T], R]], Callable[P, R]]:
+    def wrapper(func: Callable[[T], R] | Callable[[Any, T], R]) -> Callable[P, R]:
+        def inner(*args: P.args, **kwargs: P.kwargs):
+            if is_method:
+                return func(args[0], fn(*args[1:], **kwargs))  # type: ignore
+            return func(fn(*args, **kwargs))  # type: ignore
+
+        return inner
+
+    return wrapper
```

