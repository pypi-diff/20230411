# Comparing `tmp/corgy-6.0.0.tar.gz` & `tmp/corgy-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corgy-6.0.0.tar", max compression
+gzip compressed data, was "corgy-7.0.0.tar", max compression
```

## Comparing `corgy-6.0.0.tar` & `corgy-7.0.0.tar`

### file list

```diff
@@ -1,21 +1,42 @@
--rw-r--r--   0        0        0    25090 2023-03-27 14:28:17.177652 corgy-6.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-03-27 14:28:17.177652 corgy-6.0.0/LICENSE
--rw-r--r--   0        0        0     4158 2023-03-27 14:28:17.177652 corgy-6.0.0/README.md
--rw-r--r--   0        0        0      225 2023-03-27 14:28:17.177652 corgy-6.0.0/corgy/__init__.py
--rw-r--r--   0        0        0    63878 2023-03-27 14:28:17.177652 corgy-6.0.0/corgy/_corgy.py
--rw-r--r--   0        0        0    36279 2023-03-27 14:28:17.177652 corgy-6.0.0/corgy/_helpfmt.py
--rw-r--r--   0        0        0     6988 2023-03-27 14:28:17.177652 corgy-6.0.0/corgy/_utils.py
--rw-r--r--   0        0        0       64 2023-03-27 14:28:56.430452 corgy-6.0.0/corgy/_version.py
--rw-r--r--   0        0        0        0 2023-03-27 14:28:17.177652 corgy-6.0.0/corgy/py.typed
--rw-r--r--   0        0        0    32416 2023-03-27 14:28:17.177652 corgy-6.0.0/corgy/types.py
--rw-r--r--   0        0        0    32202 2023-03-27 14:28:17.177652 corgy-6.0.0/docs/corgy.md
--rw-r--r--   0        0        0    12777 2023-03-27 14:28:17.177652 corgy-6.0.0/docs/corgy.types.md
--rw-r--r--   0        0        0      129 2023-03-27 14:28:17.177652 corgy-6.0.0/docs/index.md
--rwxr-xr-x   0        0        0      839 2023-03-27 14:28:17.177652 corgy-6.0.0/docs/make.sh
--rw-r--r--   0        0        0     2669 2023-03-27 14:28:56.430452 corgy-6.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 14:28:17.177652 corgy-6.0.0/tests/__init__.py
--rw-r--r--   0        0        0   102668 2023-03-27 14:28:17.181652 corgy-6.0.0/tests/test_corgy.py
--rw-r--r--   0        0        0      466 2023-03-27 14:28:17.181652 corgy-6.0.0/tests/test_doctests.py
--rw-r--r--   0        0        0    46095 2023-03-27 14:28:17.181652 corgy-6.0.0/tests/test_helpfmt.py
--rw-r--r--   0        0        0    24995 2023-03-27 14:28:17.181652 corgy-6.0.0/tests/test_types.py
--rw-r--r--   0        0        0     5457 1970-01-01 00:00:00.000000 corgy-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0    27949 2023-04-11 20:42:16.071329 corgy-7.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-04-11 20:42:16.071329 corgy-7.0.0/LICENSE
+-rw-r--r--   0        0        0     4158 2023-04-11 20:42:16.071329 corgy-7.0.0/README.md
+-rw-r--r--   0        0        0      395 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/__init__.py
+-rw-r--r--   0        0        0     2329 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/_actions.py
+-rw-r--r--   0        0        0      505 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/_annotations.py
+-rw-r--r--   0        0        0    46721 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/_corgy.py
+-rw-r--r--   0        0        0     6228 2023-04-11 20:42:16.071329 corgy-7.0.0/corgy/_corgyparser.py
+-rw-r--r--   0        0        0    36993 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/_helpfmt.py
+-rw-r--r--   0        0        0    17249 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/_meta.py
+-rw-r--r--   0        0        0       64 2023-04-11 20:43:01.971882 corgy-7.0.0/corgy/_version.py
+-rw-r--r--   0        0        0        0 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/py.typed
+-rw-r--r--   0        0        0     1727 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/__init__.py
+-rw-r--r--   0        0        0     5838 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_dir.py
+-rw-r--r--   0        0        0     2382 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_expand.py
+-rw-r--r--   0        0        0     3414 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_filepath.py
+-rw-r--r--   0        0        0     3413 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_initargs.py
+-rw-r--r--   0        0        0     2777 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_inputfile.py
+-rw-r--r--   0        0        0     5464 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_keyvaluepairs.py
+-rw-r--r--   0        0        0     5271 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_outputfile.py
+-rw-r--r--   0        0        0     9846 2023-04-11 20:42:16.075329 corgy-7.0.0/corgy/types/_subclass.py
+-rw-r--r--   0        0        0    32375 2023-04-11 20:42:16.075329 corgy-7.0.0/docs/corgy.md
+-rw-r--r--   0        0        0    14889 2023-04-11 20:42:16.075329 corgy-7.0.0/docs/corgy.types.md
+-rw-r--r--   0        0        0      132 2023-04-11 20:42:16.075329 corgy-7.0.0/docs/index.md
+-rw-r--r--   0        0        0     2679 2023-04-11 20:43:01.971882 corgy-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/__init__.py
+-rw-r--r--   0        0        0    87305 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/test_corgy.py
+-rw-r--r--   0        0        0    16513 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/test_corgyparser.py
+-rw-r--r--   0        0        0      823 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/test_doctests.py
+-rw-r--r--   0        0        0    47095 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/test_helpfmt.py
+-rw-r--r--   0        0        0        0 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/_pklclasses.py
+-rw-r--r--   0        0        0     2002 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/_specialtmps.py
+-rw-r--r--   0        0        0     3356 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/_test_file.py
+-rw-r--r--   0        0        0     6023 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_dirs.py
+-rw-r--r--   0        0        0     5365 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_filepaths.py
+-rw-r--r--   0        0        0     2678 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_initargs.py
+-rw-r--r--   0        0        0     2496 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_inputfiles.py
+-rw-r--r--   0        0        0     5443 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_keyvaluepairs.py
+-rw-r--r--   0        0        0     5085 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_outputfiles.py
+-rw-r--r--   0        0        0     7082 2023-04-11 20:42:16.075329 corgy-7.0.0/tests/types/test_subclass.py
+-rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 corgy-7.0.0/PKG-INFO
```

### Comparing `corgy-6.0.0/CHANGELOG.md` & `corgy-7.0.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,54 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+## [7.0.0](https://github.com/jayanthkoushik/corgy/compare/v6.0.0...v7.0.0) (2023-04-11)
+
+
+### ⚠ BREAKING CHANGES
+
+* A few types in `corgy.types` accepted arbitrary keyword
+arguments. This was not consistent, not tested, and has been removed.
+All file related types now accept a single "path-like" argument.
+* `Path` subclasses in `corgy.types` now perform user
+home (~) and environment variable expansion by default. These classes
+also have two new attributes: `do_expanduser` and `do_expandvars` which
+can be set to `False` to disable expansion of home and environment vars
+respectively.
+* `OutputTextFile.stdout_wrapper`,
+`OutputTextFile.stderr_wrapper`, `InputTextFile.stdin_wrapper` are now
+classmethods instead of classproperties. The change allows simpler
+implementation without relying on custom metaclass, and also enables
+type checking in these methods.
+* The package no longer relies on, or uses
+`typing.Required` and `typing.NotRequired`, since type checkers consider
+it an error to use them outside of `TypedDict`s. `corgy` now provides
+its own versions of these types, implemented using `typing.Annotated`,
+so that type checking works as expected. Usage remains the same.
+
+### Features
+
+* add binary versions of `stdout/stderr/stdin` wrappers in `corgy.types` ([5083b23](https://github.com/jayanthkoushik/corgy/commit/5083b238e5e87d1917332ca0d735608893d40b3e))
+* add types for input/output file paths ([f96eca7](https://github.com/jayanthkoushik/corgy/commit/f96eca710524d91605521cf237aede4a05d63eb9))
+* perform user and environment variable expansion in `Path` types ([e3100fe](https://github.com/jayanthkoushik/corgy/commit/e3100feeb8c16845ca4edba4a0b6339d09fa7156))
+
+
+### Bug Fixes
+
+* do not convert positional bools to option pairs in `Corgy.add_args_to_parser` ([7fcda64](https://github.com/jayanthkoushik/corgy/commit/7fcda649a2a8f65d4b990a0f923b7371cb4173ae))
+* fix handling of choices when using custom parsers ([40ec87b](https://github.com/jayanthkoushik/corgy/commit/40ec87b1ae44572bfdc591b9f819d8074c7c60c2))
+* only mark args as 'optional' by 'CorgyHelpFormatter' if `default=SUPPRESS` ([5b7603f](https://github.com/jayanthkoushik/corgy/commit/5b7603f272a7f56fa9487c5dc523d876b4732269))
+* remove `kwargs` from argument list of file types ([f3aa648](https://github.com/jayanthkoushik/corgy/commit/f3aa6487bb7cfd7acf61610c4dc0da93cd888bf0))
+* use custom implementations of `Required` and `NotRequired` ([ebf0913](https://github.com/jayanthkoushik/corgy/commit/ebf0913c4f0b61ae9d88422456c477ef170dfbf1))
+* use proper delegation to concrete `Path` types in `corgy.types` ([580dd86](https://github.com/jayanthkoushik/corgy/commit/580dd868c95b8f7e8d8a9ae4af2b0a1bdae767b0))
+
+
+* rewrite `stdout/stderr/stdin` wrappers in \`corgy.types\` ([99307eb](https://github.com/jayanthkoushik/corgy/commit/99307ebf6f9811e79c907fcb292625d44a2552a8))
+
 ## [6.0.0](https://github.com/jayanthkoushik/corgy/compare/v5.0.0...v6.0.0) (2023-03-27)
 
 
 ### ⚠ BREAKING CHANGES
 
 * By default, `Corgy.add_args_to_parser` now adds
 attributes as optional. This makes command line parsing consistent with
```

### Comparing `corgy-6.0.0/LICENSE` & `corgy-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corgy-6.0.0/README.md` & `corgy-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `corgy-6.0.0/corgy/_corgy.py` & `corgy-7.0.0/corgy/_corgy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,327 +1,39 @@
 from __future__ import annotations
 
 import argparse
-import importlib
 import sys
+from argparse import _ActionsContainer, Action, ArgumentParser
 from collections import defaultdict
 from collections.abc import Sequence as AbstractSequence
-from contextlib import suppress
 from functools import partial
-from typing import (
-    Any,
-    Callable,
-    ClassVar,
-    Dict,
-    IO,
-    List,
-    Mapping,
-    NamedTuple,
-    Optional,
-    Type,
-    TypeVar,
-    Union,
-)
+from importlib import import_module
+from typing import Any, Callable, Dict, IO, Mapping, Optional, Type, TypeVar, Union
 
 if sys.version_info >= (3, 9):
-    from typing import get_type_hints, Literal
-else:
-    from typing_extensions import get_type_hints, Literal
-
-if sys.version_info >= (3, 11):
-    from typing import NotRequired, Required
+    from typing import Literal
 else:
-    from typing_extensions import Required, NotRequired
+    from typing_extensions import Literal
 
+from ._actions import BooleanOptionalAction, OptionalTypeAction
+from ._corgyparser import CorgyParserAction
 from ._helpfmt import CorgyHelpFormatter
-from ._utils import (
+from ._meta import (
     check_val_type,
+    CorgyMeta,
     get_concrete_collection_type,
     is_literal_type,
     is_optional_type,
-    OptionalTypeAction,
 )
 
-# The main interface is the `Corgy` class. `_CorgyMeta` modifies creation of `Corgy`
-# (and its subclasses) by converting annotations to properties, and setting up utilities
-# for command line parsing. `corgyparser` is a decorator that allows custom parsers to
-# be defined for `Corgy` attributes.
-
-__all__ = ("Corgy", "corgyparser")
+__all__ = ("Corgy",)
 _T = TypeVar("_T", bound="Corgy")
 
 
-class BooleanOptionalAction(argparse.Action):
-    # :meta private:
-    # Backport of `argparse.BooleanOptionalAction` from Python 3.9.
-    # Taken almost verbatim from `CPython/Lib/argparse.py`.
-    def __init__(self, option_strings, dest, *args, **kwargs):
-        _option_strings = []
-        for option_string in option_strings:
-            _option_strings.append(option_string)
-
-            if option_string.startswith("--"):
-                option_string = "--no-" + option_string[2:]
-                _option_strings.append(option_string)
-
-        super().__init__(
-            option_strings=_option_strings, dest=dest, nargs=0, *args, **kwargs
-        )
-
-    def __call__(self, parser, namespace, values, option_string=None):
-        if option_string in self.option_strings:
-            setattr(namespace, self.dest, not option_string.startswith("--no-"))
-
-
-class _CorgyMeta(type):
-    """Metaclass for `Corgy`.
-
-    Modifies class creation by parsing type annotations, and creating properties for
-    each annotated attribute. Default values and custom parsers are stored in the
-    `__defaults` and `__parsers` attributes. Custom flags, if present, are stored in
-    the `__flags` attribute. `Required` and `NotRequired` annotations are extracted,
-    and required attributes are stored in `__required`.
-    """
-
-    __slots__ = ()
-
-    def __new__(cls, name, bases, namespace, **kwds) -> _CorgyMeta:
-        try:
-            _make_slots = kwds.pop("corgy_make_slots")
-        except KeyError:
-            _make_slots = True
-
-        if _make_slots:
-            if "__slots__" not in namespace:
-                namespace["__slots__"] = []
-            else:
-                namespace["__slots__"] = list(namespace["__slots__"])
-            namespace["__slots__"].append("__frozen")
-        elif "__slots__" in namespace:
-            raise TypeError(
-                "`__slots__` cannot be defined if `corgy_make_slots` is `False`"
-            )
-
-        cls_annotations = namespace.get("__annotations__", {})
-        namespace["__annotations__"] = {}
-        namespace["__defaults"] = {}
-        namespace["__flags"] = {}
-        namespace["__parsers"] = {}
-        namespace["__helps"] = {}
-        namespace["__required"] = set()
-
-        # Temp set of not required attributes--to handle inheritance from
-        # non-`Corgy` classes.
-        _not_required = set()
-
-        # Extract `corgy_freeze_after_init` (default `False`).
-        try:
-            namespace["__freeze_after_init"] = kwds.pop("corgy_freeze_after_init")
-        except KeyError:
-            namespace["__freeze_after_init"] = False
-
-        # See if `corgy_track_bases` is specified (default `True`).
-        try:
-            _track_bases = kwds.pop("corgy_track_bases")
-        except KeyError:
-            _track_bases = True
-        if _track_bases:
-            for base in bases:
-                _base_annotations = getattr(base, "__annotations__", {})
-                namespace["__annotations__"].update(_base_annotations)
-                if isinstance(base, cls):
-                    # `base` is also a `Corgy` class.
-                    namespace["__defaults"].update(getattr(base, "__defaults"))
-                    namespace["__flags"].update(getattr(base, "__flags"))
-                    namespace["__parsers"].update(getattr(base, "__parsers"))
-                    namespace["__helps"].update(getattr(base, "__helps"))
-                    namespace["__required"].update(getattr(base, "__required"))
-                    # Add not required attributes to temp set.
-                    _base_required = getattr(base, "__required")
-                    for _var_name in _base_annotations:
-                        if _var_name not in _base_required:
-                            _not_required.add(_var_name)
-                else:
-                    # Fetch default values directly from the base.
-                    for _var_name in _base_annotations:
-                        try:
-                            namespace["__defaults"][_var_name] = getattr(
-                                base, _var_name
-                            )
-                        except AttributeError:
-                            pass
-
-        # Add current annotations last, so that they override base values.
-        namespace["__annotations__"].update(cls_annotations)
-
-        # See if `corgy_required_by_default` is specified (default `False`).
-        try:
-            _required_by_default = kwds.pop("corgy_required_by_default")
-        except KeyError:
-            _required_by_default = False
-
-        tempnew = super().__new__(cls, name, bases, namespace)
-        type_hints = get_type_hints(tempnew, include_extras=True)
-
-        if not type_hints:
-            return tempnew
-
-        del tempnew  # YUCK
-        for var_name in set(namespace["__annotations__"].keys()):
-            var_ano = type_hints[var_name]
-            # Check for name conflicts.
-            _mangled_name = f"_{name.lstrip('_')}__{var_name}"
-            if _mangled_name in namespace or _mangled_name in cls_annotations:
-                raise TypeError(f"name clash: `{var_name}`, `{_mangled_name}`")
-
-            if hasattr(var_ano, "__origin__") and hasattr(var_ano, "__metadata__"):
-                # `<var_name>: Annotated[<var_type>, <var_help>, [<var_flags>]]`.
-                var_type = var_ano.__origin__
-                var_help = var_ano.__metadata__[0]
-                if not isinstance(var_help, str):
-                    raise TypeError(
-                        f"incorrect help string annotation for variable `{var_name}`: "
-                        f"expected str"
-                    )
-
-                if len(var_ano.__metadata__) > 1:
-                    if isinstance(var_type, cls):
-                        # Custom flags are not allowed for groups.
-                        raise TypeError(
-                            f"invalid annotation for group `{var_name}`: "
-                            f"custom flags not allowed for groups"
-                        )
-
-                    var_flags = var_ano.__metadata__[1]
-                    if not isinstance(var_flags, list) or not var_flags:
-                        raise TypeError(
-                            f"incorrect custom flags for variable `{var_name}`: "
-                            f"expected non-empty list"
-                        )
-                else:
-                    var_flags = None
-            else:
-                # `<var_name>: <var_type>`.
-                var_type = var_ano
-                var_help = namespace["__helps"].get(var_name, None)
-                var_flags = namespace["__flags"].get(var_name, None)
-
-            if hasattr(var_type, "__origin__") and var_type.__origin__ is ClassVar:
-                # Class variable: make sure it has an associated value.
-                if var_name not in namespace:
-                    if var_name in namespace["__defaults"]:
-                        del namespace["__defaults"][var_name]
-                    else:
-                        raise TypeError(f"class variable `{var_name}` has no value set")
-                del namespace["__annotations__"][var_name]
-                continue
-
-            # Determine if variable is required or not.
-            if hasattr(var_type, "__origin__") and var_type.__origin__ in (
-                Required,
-                NotRequired,
-            ):
-                _var_required = var_type.__origin__ is Required
-                var_type = var_type.__args__[0]
-            elif var_name not in cls_annotations:
-                # Variable was defined in a base class, and is not redefined.
-                if var_name in namespace["__required"]:
-                    _var_required = True
-                elif var_name in _not_required:
-                    _var_required = False
-                else:
-                    # Variable inherited from a non-`Corgy` class.
-                    _var_required = _required_by_default
-            else:
-                _var_required = _required_by_default
-
-            if _var_required:
-                namespace["__required"].add(var_name)
-            else:
-                # Remove from `__required`, in case it was required in a base class.
-                namespace["__required"].discard(var_name)
-
-            namespace["__annotations__"][var_name] = var_type
-
-            if var_help is not None:
-                namespace["__helps"][var_name] = var_help
-            if var_flags is not None:
-                namespace["__flags"][var_name] = var_flags
-
-            # Add default value to dedicated dict.
-            if var_name in namespace:
-                try:
-                    check_val_type(namespace[var_name], var_type)
-                except ValueError as e:
-                    raise ValueError(
-                        f"default value type mismatch for '{var_name}'"
-                    ) from e
-                namespace["__defaults"][var_name] = namespace[var_name]
-            elif var_name in namespace["__defaults"] and var_name in cls_annotations:
-                # Variable had a default value in a base class, but does not anymore.
-                del namespace["__defaults"][var_name]
-
-            # Create `<var_name>` property.
-            namespace[var_name] = cls._create_var_property(
-                name, var_name, var_type, var_help
-            )
-            if _make_slots:
-                if f"__{var_name}" in namespace["__slots__"]:
-                    raise TypeError(
-                        f"cannot have slot `__{var_name}`: internal clash with "
-                        f"`{var_name}`"
-                    )
-                namespace["__slots__"].append(f"__{var_name}")
-
-        if _make_slots:
-            namespace["__slots__"] = tuple(namespace["__slots__"])
-
-        # Store custom parsers in a dict.
-        for _, v in namespace.items():
-            if not isinstance(v, _CorgyParser):
-                continue
-            for var_name in v.var_names:
-                if (var_name in namespace["__annotations__"]) and isinstance(
-                    namespace[var_name], property
-                ):
-                    namespace["__parsers"][var_name] = v.fparse
-                else:
-                    raise TypeError(f"invalid target for corgyparser: {var_name}")
-
-        return super().__new__(cls, name, bases, namespace, **kwds)
-
-    @staticmethod
-    def _create_var_property(cls_name, var_name, var_type, var_doc) -> property:
-        # Properties are stored in private instance variables prefixed with `__`, and
-        # must be accessed as `_<cls>__<var_name>`.
-        def var_fget(self):
-            with suppress(AttributeError):
-                return getattr(self, f"_{cls_name.lstrip('_')}__{var_name}")
-            raise AttributeError(f"no value available for attribute `{var_name}`")
-
-        def var_fset(self, val):
-            if getattr(self, f"_{cls_name.lstrip('_')}__frozen"):
-                raise TypeError(f"cannot set `{var_name}`: object is frozen")
-            check_val_type(val, var_type)
-            setattr(self, f"_{cls_name.lstrip('_')}__{var_name}", val)
-
-        def var_fdel(self):
-            if getattr(self, f"_{cls_name.lstrip('_')}__frozen"):
-                raise TypeError(f"cannot delete `{var_name}`: object is frozen")
-            if var_name in getattr(self, "__required"):
-                raise TypeError(f"attribute `{var_name}` cannot be unset")
-            delattr(self, f"_{cls_name.lstrip('_')}__{var_name}")
-
-        var_fget.__annotations__ = {"return": var_type}
-        var_fset.__annotations__ = {"val": var_type}
-
-        return property(var_fget, var_fset, var_fdel, doc=var_doc)
-
-
-class Corgy(metaclass=_CorgyMeta):
+class Corgy(metaclass=CorgyMeta):
     """Base class for collections of attributes.
 
     To use, subclass `Corgy`, and declare attributes using type annotations::
 
         >>> from corgy import Corgy
 
         >>> class A(Corgy):
@@ -541,22 +253,18 @@
         ValueError: missing required attribute: `x`
         >>> a = A(x=1)
         >>> del a.x
         Traceback (most recent call last):
             ...
         TypeError: attribute `x` cannot be unset
 
-    Attributes can also explicitly be marked as required/not-required using the
-    `Required` and `NotRequired` annotations::
+    Attributes can also explicitly be marked as required/not-required using
+    `corgy.Required` and `corgy.NotRequired` annotations::
 
-        >>> import sys
-        >>> if sys.version_info >= (3, 11):
-        ...     from typing import Required, NotRequired
-        ... else:
-        ...     from typing_extensions import Required, NotRequired
+        >>> from corgy import Required, NotRequired
 
         >>> class A(Corgy):
         ...     x: Required[int]
         ...     y: NotRequired[int]
         ...     z: int  # not required by default
 
         >>> a = A(x=1)
@@ -720,15 +428,15 @@
     match the argument type; in the above example, `__choices__` could be set to
     `(1, "2")`.
     """
 
     @classmethod
     def add_args_to_parser(
         cls,
-        parser: argparse._ActionsContainer,
+        parser: _ActionsContainer,
         name_prefix: str = "",
         flatten_subgrps: bool = False,
         defaults: Optional[Mapping[str, Any]] = None,
     ):
         """Add the class' `Corgy` attributes to the given parser.
 
         Args:
@@ -749,24 +457,25 @@
         special annotations are parsed and stripped from attribute types to determine
         the parameters for calling `ArgumentParser.add_argument`. These special
         annotations are described below.
 
         *Annotated*
         `typing.Annotated` can be used to add a help message for the argument::
 
-            >>> from argparse import ArgumentParser, SUPPRESS
+            >>> import argparse
+            >>> from argparse import ArgumentParser
             >>> from corgy import CorgyHelpFormatter
 
             >>> class A(Corgy):
             ...     x: Annotated[int, "help for x"]
 
             >>> parser = ArgumentParser(
             ...     formatter_class=CorgyHelpFormatter,
             ...     add_help=False,
-            ...     usage=SUPPRESS,
+            ...     usage=argparse.SUPPRESS,
             ... )
 
             >>> A.add_args_to_parser(parser)
             >>> parser.print_help()
             options:
               --x int  help for x (optional)
 
@@ -778,15 +487,15 @@
             >>> class A(Corgy):
             ...     x: Annotated[int, "help for x", ["-x", "--ex"]]
             ...     y: Annotated[int, "help for y", ["y"]]
 
             >>> parser = ArgumentParser(
             ...     formatter_class=CorgyHelpFormatter,
             ...     add_help=False,
-            ...     usage=SUPPRESS,
+            ...     usage=argparse.SUPPRESS,
             ... )
 
             >>> A.add_args_to_parser(parser)
             >>> parser.print_help()
             positional arguments:
               y int        help for y
             <BLANKLINE>
@@ -799,34 +508,36 @@
 
         *Required/NotRequired*
         Every corgy attribute is either required or not required. The default status
         depends on the class parameter `corgy_required_by_default` (`False` by default).
         Attributes can also be explicitly marked as required or not required, and will
         control whether the argument will be added with `required=True`::
 
+            >>> from corgy import Required, NotRequired
+
             >>> class A(Corgy):
             ...     x: Required[int]
             ...     y: NotRequired[int]
             ...     z: int
 
             >>> parser = ArgumentParser(
             ...     formatter_class=CorgyHelpFormatter,
             ...     add_help=False,
-            ...     usage=SUPPRESS,
+            ...     usage=argparse.SUPPRESS,
             ... )
 
             >>> A.add_args_to_parser(parser)
             >>> parser.print_help()
             options:
               --x int  (required)
               --y int  (optional)
               --z int  (optional)
 
         Attributes which are not required, and don't have a default value are added
-        with `default=SUPPRESS`, and so will not be included in the parsed namespace::
+        with `default=argparse.SUPPRESS`, and so will not be in the parsed namespace::
 
             >>> parser.parse_args(["--x", "1", "--y", "2"])
             Namespace(x=1, y=2)
 
         *Optional*
         Attributes marked with `typing.Optional` are allowed to be `None`. The
         arguments for these attributes can be passed with no values (i.e. `--x`
@@ -851,15 +562,15 @@
 
             >>> class A(Corgy):
             ...     arg: bool
 
             >>> parser = ArgumentParser(
             ...     formatter_class=CorgyHelpFormatter,
             ...     add_help=False,
-            ...     usage=SUPPRESS,
+            ...     usage=argparse.SUPPRESS,
             ... )
 
             >>> A.add_args_to_parser(parser)
             >>> parser.print_help()
             options:
               --arg/--no-arg
 
@@ -902,15 +613,15 @@
 
             >>> class A(Corgy):
             ...     x: Literal[T1, T2]
 
             >>> parser = ArgumentParser(
             ...     formatter_class=CorgyHelpFormatter,
             ...     add_help=False,
-            ...     usage=SUPPRESS,
+            ...     usage=argparse.SUPPRESS,
             ... )
 
             >>> A.add_args_to_parser(parser)
             >>> parser.print_help()
             options:
               --x T  ({T1/T2} optional)
 
@@ -934,15 +645,15 @@
             >>> class A(Corgy):
             ...     x: int
             ...     g: G
 
             >>> parser = ArgumentParser(
             ...     formatter_class=CorgyHelpFormatter,
             ...     add_help=False,
-            ...     usage=SUPPRESS,
+            ...     usage=argparse.SUPPRESS,
             ... )
 
             >>> A.add_args_to_parser(parser)
             >>> parser.print_help()
             options:
               --x int      (optional)
             <BLANKLINE>
@@ -990,14 +701,18 @@
                     for flag in var_flags
                 ]
                 var_dest = f"{name_prefix}:{var_name}"
             else:
                 var_dest = var_name
 
             if not any(_flag.startswith("-") for _flag in var_flags):
+                # Note: the flags cannot be passed to `add_argument` with `dest` set
+                # to `var_name` since `argparse` will raise an error for passing `dest`
+                # twice (for positional arguments, `argparse` uses the flag to infer the
+                # `dest`).
                 var_flags = [var_name]
                 var_positional = True
             elif all(_flag.startswith("-") for _flag in var_flags):
                 var_positional = False
             else:
                 raise TypeError(
                     f"inconsistent positional/optional flags for {var_name}: "
@@ -1019,23 +734,23 @@
                         ) from None
                 else:
                     grp_defaults = {}
 
                 # Update defaults with any values specified individually.
                 grp_defaults.update(group_arg_defaults.get(var_name, {}))
 
-                grp_parser: argparse._ActionsContainer
+                grp_parser: _ActionsContainer
                 if flatten_subgrps:
                     grp_parser = base_parser
                 else:
                     grp_parser = base_parser.add_argument_group(var_dest, var_help)
                 var_type.add_args_to_parser(grp_parser, var_dest, True, grp_defaults)
                 continue
 
-            var_action: Optional[Type[argparse.Action]] = None
+            var_action: Optional[Type[Action]] = None
 
             # Check if the variable is required on the command line.
             var_required = var_name not in base_defaults and var_name in required_attrs
 
             # Check if the variable can be `None`.
             if is_optional_type(var_type):
                 var_base_type = var_type.__args__[0]
@@ -1112,23 +827,27 @@
             # Check if the variable is boolean. Boolean variables are converted to
             # `--<var-name>`/`--no-<var-name>` arguments.
             if (
                 var_base_type is bool
                 and var_nargs is None
                 and var_action is None
                 and var_choices is None
+                and not var_positional
             ):
                 var_action = BooleanOptionalAction
 
             # Check if the variable has a custom parser.
             _parsers = getattr(cls, "__parsers")
             if var_name in _parsers:
                 _var_parser = _parsers[var_name]
-                var_action = partial(CorgyParserAction, _var_parser)  # type: ignore
+                var_action = partial(
+                    CorgyParserAction, _var_parser, var_choices  # type: ignore
+                )
                 var_add_type = str
+                var_choices = None  # handled by the parser
                 var_nargs = getattr(_var_parser, "__nargs__", None)
                 _parser_metavar = getattr(_var_parser, "__metavar__", None)
                 if _parser_metavar is not None:
                     var_type_metavar = _parser_metavar
             else:
                 var_add_type = var_base_type
 
@@ -1273,28 +992,28 @@
         def dictify_corgys(_val):
             _coll_type = get_concrete_collection_type(type(_val))
             if _coll_type is not None:
                 _cast_type = _coll_type if _coll_type is not AbstractSequence else list
                 return _cast_type(  # pylint: disable=abstract-class-instantiated
                     [dictify_corgys(_val_part) for _val_part in _val]
                 )
-            if isinstance(_val.__class__, _CorgyMeta):
+            if isinstance(_val.__class__, CorgyMeta):
                 return _val.as_dict(recursive=True, flatten=flatten)
             return _val
 
         self_dict = {}
         for attr_name, attr_type in self.attrs().items():
             try:
                 attr_val = getattr(self, attr_name)
             except AttributeError:
                 continue
 
             if recursive:
                 attr_val = dictify_corgys(attr_val)
-                if flatten and isinstance(attr_type, _CorgyMeta):
+                if flatten and isinstance(attr_type, CorgyMeta):
                     for _k, _v in attr_val.items():
                         _flat_key = f"{attr_name}:{_k}"
                         self_dict[_flat_key] = _v
                     continue
 
             self_dict[attr_name] = attr_val
 
@@ -1355,21 +1074,21 @@
                         f"`{cls}` has no group named `{grp_name}`"
                     )
                 if grp_name in d:
                     raise ValueError(
                         f"conflicting arguments: `{arg_name}` and `{grp_name}`"
                     )
                 grp_type = cls_attrs[grp_name]
-                if not isinstance(grp_type, _CorgyMeta):
+                if not isinstance(grp_type, CorgyMeta):
                     raise ValueError(f"`{grp_name}` is not a `Corgy` class")
                 grp_args_map[grp_name][arg_name_base] = arg_val
 
             elif hasattr(cls, arg_name):
                 arg_type = cls_attrs[arg_name]
-                if isinstance(arg_type, _CorgyMeta) and isinstance(arg_val, dict):
+                if isinstance(arg_type, CorgyMeta) and isinstance(arg_val, dict):
                     grp_args_map[arg_name] = arg_val
                 else:
                     main_args_map[arg_name] = arg_val
 
         for grp_name, grp_args in grp_args_map.items():
             grp_type = cls_attrs[grp_name]
             main_args_map[grp_name] = grp_type.from_dict(grp_args, try_cast)
@@ -1429,29 +1148,29 @@
                         f"`{self.__class__}` has no group named `{grp_name}`"
                     )
                 if grp_name in d:
                     raise ValueError(
                         f"conflicting arguments: `{arg_name}` and `{grp_name}`"
                     )
                 grp_type = cls_attrs[grp_name]
-                if not isinstance(grp_type, _CorgyMeta):
+                if not isinstance(grp_type, CorgyMeta):
                     raise ValueError(f"`{grp_name}` is not a `Corgy` class")
                 main_args_map[grp_name][arg_name_base] = arg_val
 
             elif arg_name in cls_attrs:
                 main_args_map[arg_name] = arg_val
 
         for arg_name, arg_type in cls_attrs.items():
             if arg_name not in main_args_map:
                 if strict and hasattr(self, arg_name):
                     delattr(self, arg_name)
                 continue
 
             arg_new_val = main_args_map[arg_name]
-            if isinstance(arg_type, _CorgyMeta) and isinstance(arg_new_val, dict):
+            if isinstance(arg_type, CorgyMeta) and isinstance(arg_new_val, dict):
                 try:
                     arg_obj = getattr(self, arg_name)
                 except AttributeError:
                     setattr(self, arg_name, arg_type.from_dict(arg_new_val))
                 else:
                     arg_obj.load_dict(arg_new_val, try_cast, strict)
             else:
@@ -1459,15 +1178,15 @@
                     arg_new_val, arg_type, try_cast, try_load_corgy_dicts=True
                 )
                 setattr(self, arg_name, arg_new_val)
 
     @classmethod
     def parse_from_cmdline(
         cls: Type[_T],
-        parser: Optional[argparse.ArgumentParser] = None,
+        parser: Optional[ArgumentParser] = None,
         defaults: Optional[Mapping[str, Any]] = None,
         **parser_args,
     ) -> _T:
         """Return an instance of the class parsed from command line arguments.
 
         Args:
             parser: An instance of `argparse.ArgumentParser` or `None`. If `None`, a new
@@ -1475,20 +1194,20 @@
             defaults: A dictionary of default values for the attributes, passed to
                 `add_args_to_parser`. Refer to the docs for `add_args_to_parser` for
                 more details.
             parser_args: Arguments to be passed to `argparse.ArgumentParser()`. Ignored
                 if `parser` is not None.
 
         Raises:
-            ArgumentError: Error parsing command line arguments.
+            ArgumentTypeError: Error parsing command line arguments.
         """
         if parser is None:
             if "formatter_class" not in parser_args:
                 parser_args["formatter_class"] = CorgyHelpFormatter
-            parser = argparse.ArgumentParser(**parser_args)
+            parser = ArgumentParser(**parser_args)
         cls.add_args_to_parser(parser, defaults=defaults)
         args = vars(parser.parse_args())
         return cls.from_dict(args, try_cast=True)
 
     @classmethod
     def parse_from_toml(
         cls: Type[_T],
@@ -1523,17 +1242,15 @@
             ...     y = [1, 2, 3]
             ... ''')
 
             >>> A.parse_from_toml(f)  # doctest: +SKIP
             A(x='one', g=G(x=1, y=[1, 2, 3]))
 
         """
-        tomli = importlib.import_module(
-            "tomllib" if sys.version_info >= (3, 11) else "tomli"
-        )
+        tomli = import_module("tomllib" if sys.version_info >= (3, 11) else "tomli")
         toml_data = tomli.load(toml_file)
         if defaults is not None:
             for _k, _v in defaults.items():
                 if _k not in toml_data:
                     toml_data[_k] = _v
         _parsers = getattr(cls, "__parsers")
         for _k, _v in toml_data.items():
@@ -1560,158 +1277,7 @@
             >>> del a.y
             Traceback (most recent call last):
                 ...
             TypeError: cannot delete `y`: object is frozen
 
         """
         setattr(self, f"_{self.__class__.__name__.lstrip('_')}__frozen", True)
-
-
-class _CorgyParser(NamedTuple):
-    """Class to represent custom parsers.
-
-    This class is returned by the `@corgyparser` decorator, and is used by `Corgy` to
-    keep track of parsers.
-    """
-
-    var_names: List[str]
-    fparse: Callable[[str], Any]
-    nargs: Union[None, Literal["*", "+"], int]
-
-    def __call__(self, s):
-        return self.fparse(s)
-
-
-def corgyparser(
-    *var_names: str,
-    metavar: Optional[str] = None,
-    nargs: Union[None, Literal["*", "+"], int] = None,
-) -> Callable[[Union[Callable[[str], Any], _CorgyParser]], _CorgyParser]:
-    """Decorate a function as a custom parser for one or more attributes.
-
-    To use a custom function for parsing a `Corgy` attribute, use this decorator.
-    Parsing functions must be static, and should only accept a single argument.
-    Decorating the function with `@staticmethod` is optional, but prevents type errors.
-    `@corgyparser` must be the final decorator in the decorator chain.
-
-    Args:
-        var_names: The attributes associated with the decorated parser.
-        metavar: Keyword only argument to set the metavar when adding the associated
-            attribute(s) to an `ArgumentParser` instance.
-        nargs: Keyword only argument to set the number of arguments to be used for the
-            associated attribute(s). Must be `None`, `'*'`, `'+'`, or a positive number.
-            This value is passed as the `nargs` argument to
-            `ArgumentParser.add_argument`, and controls the number of arguments that
-            will be read from the command line, and passed to the parsing function.
-            For all values other than `None`, the parsing function will receive a list
-            of strings.
-
-    Example::
-
-        >>> from corgy import corgyparser
-
-        >>> class A(Corgy):
-        ...     time: Tuple[int, int, int]
-        ...     @corgyparser("time", metavar="int:int:int")
-        ...     @staticmethod
-        ...     def parse_time(s):
-        ...         return tuple(map(int, s.split(":")))
-
-        >>> parser = ArgumentParser(
-        ...     formatter_class=CorgyHelpFormatter,
-        ...     add_help=False,
-        ...     usage=SUPPRESS,
-        ... )
-
-        >>> A.add_args_to_parser(parser)
-        >>> parser.parse_args(["--time", "1:2:3"])
-        Namespace(time=(1, 2, 3))
-
-    Multiple arguments can be passed to the decorator, and will all be associated with
-    the same parser::
-
-        >>> class A(Corgy):
-        ...     x: int
-        ...     y: int
-        ...     @corgyparser("x", "y")
-        ...     @staticmethod
-        ...     def parse_x_y(s):
-        ...         return int(s)
-
-    The `@corgyparser` decorator can also be chained to use the same parser for multiple
-    arguments::
-
-        >>> class A(Corgy):
-        ...     x: int
-        ...     y: int
-        ...     @corgyparser("x")
-        ...     @corgyparser("y")
-        ...     @staticmethod
-        ...     def parse_x_y(s):
-        ...         return int(s)
-
-    Note: when chaining, the outer-most non-`None` value of `metavar` will be used.
-
-    Custom parsers can control the number of arguments they receive, independent of the
-    argument type::
-
-        >>> class A(Corgy):
-        ...     x: int
-        ...     @corgyparser("x", nargs=3)
-        ...     @staticmethod
-        ...     def parse_x(s):
-        ...         # `s` will be a list of 3 strings.
-        ...         return sum(map(int, s))
-
-        >>> parser = ArgumentParser(
-        ...     formatter_class=CorgyHelpFormatter,
-        ...     add_help=False,
-        ...     usage=SUPPRESS,
-        ... )
-
-        >>> A.add_args_to_parser(parser)
-        >>> parser.parse_args(["--x", "1", "2", "3"])
-        Namespace(x=6)
-
-    When chaining, `nargs` must be the same for all decorators, otherwise `TypeError` is
-    raised.
-    """
-    if not all(isinstance(_var_name, str) for _var_name in var_names):
-        raise TypeError(
-            "corgyparser should be passed the name of arguments: decorate using"
-            "@corgyparser(<argument(s)>)"
-        )
-
-    def wrapper(var_names, metavar, fparse):
-        if isinstance(fparse, _CorgyParser):
-            if nargs != fparse.nargs:
-                raise TypeError(
-                    "all `corgyparser` decorations of a funciton must have same `nargs`"
-                )
-            corgy_parser = fparse
-            corgy_parser.var_names.extend(var_names)
-        else:
-            if isinstance(fparse, staticmethod):
-                fparse = fparse.__func__
-            if not callable(fparse):
-                raise TypeError("corgyparser can only decorate static functions")
-            corgy_parser = _CorgyParser(list(var_names), fparse, nargs)
-
-        if metavar is not None:
-            setattr(corgy_parser.fparse, "__metavar__", metavar)
-        if nargs is not None:
-            setattr(corgy_parser.fparse, "__nargs__", nargs)
-        return corgy_parser
-
-    return partial(wrapper, var_names, metavar)
-
-
-class CorgyParserAction(argparse.Action):
-    def __init__(self, corgy_parser: _CorgyParser, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._corgy_parser = corgy_parser
-
-    def __call__(self, parser, namespace, values, option_string=None):
-        try:
-            setattr(namespace, self.dest, self._corgy_parser(values))
-        except ValueError as e:
-            raise argparse.ArgumentTypeError from e
```

### Comparing `corgy-6.0.0/corgy/_helpfmt.py` & `corgy-7.0.0/corgy/_helpfmt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from __future__ import annotations
 
-import importlib
+import argparse
 import inspect
 import re
-import shutil
 import sys
 import textwrap
-from argparse import (
-    Action,
-    ArgumentParser,
-    HelpFormatter,
-    ONE_OR_MORE,
-    PARSER,
-    SUPPRESS,
-    ZERO_OR_MORE,
-)
+from argparse import Action, ArgumentParser, HelpFormatter
 from collections.abc import Sequence as AbstractSequence
 from functools import lru_cache, partial
+from importlib import import_module
 from itertools import cycle, zip_longest
+from shutil import get_terminal_size
 from types import ModuleType
 from typing import Optional, Sequence, Tuple, Union
 from unittest.mock import patch
 
-from ._utils import get_concrete_collection_type, is_optional_type
+from ._actions import OptionalTypeAction
+from ._meta import get_concrete_collection_type, is_optional_type
 
 __all__ = ("CorgyHelpFormatter",)
 
 # These placeholders are used to replace special characters and words, so they can be
 # identified later for colorizing, without clashes with the help text. The code-points
 # are non-character points from `U+FDD0` to `U+FDEF`, which are guaranteed to never be
 # used for a character.
@@ -48,15 +42,15 @@
 # These markers are used by `argparse` to indicate metavar sequences, e.g.,
 # `[int ...]`, `int [int ...]`.
 _MARKER_METAVARS_BEGIN = "["
 _MARKER_METAVARS_END = "]"
 _MARKER_METAVARS_REPEAT = "..."
 
 
-class _ColorHelper:
+class ColorHelper:
     """Wrapper around `crayons` library to colorize text.
 
     Args:
         use_colors: Whether to enable colored output. If `None`, coloring is enabled
             if the `crayons` library is available, and the output is a tty.
         skip_tty_check: Whether to skip checking if the output is a tty. Only used if
             `use_colors` is None.
@@ -64,22 +58,22 @@
 
     __slots__ = ("crayons",)
     crayons: Optional[ModuleType]
 
     def __init__(self, use_colors: Optional[bool] = None, skip_tty_check: bool = False):
         if use_colors:
             try:
-                self.crayons = importlib.import_module("crayons")
+                self.crayons = import_module("crayons")
             except ImportError:
                 raise ImportError(
                     "`crayons` library is required to use colors"
                 ) from None
         elif use_colors is None and (skip_tty_check or sys.stdout.isatty()):
             try:
-                self.crayons = importlib.import_module("crayons")
+                self.crayons = import_module("crayons")
             except ImportError:
                 self.crayons = None
         else:
             self.crayons = None
 
     def colorize(self, text: str, color: str) -> str:
         """Colorize given text.
@@ -134,20 +128,21 @@
     """Formatter class for `argparse` with a cleaner layout, and support for colors.
 
     `Corgy.parse_from_cmdline` uses this formatter by default, unless a different
     `formatter_class` argument is provided. `CorgyHelpFormatter` can also be used
     independently of `Corgy`. Simply pass it as the `formatter_class` argument to
     `argparse.ArgumentParser()`::
 
-        >>> from argparse import ArgumentParser, SUPPRESS
+        >>> import argparse
+        >>> from argparse import ArgumentParser
         >>> from corgy import CorgyHelpFormatter
 
         >>> parser = ArgumentParser(
         ...     formatter_class=CorgyHelpFormatter,
-        ...     usage=SUPPRESS,
+        ...     usage=argparse.SUPPRESS,
         ... )
         >>> _ = parser.add_argument("--x", type=int, required=True)
         >>> _ = parser.add_argument("--y", type=str, nargs="*", required=True)
         >>> parser.print_help()
         options:
           -h/--help      show this help message and exit
           --x int        (required)
@@ -203,43 +198,43 @@
 
             >>> class T:
             ...     __metavar__ = "METAVAR"
 
             >>> parser = ArgumentParser(
             ...     formatter_class=CorgyHelpFormatter,
             ...     add_help=False,
-            ...     usage=SUPPRESS,
+            ...     usage=argparse.SUPPRESS,
             ... )
             >>> _ = parser.add_argument("--arg", type=T)
             >>> parser.print_help()
             options:
-              --arg METAVAR  (optional)
+              --arg METAVAR  (default: None)
 
     """
 
     use_colors: Optional[bool] = None
     color_choices = "blue"
     color_defaults = "YELLOW"
     color_keywords = "green"
     color_metavars = "RED"
     color_options = "BOLD"
 
     output_width: Optional[int] = None
-    max_help_position: Optional[int] = shutil.get_terminal_size().columns // 2
+    max_help_position: Optional[int] = get_terminal_size().columns // 2
 
     marker_extras_begin = "("
     marker_extras_end = ")"
     marker_choices_begin = "{"
     marker_choices_end = "}"
     marker_choices_sep = "/"
 
     show_full_help = True
 
     __slots__ = ("_color_helper",)
-    _color_helper: _ColorHelper
+    _color_helper: ColorHelper
 
     @property
     def using_colors(self) -> bool:
         """Whether colors are enabled."""
         return self._color_helper.crayons is not None
 
     # Regex to match a choice within a choice list, e.g., `b` in `{a/b/c}`.
@@ -302,23 +297,28 @@
                 return "None"
             return CorgyHelpFormatter._stringify(obj, type_.__args__[0])
 
         try:
             return obj.__name__  # type: ignore
         except AttributeError:
             try:
-                return type_.__str__(obj)
-            except:  # pylint: disable=bare-except
-                return str(obj)
+                if isinstance(obj, type_):
+                    return type_.__str__(obj)
+            except TypeError:
+                pass
+            return str(obj)
 
     @staticmethod
     def _get_stringify_type_for_default(action):
         """Get the type that should be used to stringify `action.default`."""
         _stringify_type = action.type
-        if isinstance(action.nargs, int) or action.nargs in (ZERO_OR_MORE, ONE_OR_MORE):
+        if isinstance(action.nargs, int) or action.nargs in (
+            argparse.ZERO_OR_MORE,
+            argparse.ONE_OR_MORE,
+        ):
             # If the argument specifies nargs, and the default value is a,
             # collection, wrap the action type with the default collection type.
             if isinstance(action.default, tuple):
                 _stringify_type = Tuple[action.type]  # type: ignore
             elif isinstance(action.default, AbstractSequence):
                 _stringify_type = Sequence[action.type]  # type: ignore
         return _stringify_type
@@ -439,17 +439,19 @@
 
     def _format_action_invocation(self, action: Action) -> str:
         """Format the invocation part of an argument, e.g. `-x, --x int`."""
         if action.option_strings:
             option_strings = action.option_strings
         else:
             # If no option strings are present, (positional arguments), use
-            # `action.dest`. However, this can be `SUPPRESS` for sub-actions, in which
-            # case use the word `CMD`.
-            option_strings = [action.dest if action.dest != SUPPRESS else "CMD"]
+            # `action.dest`. However, this can be `argparse.SUPPRESS` for sub-actions,
+            # in which case use the word `CMD`.
+            option_strings = [
+                action.dest if action.dest != argparse.SUPPRESS else "CMD"
+            ]
 
         if self.using_colors:
             # Create placeholders for the option strings, and store originals.
             placeholder_option_strings: Sequence[str] = [
                 _PLACEHOLDER_OPTION_STR * len(option_string)
                 for option_string in option_strings
             ]
@@ -464,15 +466,15 @@
             "option_strings",
             [self.marker_choices_sep.join(placeholder_option_strings)],
         ):
             return super()._format_action_invocation(action).rstrip()
 
     def _format_args(self, action: Action, default_metavar: Optional[str]) -> str:
         """Format the metavars."""
-        if action.nargs == PARSER:
+        if action.nargs == argparse.PARSER:
             # No metavars for a sub-command.
             return ""
 
         metavar = action.metavar or default_metavar or ""
 
         if self.using_colors:
             # Create a placeholder for the metavar, and store it in the action.
@@ -505,24 +507,34 @@
                 placeholder_metavar, metavar = _placeholderize_metavar(metavar)
             # Store the non-extra characters in the action, so they can be colorized
             # and substituted into the placeholder later.
             setattr(action, "_corgy_metavar", metavar)
         else:
             placeholder_metavar = metavar
 
-        with patch.object(action, "metavar", placeholder_metavar):
-            if action.nargs == ZERO_OR_MORE:
+        # For `corgy._corgy.OptionalTypeAction`s, use the true `nargs` for formatting.
+        _fmt_nargs = (
+            action._base_nargs
+            if isinstance(action, OptionalTypeAction)
+            else action.nargs
+        )
+        with patch.multiple(action, nargs=_fmt_nargs, metavar=placeholder_metavar):
+            if action.nargs == argparse.ZERO_OR_MORE:
                 # Python 3.9+ shows '*' argumets of a single type as `[<base_type> ...]`
                 # instead of `[<base_type> [<base_type> ...]]`. This code backports that
                 # functionality.
                 _mv = self._metavar_formatter(action, "")(1)
                 if len(_mv) == 2:
                     return f"[{_mv[0]} [{_mv[1]} ...]]"
                 return f"[{_mv[0]} ...]"
-            return super()._format_args(action, "")
+            _fmt = super()._format_args(action, "")
+            if isinstance(action, OptionalTypeAction):
+                # Add `[]` around the metavar.
+                _fmt = f"[{_fmt}]"
+            return _fmt
 
     def _format_action(self, action: Action) -> str:
         """Format a single argument.
 
         The superclass implementation produces an output like
         `  --arg ARG   arg help`.
 
@@ -570,15 +582,15 @@
                 arg_qualifier = (
                     _PLACEHOLDER_KWD_REQUIRED * len("required")
                     if self.using_colors
                     else "required"
                 )
             else:
                 arg_qualifier = ""
-        elif action.default is None or action.default is SUPPRESS:
+        elif action.default is argparse.SUPPRESS:
             if action.nargs == 0:
                 # The argument takes no values, so no need to explicitly indicate that
                 # it is optional. For example, help and version actions are obviously
                 # optional.
                 arg_qualifier = ""
             else:
                 arg_qualifier = (
@@ -616,15 +628,15 @@
                 + arg_qualifier
                 + marker_extras_end
             )
         else:
             extra_help = ""
 
         # Wrap the text according to `output_width` and `max_help_position`.
-        output_width = self.output_width or shutil.get_terminal_size().columns
+        output_width = self.output_width or get_terminal_size().columns
         max_help_position = self.max_help_position or output_width
         if len(base_fmt) + self._current_indent < min(output_width, max_help_position):
             # Example of desired result:
             #     --arg str  the help begins here,
             #                and continue here,
             #                and ends here (optional)
             indent = " " * len(base_fmt)
@@ -722,15 +734,15 @@
                 metavar = next(metavar_iter)
                 match_sub = self._sub_non_ws_with_colored_repl(
                     match, metavar, self.color_metavars
                 )
                 fmt = fmt[: match.start()] + match_sub + fmt[match.end() :]
 
         # Colorize the default value.
-        if action.default is not None and action.default != SUPPRESS:
+        if action.default != argparse.SUPPRESS:
             pattern = self._pattern_placeholder_text(_PLACEHOLDER_DEFAULT_VAL)
             _stringify_type = self._get_stringify_type_for_default(action)
             f_sub = partial(
                 self._sub_non_ws_with_colored_repl,
                 replacement=self._stringify(action.default, _stringify_type),
                 color=self.color_defaults,
             )
@@ -783,27 +795,27 @@
             current_frame = current_frame.f_back
 
     def _format_usage(self, usage: Optional[str], *args, **kwargs) -> str:
         with patch.object(self._color_helper, "crayons", None):
             # Disable colors for usage string.
             fmt = super()._format_usage(usage, *args, **kwargs)
 
-        output_width = self.output_width or shutil.get_terminal_size().columns
+        output_width = self.output_width or get_terminal_size().columns
         # Wrap usage to output width.
         fmt = textwrap.fill(
             fmt,
             width=output_width,
             subsequent_indent=" " * self._indent_increment,
             break_on_hyphens=False,
         )
         return fmt + "\n"
 
     def __init__(self, prog: str):
         # noqa: D107
-        self._color_helper = _ColorHelper(self.use_colors)
+        self._color_helper = ColorHelper(self.use_colors)
         # Wrapping is managed by this class, so pass `sys.maxsize` to the superclass.
         super().__init__(prog, max_help_position=sys.maxsize, width=sys.maxsize)
 
     class ShortHelpAction(Action):
         """`argparse.Action` that displays the short help, and exits."""
 
         def __call__(self, parser, namespace, values, option_string=None):
@@ -845,22 +857,30 @@
                 full help message and exit"`.
 
         Example::
 
             >>> parser = ArgumentParser(
             ...     formatter_class=CorgyHelpFormatter,
             ...     add_help=False,
-            ...     usage=SUPPRESS,
+            ...     usage=argparse.SUPPRESS,
             ... )
             >>> CorgyHelpFormatter.add_short_full_helps(parser)
             >>> parser.print_help()
             options:
               -h/--help   show help message and exit
               --helpfull  show full help message and exit
 
         """
         parser.add_argument(
-            *short_help_flags, nargs=0, action=cls.ShortHelpAction, help=short_help_msg
+            *short_help_flags,
+            nargs=0,
+            action=cls.ShortHelpAction,
+            help=short_help_msg,
+            default=argparse.SUPPRESS,
         )
         parser.add_argument(
-            *full_help_flags, nargs=0, action=cls.FullHelpAction, help=full_help_msg
+            *full_help_flags,
+            nargs=0,
+            action=cls.FullHelpAction,
+            help=full_help_msg,
+            default=argparse.SUPPRESS,
         )
```

### Comparing `corgy-6.0.0/docs/corgy.md` & `corgy-7.0.0/docs/corgy.md`

 * *Files 1% similar despite different names*

```diff
@@ -252,23 +252,19 @@
 >>> a = A(x=1)
 >>> del a.x
 Traceback (most recent call last):
     ...
 TypeError: attribute `x` cannot be unset
 ```
 
-Attributes can also explicitly be marked as required/not-required using the
-`Required` and `NotRequired` annotations:
+Attributes can also explicitly be marked as required/not-required using
+`corgy.Required` and `corgy.NotRequired` annotations:
 
 ```python
->>> import sys
->>> if sys.version_info >= (3, 11):
-...     from typing import Required, NotRequired
-... else:
-...     from typing_extensions import Required, NotRequired
+>>> from corgy import Required, NotRequired
 
 >>> class A(Corgy):
 ...     x: Required[int]
 ...     y: NotRequired[int]
 ...     z: int  # not required by default
 
 >>> a = A(x=1)
@@ -487,24 +483,25 @@
 the parameters for calling `ArgumentParser.add_argument`. These special
 annotations are described below.
 
 *Annotated*
 `typing.Annotated` can be used to add a help message for the argument:
 
 ```python
->>> from argparse import ArgumentParser, SUPPRESS
+>>> import argparse
+>>> from argparse import ArgumentParser
 >>> from corgy import CorgyHelpFormatter
 
 >>> class A(Corgy):
 ...     x: Annotated[int, "help for x"]
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 
 >>> A.add_args_to_parser(parser)
 >>> parser.print_help()
 options:
   --x int  help for x (optional)
 ```
@@ -518,15 +515,15 @@
 >>> class A(Corgy):
 ...     x: Annotated[int, "help for x", ["-x", "--ex"]]
 ...     y: Annotated[int, "help for y", ["y"]]
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 
 >>> A.add_args_to_parser(parser)
 >>> parser.print_help()
 positional arguments:
   y int        help for y
 
@@ -541,35 +538,37 @@
 *Required/NotRequired*
 Every corgy attribute is either required or not required. The default status
 depends on the class parameter `corgy_required_by_default` (`False` by default).
 Attributes can also be explicitly marked as required or not required, and will
 control whether the argument will be added with `required=True`:
 
 ```python
+>>> from corgy import Required, NotRequired
+
 >>> class A(Corgy):
 ...     x: Required[int]
 ...     y: NotRequired[int]
 ...     z: int
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 
 >>> A.add_args_to_parser(parser)
 >>> parser.print_help()
 options:
   --x int  (required)
   --y int  (optional)
   --z int  (optional)
 ```
 
 Attributes which are not required, and don’t have a default value are added
-with `default=SUPPRESS`, and so will not be included in the parsed namespace:
+with `default=argparse.SUPPRESS`, and so will not be in the parsed namespace:
 
 ```python
 >>> parser.parse_args(["--x", "1", "--y", "2"])
 Namespace(x=1, y=2)
 ```
 
 *Optional*
@@ -601,15 +600,15 @@
 ```python
 >>> class A(Corgy):
 ...     arg: bool
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 
 >>> A.add_args_to_parser(parser)
 >>> parser.print_help()
 options:
   --arg/--no-arg
 ```
@@ -656,15 +655,15 @@
 
 >>> class A(Corgy):
 ...     x: Literal[T1, T2]
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 
 >>> A.add_args_to_parser(parser)
 >>> parser.print_help()
 options:
   --x T  ({T1/T2} optional)
 ```
@@ -690,15 +689,15 @@
 >>> class A(Corgy):
 ...     x: int
 ...     g: G
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 
 >>> A.add_args_to_parser(parser)
 >>> parser.print_help()
 options:
   --x int      (optional)
 
@@ -891,15 +890,15 @@
     * **parser_args** – Arguments to be passed to `argparse.ArgumentParser()`. Ignored
     if `parser` is not None.
 
 
 
 * **Raises**
 
-    **ArgumentError** – Error parsing command line arguments.
+    **ArgumentTypeError** – Error parsing command line arguments.
 
 
 
 #### _classmethod_ parse_from_toml(toml_file, defaults=None)
 Parse an object of the class from a toml file.
 
 
@@ -994,27 +993,30 @@
     For all values other than `None`, the parsing function will receive a list
     of strings.
 
 
 Example:
 
 ```python
->>> from corgy import corgyparser
+>>> import argparse
+>>> from argparse import ArgumentParser
+>>> from typing import Tuple
+>>> from corgy import Corgy, CorgyHelpFormatter, corgyparser
 
 >>> class A(Corgy):
 ...     time: Tuple[int, int, int]
 ...     @corgyparser("time", metavar="int:int:int")
 ...     @staticmethod
 ...     def parse_time(s):
 ...         return tuple(map(int, s.split(":")))
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 
 >>> A.add_args_to_parser(parser)
 >>> parser.parse_args(["--time", "1:2:3"])
 Namespace(time=(1, 2, 3))
 ```
 
@@ -1058,15 +1060,15 @@
 ...     def parse_x(s):
 ...         # `s` will be a list of 3 strings.
 ...         return sum(map(int, s))
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 
 >>> A.add_args_to_parser(parser)
 >>> parser.parse_args(["--x", "1", "2", "3"])
 Namespace(x=6)
 ```
 
@@ -1079,20 +1081,21 @@
 
 `Corgy.parse_from_cmdline` uses this formatter by default, unless a different
 `formatter_class` argument is provided. `CorgyHelpFormatter` can also be used
 independently of `Corgy`. Simply pass it as the `formatter_class` argument to
 `argparse.ArgumentParser()`:
 
 ```python
->>> from argparse import ArgumentParser, SUPPRESS
+>>> import argparse
+>>> from argparse import ArgumentParser
 >>> from corgy import CorgyHelpFormatter
 
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 >>> _ = parser.add_argument("--x", type=int, required=True)
 >>> _ = parser.add_argument("--y", type=str, nargs="*", required=True)
 >>> parser.print_help()
 options:
   -h/--help      show this help message and exit
   --x int        (required)
@@ -1159,20 +1162,20 @@
     ```python
     >>> class T:
     ...     __metavar__ = "METAVAR"
 
     >>> parser = ArgumentParser(
     ...     formatter_class=CorgyHelpFormatter,
     ...     add_help=False,
-    ...     usage=SUPPRESS,
+    ...     usage=argparse.SUPPRESS,
     ... )
     >>> _ = parser.add_argument("--arg", type=T)
     >>> parser.print_help()
     options:
-      --arg METAVAR  (optional)
+      --arg METAVAR  (default: None)
     ```
 
 
 #### _property_ using_colors()
 Whether colors are enabled.
 
 
@@ -1223,20 +1226,20 @@
 
 Example:
 
 ```python
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 >>> CorgyHelpFormatter.add_short_full_helps(parser)
 >>> parser.print_help()
 options:
   -h/--help   show help message and exit
   --helpfull  show full help message and exit
 ```
 
-## Submodules
+## Subpackages
 
 
-* [corgy.types module](corgy.types.md)
+* [corgy.types package](corgy.types.md)
```

### Comparing `corgy-6.0.0/docs/corgy.types.md` & `corgy-7.0.0/docs/corgy.types.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# corgy.types module
+# corgy.types package
 
 Types for use with `corgy` (or standalone with `argparse`).
 
 An object of the types defined in this module can be created by calling the respective
 type class with a single string argument. `ValueError` is raised if the argument can not
 be converted to the desired type.
 
@@ -22,58 +22,82 @@
 >>> from corgy.types import SubClass
 >>> ASubClsType = SubClass[A]
 >>> a_subcls = ASubClsType("B")
 >>> a_subcls_obj = a_subcls()
 >>> a_subcls_obj
 <B object at 0x106cd93d0>
 
->>> from argparse import ArgumentParser, SUPPRESS
+>>> import argparse
+>>> from argparse import ArgumentParser
 >>> from corgy import CorgyHelpFormatter
 >>> from corgy.types import InputDirectory
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 >>> _ = parser.add_argument("--d", type=InputDirectory)
 >>> parser.print_help()
 options:
-  --d dir  (optional)
+  --d dir  (default: None)
 ```
 
 
-### _class_ corgy.types.OutputTextFile(path, \*\*kwargs)
-`TextIOWrapper` sub-class representing an output file.
+### _class_ corgy.types.ReadableFile(path)
+`Path` sub-class representing a readable file.
 
 
 * **Parameters**
 
+    **path** – String or path-like object.
 
-    * **path** – Path to a file.
 
+The provided path must point to an existing file, and the file must be readable.
+`ValueError` is raised otherwise.
 
-    * **kwargs** – Keyword only arguments that are passed to `TextIOWrapper`.
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
 
-The file will be created if it does not exist (including any parent directories),
-and opened in text mode (`w`). Existing files will be truncated. `ValueError`
-is raised if any of the operations fail. An `atexit` handler will be registered to
-close the file on program termination.
+### _class_ corgy.types.WritableFile(path)
+`Path` sub-class representing a writable file.
+
+
+* **Parameters**
+
+    **path** – String or path-like object.
 
 
-#### init()
-No-op for compatibility with `LazyOutputTextFile`.
+If the path exists, it must be a file, and it must be writable. If the path does
+not exist, the path’s directory must exist and be writable. `ValueError` is
+raised otherwise.
 
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
-#### _class property_ stdout_wrapper()
-`sys.__stdout__` wrapped with `TextIOWrapper` (line buffered).
 
+### _class_ corgy.types.OutputTextFile(path)
+`TextIOWrapper` sub-class representing an output file.
+
+
+* **Parameters**
+
+    **path** – Path to a file.
+
+
+The file will be created if it does not exist (including any parent directories),
+and opened in text mode (`w`). Existing files will be truncated. `ValueError`
+is raised if any of the operations fail. An `atexit` handler will be registered to
+close the file on program termination.
 
-#### _class property_ stderr_wrapper()
-`sys.__stderr__` wrapped with `TextIOWrapper` (line buffered).
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
 
 ### _class_ corgy.types.OutputBinFile(path)
 Type for an output binary file.
 
 
 * **Parameters**
@@ -83,61 +107,57 @@
 
 This class is a thin wrapper around `BufferedWriter` that accepts a path, instead
 of a file stream. The file will be created if it does not exist (including any
 parent directories), and opened in binary mode. Existing files will be truncated.
 `ValueError` is raised if any of the operations fail. An `atexit` handler
 will be registered to close the file on program termination.
 
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
-#### init()
-No-op for compatibility with `LazyOutputBinFile`.
 
-
-### _class_ corgy.types.LazyOutputTextFile(path, \*\*kwargs)
+### _class_ corgy.types.LazyOutputTextFile(path)
 `OutputTextFile` sub-class that does not auto-initialize.
 
 Useful for “default” files, which only need to be created if an alternative is not
 provided. `init` must be called on instances before they can be used.
 
-
-#### init()
-Initialize the file.
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
 
 ### _class_ corgy.types.LazyOutputBinFile(path)
 `OutputBinFile` sub-class that does not auto-initialize.
 
 Useful for “default” files, which only need to be created if an alternative is not
 provided. `init` must be called on instances before they can be used.
 
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
-#### init()
-Initialize the file.
 
-
-### _class_ corgy.types.InputTextFile(path, \*\*kwargs)
+### _class_ corgy.types.InputTextFile(path)
 `TextIOWrapper` sub-class representing an input file.
 
 
 * **Parameters**
 
-
-    * **path** – Path to a file.
-
-
-    * **kwargs** – Keyword only arguments that are passed to `TextIOWrapper`.
+    **path** – Path to a file.
 
 
 The file must exist, and will be opened in text mode (`r`). `ValueError` is
 raised if this fails. An `atexit` handler will be registered to close the file on
 program termination.
 
-
-#### _class property_ stdin_wrapper()
-`sys.__stdin__` wrapped with `TextIOWrapper`.
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
 
 ### _class_ corgy.types.InputBinFile(path)
 Type for an input binary file.
 
 
 * **Parameters**
@@ -146,69 +166,81 @@
 
 
 This class is a thin wrapper around `BufferedReader` that accepts a path, instead
 of a file stream. The file must exist, and will be opened in binary mode.
 `ValueError` is raised if this fails. An `atexit` handler will be registered
 to close the file on program termination.
 
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
+
 
 ### _class_ corgy.types.OutputDirectory(path)
 `Path` sub-class representing a directory to be written to.
 
 
 * **Parameters**
 
     **path** – Path to a directory.
 
 
 If the path does not exist, a directory with the path name will be created
 (including any parent directories). `ValueError` is raised if this fails, or
 if the path is not a directory, or if the directory is not writable.
 
-
-#### init()
-No-op for compatibility with `LazyOutputDirectory`.
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
 
 ### _class_ corgy.types.LazyOutputDirectory(path)
 `OutputDirectory` sub-class that does not auto-initialize.
 
 Useful for “default” folders, which only need to be created if an alternative is not
 provided. `init` must be called on instances to ensure that the directory exists.
 
-
-#### init()
-Initialize the directory.
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
 
 
 ### _class_ corgy.types.InputDirectory(path)
 `Path` sub-class representing a directory to be read from.
 
 
 * **Parameters**
 
     **path** – Path to a directory.
 
 
 The directory must exist, and will be checked to ensure it is readable.
 `ValueError` is raised if this is not the case.
 
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
+
 
 ### _class_ corgy.types.IODirectory(path)
 `Path` sub-class representing an existing directory to be read from/written to.
 
 
 * **Parameters**
 
     **path** – Path to a directory.
 
 
 The directory must exist, and will be checked to ensure it is readable and
 writeable. `ValueError` is raised if this is not the case.
 
+User directory and environment variable expansion is performed on the path.
+To disable this behavior, set class attributes `do_expanduser` and `do_expandvars`
+to `False` respectively.
+
 
 ### _class_ corgy.types.SubClass(name)
 Type representing a sub-class of a given class.
 
 Example:
 
 ```python
@@ -339,14 +371,16 @@
 
 ### _class_ corgy.types.KeyValuePairs(values)
 Dictionary sub-class that is initialized from a string of key-value pairs.
 
 Example:
 
 ```python
+>>> from corgy.types import KeyValuePairs
+
 >>> MapType = KeyValuePairs[str, int]
 >>> print(MapType("a=1,b=2"))
 {'a': 1, 'b': 2}
 ```
 
 This class supports the class indexing syntax to specify the types for keys and
 values. `KeyValuePairs[KT, VT]` returns a new `KeyValuePairs` type where the key
@@ -388,15 +422,16 @@
 
 ### _class_ corgy.types.InitArgs(\*\*args)
 Corgy wrapper around arguments of a class’s `__init__`.
 
 Example:
 
 ```python
->>> from argparse import ArgumentParser, SUPPRESS
+>>> import argparse
+>>> from argparse import ArgumentParser
 >>> from typing import Sequence
 >>> from corgy import CorgyHelpFormatter
 >>> from corgy.types import InitArgs
 
 >>> class Foo:
 ...     def __init__(
 ...         self,
@@ -406,15 +441,15 @@
 ...     ):
 ...         ...
 
 >>> FooInitArgs = InitArgs[Foo]
 >>> parser = ArgumentParser(
 ...     formatter_class=CorgyHelpFormatter,
 ...     add_help=False,
-...     usage=SUPPRESS,
+...     usage=argparse.SUPPRESS,
 ... )
 >>> FooInitArgs.add_args_to_parser(parser)
 >>> parser.print_help()
 options:
   --a int        (optional)
   --b [str ...]  (optional)
   --c float      (default: 0.0)
```

### Comparing `corgy-6.0.0/pyproject.toml` & `corgy-7.0.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 [tool.poetry]
 name = "corgy"
-version = "6.0.0"  # managed by `poetry-dynamic-versioning`
-description = "Elegant command line parsing"
-authors = ["Jayanth Koushik <jnkoushik@gmail.com>"]
+version = "7.0.0"  # managed by `poetry-dynamic-versioning`
+description = "Elegant data classes"
+authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jayanthkoushik/corgy"
 packages = [
-    { include = "corgy" },
-    { include = "tests", format = "sdist" }
+  { include = "corgy" },
 ]
-include = ["CHANGELOG.md", "example.png", "docs"]
+include = [
+  { path = "tests", format = "sdist" },
+  { path = "docs", format = "sdist" },
+  { path = "CHANGELOG.md", format = "sdist" },
+]
+exclude = ["docs/make.sh"]
 
 keywords = [
-    "argparse",
-    "argument parsing",
-    "command line parsing",
-    "cli",
+  "data classes",
+  "argparse",
+  "argument parsing",
+  "command line parsing",
+  "cli",
 ]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Natural Language :: English",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: User Interfaces",
-    "Topic :: Utilities",
+  "Development Status :: 5 - Production/Stable",
+  "Natural Language :: English",
+  "Operating System :: OS Independent",
+  "Intended Audience :: Developers",
+  "Topic :: Software Development :: User Interfaces",
+  "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 crayons = { version = "^0.4.0", optional = true }
 typing_extensions = { version = "^4.0", python = "<3.11" }
 tomli = {version = "^2.0.1", optional = true, python = "<3.11" }
@@ -69,38 +74,38 @@
 force_alphabetical_sort_within_sections = true
 
 [tool.pylint.FORMAT]
 max-line-length = "88"
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = """
-    fixme,
-    missing-docstring,
-    invalid-name,
-    ungrouped-imports,
-    wrong-import-order,
-    wrong-import-position,
-    import-outside-toplevel,
-    unused-argument,
-    no-self-use,
-    no-member,
-    protected-access,
-    attribute-defined-outside-init,
-    too-few-public-methods,
-    too-many-public-methods,
-    too-many-ancestors,
-    too-many-instance-attributes,
-    too-many-arguments,
-    too-many-locals,
-    too-many-statements,
-    too-many-lines,
-    too-many-branches,
-    too-many-nested-blocks,
-    too-many-return-statements,
-    too-many-boolean-expressions,
+  fixme,
+  missing-docstring,
+  invalid-name,
+  ungrouped-imports,
+  wrong-import-order,
+  wrong-import-position,
+  import-outside-toplevel,
+  unused-argument,
+  no-self-use,
+  no-member,
+  protected-access,
+  attribute-defined-outside-init,
+  too-few-public-methods,
+  too-many-public-methods,
+  too-many-ancestors,
+  too-many-instance-attributes,
+  too-many-arguments,
+  too-many-locals,
+  too-many-statements,
+  too-many-lines,
+  too-many-branches,
+  too-many-nested-blocks,
+  too-many-return-statements,
+  too-many-boolean-expressions,
 """
 
 [tool.pydocstyle]
 convention = "pep257"
 add-ignore = "D100,D101,D102,D103,D104,D105,D106,D107"
 
 [tool.mypy]
```

### Comparing `corgy-6.0.0/tests/test_corgy.py` & `corgy-7.0.0/tests/test_corgy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # pylint: disable=abstract-class-instantiated
 import argparse
 import sys
-import unittest
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, ArgumentTypeError
 from collections.abc import Sequence as AbstractSequence
-from functools import partial
 from io import BytesIO
 from typing import ClassVar, List, Optional, Sequence, Set, Tuple
-from unittest import skipIf
+from unittest import skipIf, TestCase
 from unittest.mock import MagicMock, patch
 
 SequenceType = Sequence
 TupleType = Tuple
 SetType = Set
 ListType = List
 
@@ -21,24 +20,21 @@
     Tuple = tuple  # type: ignore
     Set = set  # type: ignore
     List = list  # type: ignore
 else:
     from typing_extensions import Annotated, Literal
 
 import corgy
-from corgy import Corgy, CorgyHelpFormatter, corgyparser
-from corgy._corgy import _CorgyMeta, BooleanOptionalAction, CorgyParserAction
-from corgy._utils import get_concrete_collection_type, OptionalTypeAction
+from corgy import Corgy, CorgyHelpFormatter, corgyparser, NotRequired, Required
+from corgy._actions import BooleanOptionalAction, OptionalTypeAction
+from corgy._meta import CorgyMeta, get_concrete_collection_type
 
 if sys.version_info >= (3, 11):
     import tomllib as tomli
-    from typing import NotRequired, Required
 else:
-    from typing_extensions import NotRequired, Required
-
     try:
         import tomli
     except ImportError:
         tomli = None  # type: ignore
 
 COLLECTION_TYPES = [Sequence, Tuple, Set, List]
 
@@ -49,15 +45,15 @@
 def _get_collection_cast_type(_type) -> type:
     _cast_type = get_concrete_collection_type(_type)
     if _cast_type is AbstractSequence:
         return list
     return _cast_type  # type: ignore
 
 
-class TestCorgyMeta(unittest.TestCase):
+class TestCorgyMeta(TestCase):
     @classmethod
     def setUpClass(cls):
         class _CorgyCls(Corgy):
             x1: Sequence[int]
             x2: Annotated[int, "x2 docstr"]
             x3: int = 3
             x4: Annotated[str, "x4 docstr"] = "4"
@@ -317,15 +313,15 @@
             x: int
             y: Required[int]
             z: NotRequired[int]
 
         self.assertSetEqual(getattr(D, "__required"), {"y"})
 
 
-class TestCorgyClassInheritance(unittest.TestCase):
+class TestCorgyClassInheritance(TestCase):
     def test_corgy_cls_inherits_annotations_by_default(self):
         class C:
             x1: int
             x3: "str"
 
         class D(Corgy, C):
             x2: int
@@ -622,15 +618,15 @@
         class D3(C, Corgy):
             x: NotRequired[int]
             y: Required[int]
 
         self.assertSetEqual(getattr(D3, "__required"), {"y"})
 
 
-class TestCorgyTypeChecking(unittest.TestCase):
+class TestCorgyTypeChecking(TestCase):
     def test_corgy_cls_type_checks_during_init(self):
         class C(Corgy):
             x: int
 
         with self.assertRaises(ValueError):
             C(x="1")
 
@@ -836,15 +832,15 @@
             x: Literal
 
         c = C()
         with self.assertRaises(ValueError):
             c.x = 1
 
 
-class TestCorgyInit(unittest.TestCase):
+class TestCorgyInit(TestCase):
     def test_corgy_cls_init_assigns_values_to_attrs(self):
         class C(Corgy):
             x1: int
             x2: str
 
         c = C(x1=1, x2="2")
         self.assertEqual(c.x1, 1)
@@ -896,15 +892,15 @@
         class C(Corgy):
             g: Required[G]
 
         with self.assertRaises(ValueError):
             C()
 
 
-class TestCorgyAttrs(unittest.TestCase):
+class TestCorgyAttrs(TestCase):
     def test_corgy_cls_attrs_returns_dict_with_attr_types(self):
         class A(Corgy):
             x: int
             y: Sequence[str]
 
         self.assertDictEqual(A.attrs(), {"x": int, "y": Sequence[str]})
 
@@ -935,15 +931,15 @@
 
         class B(Corgy, A):
             y: str
 
         self.assertEqual(B.attrs(), {"x": int, "y": str})
 
 
-class TestCorgyAsDict(unittest.TestCase):
+class TestCorgyAsDict(TestCase):
     @classmethod
     def setUpClass(cls):
         class _CorgyCls(Corgy):
             x1: Sequence[int]
             x2: Annotated[int, "x2 docstr"]
             x3: int = 3
             x4: Annotated[str, "x4 docstr"] = "4"
@@ -1100,15 +1096,15 @@
 
         self.assertEqual(
             c.as_dict(recursive=True),
             {"x": ({"x": 1}, {"x": (1.1, [{"x": 10}, {"x": 20}, {"x": 30}], 2)})},
         )
 
 
-class TestCorgyFromDict(unittest.TestCase):
+class TestCorgyFromDict(TestCase):
     def test_cls_from_dict_creates_instance_from_dict(self):
         class C(Corgy):
             x: int
             y: str
 
         c = C.from_dict({"x": 1, "y": "two"})
         self.assertIsInstance(c, C)
@@ -1348,15 +1344,15 @@
         for _item in dir(bases[0]):
             if not _item.startswith("test_") or _item.endswith("_required"):
                 continue
             test_fn = getattr(bases[0], _item)
             new_test_fn_name = _item.replace("from_dict", "load_dict")
             namespace[new_test_fn_name] = test_fn
 
-        bases = (unittest.TestCase,)  # to prevent duplication of tests
+        bases = (TestCase,)  # to prevent duplication of tests
         return super().__new__(cls, name, bases, namespace, **kwds)
 
 
 class TestCorgyLoadDictIndirect(TestCorgyFromDict, metaclass=_LoadDictAsFromDictMeta):
     def setUp(self):
         def _load_as_from(cls, *args, **kwargs):
             c = cls()
@@ -1366,15 +1362,15 @@
         self._old_from_dict = Corgy.from_dict.__func__
         Corgy.from_dict = classmethod(_load_as_from)
 
     def tearDown(self):
         Corgy.from_dict = classmethod(self._old_from_dict)
 
 
-class TestCorgyLoadDict(unittest.TestCase):
+class TestCorgyLoadDict(TestCase):
     def test_load_dict_preserves_existing_values(self):
         class C(Corgy):
             x: int
             y: str
 
         c = C(x=1)
         c.load_dict({"y": "two"})
@@ -1469,15 +1465,15 @@
             x: Required[int]
 
         c = C(x=1)
         with self.assertRaises(TypeError):
             c.load_dict({}, strict=True)
 
 
-class TestCorgyPrinting(unittest.TestCase):
+class TestCorgyPrinting(TestCase):
     @classmethod
     def setUpClass(cls):
         class _CorgyCls(Corgy):
             x1: Sequence[int]
             x2: Annotated[int, "x2 docstr"]
             x3: int = 3
             x4: Annotated[str, "x4 docstr"] = "4"
@@ -1518,32 +1514,32 @@
         d1 = D(x=1, c=C(x=[0, 1]))
         d2 = eval(repr(d1))  # pylint: disable=eval-used
         self.assertEqual(d2.x, d1.x)
         self.assertEqual(d2.c.y, d1.c.y)
         self.assertListEqual(d2.c.x, d1.c.x)
 
 
-class TestCorgyAddArgsToParser(unittest.TestCase):
+class TestCorgyAddArgsToParser(TestCase):
     def setUp(self):
-        self.parser = argparse.ArgumentParser()
+        self.parser = ArgumentParser()
         self.parser.add_argument = MagicMock()
         self.parser.add_argument_group = MagicMock()
 
     @classmethod
     def setUpClass(cls):
         # Patch `CorgyMeta.__new__` to make `corgy_required_by_default` `True` if
         # not specified.
-        _old_new = _CorgyMeta.__new__
+        _old_new = CorgyMeta.__new__
 
         def _new(cls, name, bases, namespace, **kwargs):
             if "corgy_required_by_default" not in kwargs:
                 kwargs["corgy_required_by_default"] = True
             return _old_new(cls, name, bases, namespace, **kwargs)
 
-        cls._new_patcher = patch.object(_CorgyMeta, "__new__", _new)
+        cls._new_patcher = patch.object(CorgyMeta, "__new__", _new)
         cls._new_patcher.start()
 
     @classmethod
     def tearDownClass(cls):
         cls._new_patcher.stop()
 
     def test_add_args_raises_if_custom_flags_on_group(self):
@@ -1798,14 +1794,21 @@
             x: Literal[True, False]
 
         C.add_args_to_parser(self.parser)
         self.parser.add_argument.assert_called_once_with(
             "--x", type=bool, required=True, choices=(True, False)
         )
 
+    def test_add_args_handles_positional_bool(self):
+        class C(Corgy):
+            x: Annotated[bool, "x help", ["x"]]
+
+        C.add_args_to_parser(self.parser)
+        self.parser.add_argument.assert_called_once_with("x", type=bool, help="x help")
+
     def test_add_args_raises_if_coll_has_no_types(self):
         for _type in COLLECTION_TYPES:
             with self.subTest(type=_type):
 
                 class C(Corgy):
                     x: _type
 
@@ -1994,15 +1997,15 @@
             dest="the_grp:the_x_arg",
         )
 
     def test_add_args_handles_custom_flags_of_positional_args_inside_group(self):
         class G(Corgy):
             the_x_arg: Annotated[int, "x help", ["x", "the-x", "the_x_arg"]]
 
-        grp_parser = argparse.ArgumentParser()
+        grp_parser = ArgumentParser()
         grp_parser.add_argument = MagicMock()
         G.add_args_to_parser(grp_parser)
         grp_parser.add_argument.assert_called_once_with(
             "the_x_arg", type=int, help="x help"
         )
 
         class C(Corgy):
@@ -2266,17 +2269,17 @@
         class C(Corgy):
             x: Annotated[int, "x help", ["-x", "the-x"]]
 
         with self.assertRaises(TypeError):
             C.add_args_to_parser(self.parser)
 
 
-class TestCorgyAddRequiredArgsToParser(unittest.TestCase):
+class TestCorgyAddRequiredArgsToParser(TestCase):
     def setUp(self):
-        self.parser = argparse.ArgumentParser()
+        self.parser = ArgumentParser()
         self.parser.add_argument = MagicMock()
         self.parser.add_argument_group = MagicMock()
 
     def test_add_args_sets_required_true_for_required_attrs(self):
         class C(Corgy):
             x: Required[int]
 
@@ -2302,19 +2305,28 @@
     def test_add_args_handles_defaults_for_optional_attrs(self):
         class C(Corgy):
             x: NotRequired[int] = 1
 
         C.add_args_to_parser(self.parser)
         self.parser.add_argument.assert_called_once_with("--x", type=int, default=1)
 
+    def test_add_args_handles_optional_bool(self):
+        class C(Corgy):
+            x: NotRequired[bool]
+
+        C.add_args_to_parser(self.parser)
+        self.parser.add_argument.assert_called_once_with(
+            "--x", type=bool, action=BooleanOptionalAction, default=argparse.SUPPRESS
+        )
+
 
-class TestCorgyCmdlineParsing(unittest.TestCase):
+class TestCorgyCmdlineParsing(TestCase):
     def setUp(self):
-        self.parser = argparse.ArgumentParser()
-        self.orig_parse_args = argparse.ArgumentParser.parse_args
+        self.parser = ArgumentParser()
+        self.orig_parse_args = ArgumentParser.parse_args
 
     def test_cmdline_args_are_parsed_to_corgy_cls_properties(self):
         class C(Corgy):
             x: int
             y: str
             z: Sequence[int]
 
@@ -2328,37 +2340,37 @@
 
     def test_cmdline_args_are_parsed_with_custom_flags(self):
         class C(Corgy):
             var: Annotated[int, "x help", ["-x", "--the-x", "--the-x-arg"]]
 
         for flag in ["-x", "--the-x", "--the-x-arg"]:
             with self.subTest(flag=flag):
-                self.parser = argparse.ArgumentParser()
+                self.parser = ArgumentParser()
                 self.parser.parse_args = lambda: self.orig_parse_args(
                     self.parser, ["-x", "1"]
                 )
                 c = C.parse_from_cmdline(self.parser)
                 self.assertEqual(c.var, 1)
 
     def test_cmdline_positional_args_are_parsed_with_custom_flags(self):
         class C(Corgy):
             var: Annotated[int, "x help", ["x"]]
 
-        self.parser = argparse.ArgumentParser()
+        self.parser = ArgumentParser()
         self.parser.parse_args = lambda: self.orig_parse_args(self.parser, ["1"])
         c = C.parse_from_cmdline(self.parser)
         self.assertEqual(c.var, 1)
 
     def test_cmdline_positional_optional_args_are_pared_without_value(self):
         class C(Corgy):
             var: Annotated[Optional[int], "x help", ["x"]]
 
         for args in [[], ["1"]]:
             with self.subTest(args=args):
-                self.parser = argparse.ArgumentParser()
+                self.parser = ArgumentParser()
                 # pylint: disable=cell-var-from-loop
                 self.parser.parse_args = lambda: self.orig_parse_args(self.parser, args)
                 c = C.parse_from_cmdline(self.parser)
                 if not args:
                     self.assertIsNone(c.var)
                 else:
                     self.assertEqual(c.var, 1)
@@ -2382,15 +2394,15 @@
         self.assertEqual(c.g.x, 3)
         self.assertEqual(c.g.y, "four")
 
     def test_cmdline_parsing_handles_groups_with_positional_args(self):
         class G(Corgy):
             the_x_var: Annotated[int, "x help", ["x", "the_x", "the-x-var"]]
 
-        grp_parser = argparse.ArgumentParser()
+        grp_parser = ArgumentParser()
         grp_parser.parse_args = lambda: self.orig_parse_args(grp_parser, ["1"])
         g = G.parse_from_cmdline(grp_parser)
         self.assertEqual(g.the_x_var, 1)
 
         class C(Corgy):
             x: int
             g: G
@@ -2468,36 +2480,32 @@
         self.assertEqual(c.a.y, 2.3)
 
     def test_parse_from_cmdline_passes_extra_args_to_parser_constructor(self):
         class C(Corgy):
             x: int
 
         self.parser.parse_args = lambda: self.orig_parse_args(self.parser, ["--x", "1"])
-        with patch(
-            "corgy._corgy.argparse.ArgumentParser", MagicMock(return_value=self.parser)
-        ):
+        with patch("corgy._corgy.ArgumentParser", MagicMock(return_value=self.parser)):
             C.parse_from_cmdline(
-                formatter_class=argparse.ArgumentDefaultsHelpFormatter, add_help=False
+                formatter_class=ArgumentDefaultsHelpFormatter, add_help=False
             )
-            corgy._corgy.argparse.ArgumentParser.assert_called_once_with(
-                formatter_class=argparse.ArgumentDefaultsHelpFormatter, add_help=False
+            corgy._corgy.ArgumentParser.assert_called_once_with(
+                formatter_class=ArgumentDefaultsHelpFormatter, add_help=False
             )
 
     def test_parse_from_cmdline_uses_corgy_help_formatter_if_no_formatter_specified(
         self,
     ):
         class C(Corgy):
             x: int
 
         self.parser.parse_args = lambda: self.orig_parse_args(self.parser, ["--x", "1"])
-        with patch(
-            "corgy._corgy.argparse.ArgumentParser", MagicMock(return_value=self.parser)
-        ):
+        with patch("corgy._corgy.ArgumentParser", MagicMock(return_value=self.parser)):
             C.parse_from_cmdline(add_help=False)
-            corgy._corgy.argparse.ArgumentParser.assert_called_once_with(
+            corgy._corgy.ArgumentParser.assert_called_once_with(
                 formatter_class=CorgyHelpFormatter, add_help=False
             )
 
     def test_parse_from_cmdline_ignores_extra_arguments(self):
         class C(Corgy):
             x: int
 
@@ -2582,15 +2590,15 @@
                         self.parser, ["--x"]
                     )
                     c = C.parse_from_cmdline(self.parser, add_help=False)
                     self.assertEqual(c.x, None)
 
     def test_parse_from_cmdline_length_checks_optional_collection(self):
         def _raise_error(msg):
-            raise argparse.ArgumentError(None, msg)
+            raise ArgumentTypeError(None, msg)
 
         for _type in COLLECTION_TYPES:
             if _type in (SequenceType, ListType, SetType):
                 continue
 
             class C(Corgy):
                 x: Optional[_type[int, int, int]]
@@ -2599,507 +2607,34 @@
                 with self.subTest(type=_type, args=_args):
                     self.setUp()
                     self.parser.parse_args = lambda: self.orig_parse_args(
                         self.parser,
                         ["--x", *_args],  # pylint: disable=cell-var-from-loop
                     )
                     self.parser.error = _raise_error
-                    with self.assertRaises(argparse.ArgumentError):
+                    with self.assertRaises(ArgumentTypeError):
                         C.parse_from_cmdline(self.parser, add_help=False)
 
     def test_parse_from_cmdline_raises_on_missing_required_attrs(self):
         class C(Corgy):
             x: Required[int]
 
         self.parser.parse_args = lambda: self.orig_parse_args(self.parser, [])
 
         def _raise_error(msg):
-            raise argparse.ArgumentError(None, msg)
+            raise ArgumentTypeError(None, msg)
 
         self.parser.error = _raise_error
 
-        with self.assertRaises(argparse.ArgumentError):
+        with self.assertRaises(ArgumentTypeError):
             C.parse_from_cmdline(self.parser, add_help=False)
 
 
-class TestCorgyCustomParsers(unittest.TestCase):
-    def test_corgyparser_raises_if_not_passed_name(self):
-        with self.assertRaises(TypeError):
-
-            @corgyparser
-            def spam():
-                ...
-
-    def test_corgy_raises_if_corgyparser_target_invalid(self):
-        with self.assertRaises(TypeError):
-
-            class _(Corgy):
-                x: int
-
-                @corgyparser("y")
-                def parsex(s):  # type: ignore # pylint: disable=no-self-argument
-                    return 0
-
-    def test_corgy_raises_if_corgyparser_target_not_annotated(self):
-        with self.assertRaises(TypeError):
-
-            class _(Corgy):
-                x: int
-                y = 1
-
-                @corgyparser("y")
-                @staticmethod
-                def parsex(s):
-                    return 0
-
-    def test_corgy_raises_if_corgyparser_target_classvar(self):
-        with self.assertRaises(TypeError):
-
-            class _(Corgy):
-                x: ClassVar[int]
-
-                @corgyparser("x")
-                @staticmethod
-                def parsex(s):
-                    return 0
-
-    def test_corgyparser_raises_on_nargs_mismatch(self):
-        with self.assertRaises(TypeError):
-
-            class _(Corgy):
-                x: int
-                y: int
-
-                @corgyparser("x")
-                @corgyparser("y", nargs="+")
-                @staticmethod
-                def parsex(s):
-                    return 0
-
-        with self.assertRaises(TypeError):
-
-            class _(Corgy):
-                x: int
-                y: int
-
-                @corgyparser("x", nargs=2)
-                @corgyparser("y", nargs="*")
-                @staticmethod
-                def parsex(s):
-                    return 0
-
-    def test_add_args_handles_corgyparser(self):
-        class C(Corgy):
-            x: Annotated[int, "x"]
-
-            @corgyparser("x")
-            def parsex(s):  # type: ignore # pylint: disable=no-self-argument
-                return 0
-
-        parser = argparse.ArgumentParser()
-        parser.add_argument = MagicMock()
-        _parser_action = partial(CorgyParserAction, C.parsex)
-        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
-            C.add_args_to_parser(parser)
-        parser.add_argument.assert_called_once_with(
-            "--x", type=str, help="x", action=_parser_action, default=argparse.SUPPRESS
-        )
-
-    def test_add_args_with_custom_parser_respects_default_value(self):
-        class C(Corgy):
-            x: int = 1
-
-            @corgyparser("x")
-            def parsex(s):  # type: ignore # pylint: disable=no-self-argument
-                return 0
-
-        parser = argparse.ArgumentParser()
-        parser.add_argument = MagicMock()
-        _parser_action = partial(CorgyParserAction, C.parsex)
-        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
-            C.add_args_to_parser(parser)
-        parser.add_argument.assert_called_once_with(
-            "--x", type=str, default=1, action=_parser_action
-        )
-
-    def test_cmdline_parsing_calls_custom_parser(self):
-        class C(Corgy):
-            x: int
-
-            @corgyparser("x")
-            def parsex(s):  # type: ignore # pylint: disable=no-self-argument
-                return 0
-
-        getattr(C, "__parsers")["x"] = MagicMock(return_value=0)
-        parser = argparse.ArgumentParser()
-        orig_parse_args = argparse.ArgumentParser.parse_args
-        parser.parse_args = lambda: orig_parse_args(parser, ["--x", "test"])
-
-        C.parse_from_cmdline(parser)
-        getattr(C, "__parsers")["x"].assert_called_once_with("test")
-
-    def test_cmdline_parsing_calls_custom_parser_with_specified_nargs(self):
-        orig_parse_args = argparse.ArgumentParser.parse_args
-
-        def _run_and_check(cls, nargs, cmd_args, expected_call_args):
-            getattr(cls, "__parsers")["x"] = MagicMock(return_value=0, __nargs__=nargs)
-            parser = argparse.ArgumentParser()
-            parser.parse_args = lambda: orig_parse_args(parser, ["--x"] + cmd_args)
-            parser.error = MagicMock(side_effect=argparse.ArgumentTypeError)
-            cls.parse_from_cmdline(parser)
-            getattr(cls, "__parsers")["x"].assert_called_once_with(*expected_call_args)
-
-        for nargs in [None, "*", "+", 3]:
-
-            class C(Corgy):
-                x: int
-
-                @corgyparser("x", nargs=nargs)  # pylint: disable=cell-var-from-loop
-                @staticmethod
-                def parsex(s):
-                    return 0
-
-            if nargs is None:
-                _run_and_check(C, nargs, ["x"], ["x"])
-                # _run_and_check(C, [], [])
-                with self.assertRaises(argparse.ArgumentTypeError):
-                    _run_and_check(C, nargs, ["x", "y"], [["x", "y"]])
-            elif nargs == "*":
-                _run_and_check(C, nargs, ["x"], [["x"]])
-                _run_and_check(C, nargs, [], [[]])
-            elif nargs == "+":
-                _run_and_check(C, nargs, ["x"], [["x"]])
-                with self.assertRaises(argparse.ArgumentTypeError):
-                    _run_and_check(C, nargs, [], [])
-            else:
-                _run_and_check(C, nargs, ["x", "y", "z"], [["x", "y", "z"]])
-                with self.assertRaises(argparse.ArgumentTypeError):
-                    _run_and_check(C, nargs, ["x", "y"], [["x", "y"]])
-
-    def test_cmdline_parsing_returns_custom_parser_output(self):
-        class C(Corgy):
-            x: int
-
-            @corgyparser("x")
-            def parsex(s):  # type: ignore # pylint: disable=no-self-argument
-                return -1
-
-        parser = argparse.ArgumentParser()
-        orig_parse_args = argparse.ArgumentParser.parse_args
-        parser.parse_args = lambda: orig_parse_args(parser, ["--x", "test"])
-
-        args = C.parse_from_cmdline(parser)
-        self.assertEqual(args.x, -1)
-
-    def test_corgyparser_allows_decorating_staticmethod(self):
-        class C(Corgy):
-            x: int
-
-            @corgyparser("x")
-            @staticmethod
-            def parsex(s):
-                return 0
-
-        parser = argparse.ArgumentParser()
-        orig_parse_args = argparse.ArgumentParser.parse_args
-        parser.parse_args = lambda: orig_parse_args(parser, ["--x", "test"])
-
-        c = C.parse_from_cmdline(parser)
-        self.assertEqual(c.x, 0)
-
-    def test_corgyparser_raises_if_decorating_non_staticmethod(self):
-        with self.assertRaises(TypeError):
-
-            class _(Corgy):
-                x: int
-
-                @corgyparser("x")
-                @classmethod
-                def parsex(cls, s):
-                    return 0
-
-    def test_corgyparser_functions_are_callable(self):
-        class C(Corgy):
-            x: int
-            y: int
-
-            @corgyparser("x")
-            @staticmethod
-            def parsex(s):
-                return 0
-
-            @corgyparser("y")
-            def parsey(s):  # type: ignore # pylint: disable=no-self-argument
-                return 1
-
-        self.assertEqual(C.parsex("x"), 0)
-        self.assertEqual(C.parsey("y"), 1)
-
-    def test_corgyparser_accepts_multiple_arguments(self):
-        class C(Corgy):
-            x: int
-            y: int
-
-            @corgyparser("x", "y")
-            @staticmethod
-            def parsexy(s):
-                return 0
-
-        self.assertIs(getattr(C, "__parsers")["x"], getattr(C, "__parsers")["y"])
-
-    def test_corgyparser_decorators_can_be_chained(self):
-        class C(Corgy):
-            x: int
-            y: int
-
-            @corgyparser("x")
-            @corgyparser("y")
-            @staticmethod
-            def parsexy(s):
-                return 0
-
-        self.assertIs(getattr(C, "__parsers")["x"], getattr(C, "__parsers")["y"])
-
-    def test_corgyparser_allows_setting_metavar(self):
-        class C(Corgy):
-            x: int
-
-            @corgyparser("x", metavar="custom")
-            @staticmethod
-            def parsex(s):
-                return 0
-
-        parser = argparse.ArgumentParser()
-        parser.add_argument = MagicMock()
-        _parser_action = partial(CorgyParserAction, C.parsex)
-        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
-            C.add_args_to_parser(parser)
-        parser.add_argument.assert_called_once_with(
-            "--x",
-            type=str,
-            action=_parser_action,
-            default=argparse.SUPPRESS,
-            metavar="custom",
-        )
-
-    def test_corgyparser_handles_setting_metavar_with_chaining(self):
-        class C(Corgy):
-            x: int
-            y: int
-            z: int
-            w: int
-
-            @corgyparser("x")
-            @corgyparser("y", metavar="custom y")
-            @corgyparser("z")
-            @corgyparser("w", metavar="custom w")
-            @staticmethod
-            def parsexyzw(s):
-                return 0
-
-        self.assertEqual(C.parsexyzw.fparse.__metavar__, "custom y")
-
-    def test_add_args_with_custom_parser_uses_custom_metavar(self):
-        class T:
-            __metavar__ = "T"
-
-        class C(Corgy):
-            x: T
-
-            @corgyparser("x")
-            @staticmethod
-            def parsex(s):
-                return 0
-
-        parser = argparse.ArgumentParser()
-        parser.add_argument = MagicMock()
-        _parser_action = partial(CorgyParserAction, C.parsex)
-        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
-            C.add_args_to_parser(parser)
-        parser.add_argument.assert_called_once_with(
-            "--x",
-            type=str,
-            action=_parser_action,
-            default=argparse.SUPPRESS,
-            metavar="T",
-        )
-
-    def test_corgyparser_metavar_overrides_type_metavar(self):
-        class T:
-            __metavar__ = "T"
-
-        class C(Corgy):
-            x: T
-
-            @corgyparser("x", metavar="custom")
-            @staticmethod
-            def parsex(s):
-                return 0
-
-        parser = argparse.ArgumentParser()
-        parser.add_argument = MagicMock()
-        _parser_action = partial(CorgyParserAction, C.parsex)
-        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
-            C.add_args_to_parser(parser)
-        parser.add_argument.assert_called_once_with(
-            "--x",
-            type=str,
-            action=_parser_action,
-            default=argparse.SUPPRESS,
-            metavar="custom",
-        )
-
-    def test_corgy_cls_inherits_custom_parser(self):
-        class C(Corgy):
-            x: int
-
-            @corgyparser("x")
-            @staticmethod
-            def parsex(s):
-                return int(s[0]) + 1
-
-        class D(C):
-            ...
-
-        parser = argparse.ArgumentParser()
-        orig_parse_args = argparse.ArgumentParser.parse_args
-        parser.parse_args = lambda: orig_parse_args(parser, ["--x", "1"])
-
-        d = D.parse_from_cmdline(parser)
-        self.assertEqual(d.x, 2)
-
-    def test_corgy_cls_overrides_nargs_with_custom_parser(self):
-        class C1(Corgy):
-            x: Tuple[int]
-
-            @corgyparser("x")
-            @staticmethod
-            def parsex(s):
-                return 0
-
-        class C2(C1):
-            x: Tuple[int, ...]  # type: ignore
-
-        class C3(C1):
-            x: Tuple[int, int, int]  # type: ignore
-
-        for C in (C1, C2, C3):
-            with self.subTest(cls=C.__name__):
-                parser = argparse.ArgumentParser()
-                parser.add_argument = MagicMock()
-                _parser_action = partial(CorgyParserAction, C.parsex)
-                with patch(
-                    "corgy._corgy.partial", MagicMock(return_value=_parser_action)
-                ):
-                    C.add_args_to_parser(parser)
-                parser.add_argument.assert_called_once_with(
-                    "--x", type=str, default=argparse.SUPPRESS, action=_parser_action
-                )
-
-    def test_corgy_cls_respects_choices_with_custom_parser(self):
-        class C(Corgy):
-            x: Literal[1, 2, 3]
-
-            @corgyparser("x")
-            @staticmethod
-            def parsex(s):
-                return 1
-
-        parser = argparse.ArgumentParser()
-        parser.add_argument = MagicMock()
-        _parser_action = partial(CorgyParserAction, C.parsex)
-        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
-            C.add_args_to_parser(parser)
-        parser.add_argument.assert_called_once_with(
-            "--x",
-            type=str,
-            default=argparse.SUPPRESS,
-            action=_parser_action,
-            choices=(1, 2, 3),
-        )
-
-    def test_corgy_cls_respects_optional_with_custom_parser(self):
-        class C(Corgy):
-            x: Optional[int]
-
-            @corgyparser("x")
-            @staticmethod
-            def parsex(s):
-                return 0
-
-        parser = argparse.ArgumentParser()
-        parser.add_argument = MagicMock()
-        _parser_action = partial(CorgyParserAction, C.parsex)
-        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
-            C.add_args_to_parser(parser)
-        parser.add_argument.assert_called_once_with(
-            "--x", type=str, action=_parser_action, default=argparse.SUPPRESS
-        )
-
-    def test_cmdline_parsing_of_complex_nested_types_works_with_custom_parser(self):
-        class C(Corgy):
-            x: Tuple[Tuple[int, float], ...]
-
-            @corgyparser("x", nargs="*")
-            @staticmethod
-            def parsex(s_tup):
-                if not s_tup:
-                    raise ValueError
-                if len(s_tup) % 2:
-                    raise ValueError
-                o_list = []
-                for _i in range(len(s_tup) // 2):
-                    s = [s_tup[2 * _i], s_tup[2 * _i + 1]]
-                    o_list.append((int(s[0]), float(s[1])))
-                return tuple(o_list)
-
-        orig_parse_args = argparse.ArgumentParser.parse_args
-
-        def _run_with_args(*cmd_args):
-            parser = argparse.ArgumentParser()
-            parser.parse_args = lambda: orig_parse_args(
-                parser, ["--x"] + list(cmd_args)
-            )
-            args = C.parse_from_cmdline(parser)
-            return args.x
-
-        self.assertTupleEqual(_run_with_args("1", "2.1"), ((1, 2.1),))
-        self.assertTupleEqual(
-            _run_with_args("1", "2.1", "3", "4.1"), ((1, 2.1), (3, 4.1))
-        )
-        with self.assertRaises(argparse.ArgumentTypeError):
-            _run_with_args("1", "two")
-        with self.assertRaises(argparse.ArgumentTypeError):
-            _run_with_args("1.1", "2.1")
-        with self.assertRaises(argparse.ArgumentTypeError):
-            _run_with_args("1", "2.1", "3")
-        with self.assertRaises(argparse.ArgumentTypeError):
-            _run_with_args()
-
-    def test_custom_parsers_handle_required_attrs(self):
-        class C(Corgy):
-            x: Required[int]
-
-            @corgyparser("x")
-            @staticmethod
-            def parsex(s):
-                return int(s)
-
-        parser = argparse.ArgumentParser()
-        parser.add_argument = MagicMock()
-        _parser_action = partial(CorgyParserAction, C.parsex)
-        with patch("corgy._corgy.partial", MagicMock(return_value=_parser_action)):
-            C.add_args_to_parser(parser)
-        parser.add_argument.assert_called_once_with(
-            "--x", type=str, action=_parser_action, required=True
-        )
-
-
 @skipIf(tomli is None, "`tomli` package not found")
-class TestCorgyTomlParsing(unittest.TestCase):
+class TestCorgyTomlParsing(TestCase):
     def test_toml_file_parsed_to_corgy_object(self):
         class C(Corgy):
             x: int
 
         f = BytesIO(b"x = 1\n")
         c = C.parse_from_toml(f)
         self.assertEqual(c.x, 1)
@@ -3226,15 +2761,15 @@
                 return sum(map(int, s))
 
         f = BytesIO(b"x = [1, 2, 3]\n")
         c = C.parse_from_toml(f)
         self.assertEqual(c.x, 6)
 
 
-class TestCorgyEquality(unittest.TestCase):
+class TestCorgyEquality(TestCase):
     def test_corgy_instance_is_equal_to_itself(self):
         class A(Corgy):
             x: int
 
         a = A(x=1)
         self.assertEqual(a, a)
 
@@ -3338,15 +2873,15 @@
         c1 = C(y="2")
         c1.x = 1
         c2 = C(y="2")
         c2.x = 2
         self.assertEqual(c1, c2)
 
 
-class TestCorgyFreeze(unittest.TestCase):
+class TestCorgyFreeze(TestCase):
     def test_corgy_attrs_cannot_be_set_after_freeze(self):
         class A(Corgy):
             x: int
 
         a = A()
         a.freeze()
         with self.assertRaises(TypeError):
```

### Comparing `corgy-6.0.0/tests/test_helpfmt.py` & `corgy-7.0.0/tests/test_helpfmt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,39 @@
+import argparse
 import sys
-from argparse import ArgumentParser, SUPPRESS
+from argparse import ArgumentParser
 from typing import Optional
 from unittest import skipIf, TestCase
 from unittest.mock import Mock, patch
 
-from corgy import Corgy, CorgyHelpFormatter
-from corgy._corgy import BooleanOptionalAction
-from corgy._helpfmt import _ColorHelper
-from corgy.types import KeyValuePairs
-
 if sys.version_info < (3, 9):
     from typing import Sequence, Tuple
 else:
     from collections.abc import Sequence  # pylint: disable=reimported
 
     Tuple = tuple  # type: ignore
 
-if sys.version_info >= (3, 11):
-    from typing import NotRequired, Required
-else:
-    from typing_extensions import NotRequired, Required
+from corgy import Corgy, CorgyHelpFormatter, NotRequired, Required
+from corgy._corgy import BooleanOptionalAction
+from corgy._helpfmt import ColorHelper
+from corgy.types import KeyValuePairs
 
-_COLOR_HELPER = _ColorHelper(skip_tty_check=True)
+_COLOR_HELPER = ColorHelper(skip_tty_check=True)
 _CRAYONS = _COLOR_HELPER.crayons
 
 # Shortcuts for color functions to make ground truths in assert statements concise.
 _M = lambda s: _COLOR_HELPER.colorize(s, CorgyHelpFormatter.color_metavars)
 _K = lambda s: _COLOR_HELPER.colorize(s, CorgyHelpFormatter.color_keywords)
 _C = lambda s: _COLOR_HELPER.colorize(s, CorgyHelpFormatter.color_choices)
 _D = lambda s: _COLOR_HELPER.colorize(s, CorgyHelpFormatter.color_defaults)
 _O = lambda s: _COLOR_HELPER.colorize(s, CorgyHelpFormatter.color_options)
 
+# Shortcut for `default: None`.
+_DNone = lambda: f"{_K('default')}: {_D('None')}"
+
 # Make outputs independent of terminal width.
 CorgyHelpFormatter.output_width = 80
 CorgyHelpFormatter.max_help_position = 80
 
 
 def setUpModule():
     # The default choice list end markers, `{`, `}`, make f-strings messy, since they
@@ -47,25 +46,21 @@
     CorgyHelpFormatter.marker_choices_begin = "{"
     CorgyHelpFormatter.marker_choices_end = "}"
 
 
 class TestCorgyHelpFormatterAPI(TestCase):
     def test_corgy_help_formatter_raises_if_enabling_colors_without_crayons(self):
         CorgyHelpFormatter.use_colors = True
-        with patch(
-            "corgy._helpfmt.importlib.import_module", Mock(side_effect=ImportError)
-        ):
+        with patch("corgy._helpfmt.import_module", Mock(side_effect=ImportError)):
             with self.assertRaises(ImportError):
                 ArgumentParser(formatter_class=CorgyHelpFormatter)
 
     def test_corgy_help_formatter_doesnt_raise_if_use_colors_none_without_crayons(self):
         CorgyHelpFormatter.use_colors = None
-        with patch(
-            "corgy._helpfmt.importlib.import_module", Mock(side_effect=ImportError)
-        ):
+        with patch("corgy._helpfmt.import_module", Mock(side_effect=ImportError)):
             ArgumentParser(formatter_class=CorgyHelpFormatter)
 
     def test_corgy_help_formatter_raises_if_setting_new_attribute(self):
         with self.assertRaises(AttributeError):
             CorgyHelpFormatter.foo = "bar"
 
     @skipIf(_CRAYONS is None, "`crayons` package not found")
@@ -76,15 +71,17 @@
             color_choices="red",
             color_defaults="BLUE",
             color_keywords="BOLD",
             color_metavars="BLUE",
             color_options="yellow",
         ):
             parser = ArgumentParser(
-                formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+                formatter_class=CorgyHelpFormatter,
+                add_help=False,
+                usage=argparse.SUPPRESS,
             )
             parser.add_argument(
                 "--x", type=int, choices=[1, 2], help="x help", default=1
             )
 
             self.assertEqual(
                 parser.format_help(),
@@ -106,29 +103,35 @@
             marker_extras_begin="%",
             marker_extras_end="%",
             marker_choices_begin=" ( ",
             marker_choices_end=" ) ",
             marker_choices_sep="|",
         ):
             parser = ArgumentParser(
-                formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+                formatter_class=CorgyHelpFormatter,
+                add_help=False,
+                usage=argparse.SUPPRESS,
+            )
+            parser.add_argument(
+                "-x", "--x", type=int, choices=[1, 2], default=argparse.SUPPRESS
             )
-            parser.add_argument("-x", "--x", type=int, choices=[1, 2])
 
             self.assertEqual(
                 parser.format_help(), "options:\n  -x|--x int  % ( 1|2 )  optional%\n"
             )
 
     def test_corgy_help_formatter_handles_changing_output_width(self):
         CorgyHelpFormatter.use_colors = False
         with patch.object(CorgyHelpFormatter, "output_width", 10):
             parser = ArgumentParser(
                 formatter_class=CorgyHelpFormatter, add_help=False, prog=""
             )
-            parser.add_argument("--x", type=int, help="x help")
+            parser.add_argument(
+                "--x", type=int, help="x help", default=argparse.SUPPRESS
+            )
 
             self.assertEqual(
                 parser.format_help(),
                 "usage:\n"
                 "  [--x\n"
                 "  int]\n\n"
                 "options:\n"
@@ -139,31 +142,33 @@
                 "      iona\n"
                 "      l)\n",
             )
 
     def test_corgy_help_formatter_handles_changing_max_help_position(self):
         CorgyHelpFormatter.use_colors = False
         with patch.multiple(CorgyHelpFormatter, output_width=100, max_help_position=10):
-            parser = ArgumentParser(formatter_class=CorgyHelpFormatter, usage=SUPPRESS)
+            parser = ArgumentParser(
+                formatter_class=CorgyHelpFormatter, usage=argparse.SUPPRESS
+            )
             parser.add_argument(
                 "--x", type=int, metavar="A LONG METAVAR", help="x help"
             )
 
             self.assertEqual(
                 parser.format_help(),
                 # options:
                 #   -h/--help
                 #       show this help message and exit
                 #   --x A LONG METAVAR
-                #       x help (optional)
+                #       x help (default: None)
                 "options:\n"
                 "  -h/--help\n"
                 "      show this help message and exit\n"
                 "  --x A LONG METAVAR\n"
-                "      x help (optional)\n",
+                "      x help (default: None)\n",
             )
 
     def test_corgy_help_formatter_handles_changing_show_full_help(self):
         CorgyHelpFormatter.use_colors = False
         with patch.object(CorgyHelpFormatter, "show_full_help", False):
             parser = ArgumentParser(
                 formatter_class=CorgyHelpFormatter,
@@ -174,83 +179,85 @@
             parser.add_argument("--y", type=int, help="y help", choices=(1, 2))
             parser.add_argument("--z", type=int, help="z help", default=0)
 
             self.assertEqual(
                 parser.format_help(),
                 # options:
                 #   --x int  x help
-                #   --y int  y help (optional)
+                #   --y int  y help (default: None)
                 #   --z int  z help (default: 0)
                 "options:\n"
                 "  --x int  x help\n"
-                "  --y int  y help (optional)\n"
+                "  --y int  y help (default: None)\n"
                 "  --z int  z help (default: 0)\n",
             )
 
     @skipIf(_CRAYONS is None, "`crayons` package not found")
     def test_corgy_help_formatter_consistent_on_repeat_usage(self):
         CorgyHelpFormatter.use_colors = True
         parser = ArgumentParser(formatter_class=CorgyHelpFormatter, prog="")
         parser.add_argument("--x", type=int, choices=[1, 2])
 
         desired_output = (
             # usage: [-h] [--x int]
             #
             # options:
             #   -h/--help  show this help message and exit
-            #   --x int    ([1/2] optional)
+            #   --x int    ([1/2] default: None)
             f"usage: [-h] [--x int]\n\n"
             f"options:\n"
             f"  {_O('-h')}/{_O('--help')}  show this help message and exit\n"
-            f"  {_O('--x')} {_M('int')}    ([{_C(1)}/{_C(2)}] {_K('optional')})\n"
+            f"  {_O('--x')} {_M('int')}    ([{_C(1)}/{_C(2)}] {_DNone()})\n"
         )
 
         self.assertEqual(parser.format_help(), desired_output)
         self.assertEqual(parser.format_help(), desired_output)
 
         # Test with a new parser.
         parser = ArgumentParser(formatter_class=CorgyHelpFormatter, prog="")
         parser.add_argument("--x", type=int, choices=[1, 2])
         self.assertEqual(parser.format_help(), desired_output)
 
     @skipIf(_CRAYONS is None, "`crayons` package not found")
     def test_corgy_help_formatter_raises_if_using_invalid_color(self):
         with patch.object(CorgyHelpFormatter, "color_metavars", "ELUB"):
-            parser = ArgumentParser(formatter_class=CorgyHelpFormatter, usage=SUPPRESS)
+            parser = ArgumentParser(
+                formatter_class=CorgyHelpFormatter, usage=argparse.SUPPRESS
+            )
             parser.add_argument("--x", type=str)
             with self.assertRaises(ValueError):
                 parser.format_help()
 
 
 class TestCorgyHelpFormatterHelpActions(TestCase):
     def setUp(self):
         CorgyHelpFormatter.use_colors = False
         self.parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
         self.parser.print_help = Mock()
         self.parser.exit = Mock()
 
     def tearDown(self):
         CorgyHelpFormatter.show_full_help = True
 
     def test_corgy_help_formatter_short_help_action(self):
         self.parser.add_argument(
             "-h", nargs=0, action=CorgyHelpFormatter.ShortHelpAction
         )
-        self.parser.parse_args(["-h"])
+        self.parser.parse_args(["-h"])  # pylint: disable=too-many-function-args (???)
         self.parser.print_help.assert_called_once()
         self.parser.exit.assert_called_once()
         self.assertEqual(CorgyHelpFormatter.show_full_help, False)
 
     def test_corgy_help_formatter_full_help_action(self):
         self.parser.add_argument(
             "-h", nargs=0, action=CorgyHelpFormatter.FullHelpAction
         )
-        self.parser.parse_args(["-h"])
+        self.parser.parse_args(["-h"])  # pylint: disable=too-many-function-args (???)
         self.parser.print_help.assert_called_once()
         self.parser.exit.assert_called_once()
         self.assertEqual(CorgyHelpFormatter.show_full_help, True)
 
     def test_corgy_help_formatter_add_short_full_helps(self):
         self.parser.add_argument = Mock()
         CorgyHelpFormatter.add_short_full_helps(
@@ -262,31 +269,33 @@
         )
         self.parser.add_argument.assert_any_call(
             "-h",
             "--helpshort",
             nargs=0,
             action=CorgyHelpFormatter.ShortHelpAction,
             help="show short help",
+            default=argparse.SUPPRESS,
         )
         self.parser.add_argument.assert_any_call(
             "-H",
             "--helpfull",
             nargs=0,
             action=CorgyHelpFormatter.FullHelpAction,
             help="show full help",
+            default=argparse.SUPPRESS,
         )
 
 
 @skipIf(_CRAYONS is None, "`crayons` package not found")
 class TestCorgyHelpFormatterSingleArgs(TestCase):
     def setUp(self):
         _COLOR_HELPER.crayons = _CRAYONS
         CorgyHelpFormatter.use_colors = True
         self.parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
         self.maxDiff = None  # color codes can lead to very long diffs
 
     def _get_arg_help(self, *args, **kwargs):
         """Add a parser argument using `args` and `kwargs`, and return the help output.
 
         Only the output for the particular argument is returned.
@@ -309,60 +318,62 @@
             self._get_arg_help("--x", type=str, required=True),
             #   --x str  (required)
             f"  {_O('--x')} {_M('str')}  ({_K('required')})",
         )
 
     def test_corgy_help_formatter_handles_optional(self):
         self.assertEqual(
-            self._get_arg_help("--x", type=str),
+            self._get_arg_help("--x", type=str, default=argparse.SUPPRESS),
             #   --x str  (optional)
             f"  {_O('--x')} {_M('str')}  ({_K('optional')})",
         )
 
     def test_corgy_help_formatter_handles_default(self):
         self.assertEqual(
             self._get_arg_help("--x", type=str, default="def"),
             #   --x str  (default: def)
             f"  {_O('--x')} {_M('str')}  ({_K('default')}: {_D('def')})",
         )
 
     def test_corgy_help_formatter_handles_choices(self):
         self.assertEqual(
             self._get_arg_help("--x", type=str, choices=["a", "b"]),
-            #   --x str  ([a/b] optional)
-            f"  {_O('--x')} {_M('str')}  ([{_C('a')}/{_C('b')}] {_K('optional')})",
+            #   --x str  ([a/b] default: None)
+            f"  {_O('--x')} {_M('str')}  ([{_C('a')}/{_C('b')}] {_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_choices_with_default(self):
         self.assertEqual(
             self._get_arg_help("--x", type=str, default="def", choices=["a", "b"]),
             #  --x str  ([a/b] default: def)
             f"  {_O('--x')} {_M('str')}  ([{_C('a')}/{_C('b')}] "
             f"{_K('default')}: {_D('def')})",
         )
 
     def test_corgy_help_formatter_handles_help_text(self):
         self.assertEqual(
             self._get_arg_help("--x", help="x help", type=str),
-            #   --x str  x help (optional)
-            f"  {_O('--x')} {_M('str')}  x help ({_K('optional')})",
+            #   --x str  x help (default: None)
+            f"  {_O('--x')} {_M('str')}  x help ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_option_aliases(self):
         self.assertEqual(
             self._get_arg_help("-x", "--ex", "--between-y-and-z", type=str),
-            # -x/--ex/--between-y-and-z str  (optional)
+            # -x/--ex/--between-y-and-z str  (default: None)
             f"  {_O('-x')}/{_O('--ex')}/{_O('--between-y-and-z')} {_M('str')}  "
-            f"({_K('optional')})",
+            f"({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_long_option(self):
         with patch.object(CorgyHelpFormatter, "output_width", 10):
             self.assertEqual(
-                self._get_arg_help("--avery-long-argument-name", type=str),
+                self._get_arg_help(
+                    "--avery-long-argument-name", type=str, default=argparse.SUPPRESS
+                ),
                 #   --avery-
                 #     long-a
                 #     rgumen
                 #     t-name
                 #     str
                 #       (opt
                 #       iona
@@ -377,87 +388,88 @@
                 f"      {_K('l')})",
             )
 
     def test_corgy_help_formatter_handles_different_prefix_chars(self):
         with patch.object(self.parser, "prefix_chars", "+++"):
             self.assertEqual(
                 self._get_arg_help("+++x", type=str, help="x help"),
-                #   +++x str  x help (optional)
-                f"  {_O('+++x')} {_M('str')}  x help ({_K('optional')})",
+                #   +++x str  x help (default: None)
+                f"  {_O('+++x')} {_M('str')}  x help ({_DNone()})",
             )
 
     def test_corgy_help_formatter_handles_boolean_optional_action(self):
         self.assertEqual(
             self._get_arg_help(
                 "--x", action=BooleanOptionalAction, help="x help", default=True
             ),
             #   --x/--no-x  x help (default: True)
             f"  {_O('--x')}/{_O('--no-x')}  x help ({_K('default')}: {_D(True)})",
         )
 
     def test_corgy_help_formatter_handles_help_suppress(self):
         self.assertEqual(
-            self._get_arg_help("--x", type=str, help=SUPPRESS, default="def"), ""
+            self._get_arg_help("--x", type=str, help=argparse.SUPPRESS, default="def"),
+            "",
         )
 
     def test_corgy_help_formatter_handles_nargs_plus(self):
         self.assertEqual(
             self._get_arg_help("--x", nargs="+", type=str),
-            #   --x str [str ...]  (optional)
-            f"  {_O('--x')} {_M('str')} [{_M('str')} ...]  ({_K('optional')})",
+            #   --x str [str ...]  (default: None)
+            f"  {_O('--x')} {_M('str')} [{_M('str')} ...]  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_nargs_star(self):
         self.assertEqual(
             self._get_arg_help("--x", nargs="*", type=str),
-            f"  {_O('--x')} [{_M('str')} ...]  ({_K('optional')})",
+            f"  {_O('--x')} [{_M('str')} ...]  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_nargs_star_with_tuple_metavar(self):
         self.assertEqual(
             self._get_arg_help("--x", nargs="*", type=str, metavar=("a", "b")),
-            f"  {_O('--x')} [{_M('a')} [{_M('b')} ...]]  ({_K('optional')})",
+            f"  {_O('--x')} [{_M('a')} [{_M('b')} ...]]  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_nargs_const(self):
         self.assertEqual(
             self._get_arg_help("--x", nargs=3, type=str),
-            #   --x str str str  (optional)
-            f"  {_O('--x')} {_M('str')} {_M('str')} {_M('str')}  ({_K('optional')})",
+            #   --x str str str  (default: None)
+            f"  {_O('--x')} {_M('str')} {_M('str')} {_M('str')}  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_nargs_suppress(self):
         self.assertEqual(
-            self._get_arg_help("--x", nargs=SUPPRESS, type=str),
-            #   --x  (optional)
-            f"  {_O('--x')}  ({_K('optional')})",
+            self._get_arg_help("--x", nargs=argparse.SUPPRESS, type=str),
+            #   --x  (default: None)
+            f"  {_O('--x')}  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_tuple_metavar(self):
         self.assertEqual(
             self._get_arg_help("--x", metavar=("M1", "M2"), nargs=2),
-            #   --x M1 M2  (optional)
-            f"  {_O('--x')} {_M('M1')} {_M('M2')}  ({_K('optional')})",
+            #   --x M1 M2  (default: None)
+            f"  {_O('--x')} {_M('M1')} {_M('M2')}  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_tuple_metavar_with_nargs_plus(self):
         self.assertEqual(
             self._get_arg_help("--x", metavar=("M1", "M2"), nargs="+"),
-            #   --x M1 [M2 ...]  (optional)
-            f"  {_O('--x')} {_M('M1')} [{_M('M2')} ...]  ({_K('optional')})",
+            #   --x M1 [M2 ...]  (default: None)
+            f"  {_O('--x')} {_M('M1')} [{_M('M2')} ...]  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_custom_type(self):
         class CustomType:
             ...
 
         self.assertEqual(
             self._get_arg_help("--x", type=CustomType),
-            #   --x CustomType  (optional)
-            f"  {_O('--x')} {_M('CustomType')}  ({_K('optional')})",
+            #   --x CustomType  (default: None)
+            f"  {_O('--x')} {_M('CustomType')}  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_callable_type(self):
         def custom_type(s):
             return s
 
         self.assertEqual(
@@ -468,46 +480,46 @@
 
     def test_corgy_help_formatter_handles_custom_metavar(self):
         class CustomType:
             __metavar__ = "CUSTOM"
 
         self.assertEqual(
             self._get_arg_help("--x", type=CustomType),
-            #   --x CUSTOM  (optional)
-            f"  {_O('--x')} {_M('CUSTOM')}  ({_K('optional')})",
+            #   --x CUSTOM  (default: None)
+            f"  {_O('--x')} {_M('CUSTOM')}  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_missing_type(self):
         self.assertEqual(
             self._get_arg_help("--x", type=None),
-            #   --x  (optional)
-            f"  {_O('--x')}  ({_K('optional')})",
+            #   --x  (default: None)
+            f"  {_O('--x')}  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_bad_type(self):
         class T:
             def __call__(self):
                 ...
 
             def __str__(self):
                 return "BAD"
 
         self.assertEqual(
             self._get_arg_help("--x", type=T()),
-            #   --x BAD  (optional)
-            f"  {_O('--x')} {_M('BAD')}  ({_K('optional')})",
+            #   --x BAD  (default: None)
+            f"  {_O('--x')} {_M('BAD')}  ({_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_long_metavar(self):
         class CustomType:
             __metavar__ = "A-VERY-VERY-LONG-METAVAR"
 
         with patch.object(CorgyHelpFormatter, "output_width", 10):
             self.assertEqual(
-                self._get_arg_help("--x", type=CustomType),
+                self._get_arg_help("--x", type=CustomType, default=argparse.SUPPRESS),
                 #   --x A-VE
                 #     RY-VER
                 #     Y-LONG
                 #     -METAV
                 #     AR
                 #       (opt
                 #       iona
@@ -521,15 +533,20 @@
                 f"      {_K('iona')}\n"
                 f"      {_K('l')})",
             )
 
     def test_corgy_help_formatter_handles_long_help(self):
         with patch.object(CorgyHelpFormatter, "output_width", 15):
             self.assertEqual(
-                self._get_arg_help("--x", type=str, help="a very lengthy help"),
+                self._get_arg_help(
+                    "--x",
+                    type=str,
+                    help="a very lengthy help",
+                    default=argparse.SUPPRESS,
+                ),
                 #   --x str  a
                 #            very
                 #            leng
                 #            thy
                 #            help
                 #            (opt
                 #            iona
@@ -543,15 +560,20 @@
                 f"           {_K('iona')}\n"
                 f"           {_K('l')})",
             )
 
     def test_corgy_help_formatter_handles_long_help_with_small_max_help_pos(self):
         with patch.multiple(CorgyHelpFormatter, output_width=15, max_help_position=5):
             self.assertEqual(
-                self._get_arg_help("--x", type=str, help="a very lengthy help"),
+                self._get_arg_help(
+                    "--x",
+                    type=str,
+                    help="a very lengthy help",
+                    default=argparse.SUPPRESS,
+                ),
                 #   --x str
                 #       a very
                 #       lengthy
                 #       help (opt
                 #       ional)
                 f"  {_O('--x')} {_M('str')}\n"
                 f"      a very\n"
@@ -639,25 +661,25 @@
                 f"      {_C('choice')}/{_C('b')}]\n"
                 f"      {_K('default')}:\n"
                 f"      {_D('a')})",
             )
 
     def test_corgy_help_formatter_handles_default_suppress(self):
         self.assertEqual(
-            self._get_arg_help("--arg", type=str, default=SUPPRESS),
+            self._get_arg_help("--arg", type=str, default=argparse.SUPPRESS),
             f"  {_O('--arg')} {_M('str')}  ({_K('optional')})",
         )
 
     def test_corgy_help_formatter_uses_name_for_choices(self):
         class A:
             ...
 
         self.assertEqual(
             self._get_arg_help("--arg", choices=[A]),
-            f"  {_O('--arg')}  ([{_C('A')}] {_K('optional')})",
+            f"  {_O('--arg')}  ([{_C('A')}] {_DNone()})",
         )
 
     def test_corgy_help_formatter_uses_name_for_default(self):
         class A:
             ...
 
         self.assertEqual(
@@ -671,16 +693,15 @@
                 self.x = x
 
             def __repr__(self):
                 return f"A:{self.x}"
 
         self.assertEqual(
             self._get_arg_help("--arg", type=A, choices=[A(1), A("a")]),
-            f"  {_O('--arg')} {_M('A')}  ([{_C('A:1')}/{_C('A:a')}] "
-            f"{_K('optional')})",
+            f"  {_O('--arg')} {_M('A')}  ([{_C('A:1')}/{_C('A:a')}] " f"{_DNone()})",
         )
 
     def test_corgy_help_formatter_handles_dict_default(self):
         class T(KeyValuePairs[str, int]):  # type: ignore[misc]
             @classmethod
             def _metavar(cls) -> str:
                 return "T"
@@ -709,47 +730,53 @@
                 _C("'c':"),
                 " ",
                 _C("3}"),
             )
         )
         self.assertEqual(
             self._get_arg_help("--x", type=T, choices=(T("a=1"), T("b=2,c=3"))),
-            f"  {_O('--x')} {_M('T')}  ([{_choices_str}] {_K('optional')})",
+            f"  {_O('--x')} {_M('T')}  ([{_choices_str}] {_DNone()})",
         )
 
 
 @skipIf(_CRAYONS is None, "`crayons` package not found")
 class TestCorgyHelpFormatterMultiArgs(TestCase):
     def setUp(self):
         _COLOR_HELPER.crayons = _CRAYONS
         CorgyHelpFormatter.use_colors = True
-        self.parser = ArgumentParser(formatter_class=CorgyHelpFormatter, usage=SUPPRESS)
+        self.parser = ArgumentParser(
+            formatter_class=CorgyHelpFormatter, usage=argparse.SUPPRESS
+        )
         self.maxDiff = None
 
     def test_corgy_help_formatter_handles_multi_arg_alignment(self):
-        self.parser.add_argument("--x", type=int, help="x help")
+        self.parser.add_argument(
+            "--x", type=int, help="x help", default=argparse.SUPPRESS
+        )
         self.parser.add_argument("-y", "--why", type=float, required=True)
         self.parser.add_argument("-z", type=str, default="z", help="z help")
 
         self.assertEqual(
             self.parser.format_help(),
             # options:
             #   -h/--help       show this help message and exit
-            #   --x int         x help
+            #   --x int         x help (optional)
             #   -y/--why float  (required)
             #   -z str          z help (default: z)
             f"options:\n"
             f"  {_O('-h')}/{_O('--help')}       show this help message and exit\n"
             f"  {_O('--x')} {_M('int')}         x help ({_K('optional')})\n"
             f"  {_O('-y')}/{_O('--why')} {_M('float')}  ({_K('required')})\n"
             f"  {_O('-z')} {_M('str')}          z help ({_K('default')}: {_D('z')})\n",
         )
 
     def test_corgy_help_formatter_handles_multi_arg_wrapping(self):
-        self.parser.add_argument("-x", "--ex", type=float, help="help" * 10)
+        self.parser.add_argument(
+            "-x", "--ex", type=float, help="help" * 10, default=argparse.SUPPRESS
+        )
         with patch.object(CorgyHelpFormatter, "output_width", 30):
             self.assertEqual(
                 self.parser.format_help(),
                 # options:
                 #   -h/--help      show this
                 #                  help message
                 #                  and exit
@@ -777,52 +804,52 @@
                 #       show this help message and exit
                 #   -x/--ex float
                 #       helphelphelphelphelphelphelphelphelphelp (optional)
                 f"options:\n"
                 f"  {_O('-h')}/{_O('--help')}\n"
                 f"      show this help message and exit\n"
                 f"  {_O('-x')}/{_O('--ex')} {_M('float')}\n"
-                f"      helphelphelphelphelphelphelphelphelphelp ({_K('optional')})\n",
+                f"      helphelphelphelphelphelphelphelphelphelp ({_DNone()})\n",
             )
 
     def test_corgy_help_formatter_handles_argument_groups(self):
         self.parser.add_argument("arg", help="arg help")
         self.parser.add_argument("--x", type=str, help="x help")
         grp_parser = self.parser.add_argument_group("group 1")
         grp_parser.add_argument("--y", required=True)
         grp_parser.add_argument("--z", type=float)
         grp_parser = self.parser.add_argument_group("group 2", "group 2 description")
-        grp_parser.add_argument("--w", type=str)
+        grp_parser.add_argument("--w", type=str, default=argparse.SUPPRESS)
 
         self.assertEqual(
             self.parser.format_help(),
             # positional arguments:
             #   arg        arg help
             #
             # options:
             #   -h/--help  show this help message and exit
-            #   --x str    x help (optional)
+            #   --x str    x help (default: None)
             #
             # group 1:
             #   --y        (required)
-            #   --z float  (optional)
+            #   --z float  (default: None)
             #
             # group 2:
             #   group 2 description
             #   --w str    (optional)
             f"positional arguments:\n"
             f"  {_O('arg')}        arg help\n"
             f"\n"
             f"options:\n"
             f"  {_O('-h')}/{_O('--help')}  show this help message and exit\n"
-            f"  {_O('--x')} {_M('str')}    x help ({_K('optional')})\n"
+            f"  {_O('--x')} {_M('str')}    x help ({_DNone()})\n"
             f"\n"
             f"group 1:\n"
             f"  {_O('--y')}        ({_K('required')})\n"
-            f"  {_O('--z')} {_M('float')}  ({_K('optional')})\n"
+            f"  {_O('--z')} {_M('float')}  ({_DNone()})\n"
             f"\n"
             f"group 2:\n"
             f"  group 2 description\n"
             f"\n"
             f"  {_O('--w')} {_M('str')}    ({_K('optional')})\n",
         )
 
@@ -835,33 +862,33 @@
         self.assertEqual(
             self.parser.format_help(),
             # positional arguments:
             #   CMD        sub commands ([x/y])
             #
             # options:
             #   -h/--help  show this help message and exit
-            #   --arg str  (optional)
+            #   --arg str  (default: None)
             f"positional arguments:\n"
             f"  {_O('CMD')}        sub commands ([{_C('x')}/{_C('y')}])\n"
             f"\n"
             f"options:\n"
             f"  {_O('-h')}/{_O('--help')}  show this help message and exit\n"
-            f"  {_O('--arg')} {_M('str')}  ({_K('optional')})\n",
+            f"  {_O('--arg')} {_M('str')}  ({_DNone()})\n",
         )
 
 
 @skipIf(_CRAYONS is None, "`crayons` package not found")
 class TestCorgyHelpFormatterWithCorgyAnnotations(TestCase):
     def setUp(self):
         _COLOR_HELPER.crayons = _CRAYONS
         CorgyHelpFormatter.use_colors = True
 
     def _get_help_for_corgy_cls(self, corgy_cls):
         _parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
         corgy_cls.add_args_to_parser(_parser)
         _help = _parser.format_help()
         if _help:
             return _help.split("\n", maxsplit=1)[1].rstrip()
         return ""
 
@@ -1024,28 +1051,28 @@
             self._get_help_for_corgy_cls(C),
             f"  {_O('--x')} [[[{_M('T')}] ...] ...]  ({_K('default')}: "
             f"{_D('([T1, None], (None, T2))')})",
         )
 
     def test_corgy_help_formatter_handles_directly_added_bare_sequence(self):
         _parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
         _parser.add_argument("--x", type=Sequence, required=True)
         _help = _parser.format_help()
         if _help:
             _help = _help.split("\n", maxsplit=1)[1].rstrip()
 
         _tname = "typing.Sequence" if sys.version_info < (3, 9) else "Sequence"
         self.assertEqual(_help, f"  {_O('--x')} {_M(_tname)}  ({_K('required')})")
 
     def test_corgy_help_formatter_handles_directly_added_heterogenous_tuple(self):
         _T = Tuple[int, str, float]
         _parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
         _parser.add_argument("--x", type=_T, required=True)
         _help = _parser.format_help()
         if _help:
             _help = _help.split("\n", maxsplit=1)[1].rstrip()
 
         self.assertEqual(
@@ -1069,44 +1096,44 @@
             ...
 
         class T3(_TBase):
             ...
 
         _T = Tuple[T1, T2, T3]
         _parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
         _parser.add_argument("--x", type=_T, default=(T1(1), T2(2), T3(3)))
         _help = _parser.format_help()
         if _help:
             _help = _help.split("\n", maxsplit=1)[1].rstrip()
 
         self.assertEqual(
             _help,
             f"  {_O('--x')} {_M('T1')} {_M('T2')} {_M('T3')}"
             f"  ({_K('default')}: {_D('(T11, T22, T33)')})",
         )
 
         _parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
         _parser.add_argument("--x", type=_T, default=(T1(1), T2(2)))
         with self.assertRaises(ValueError):
             _parser.format_help()
 
     def test_corgy_help_formatter_handles_seq_default_for_non_seq_type(self):
         class T:
             def __init__(self, s):
                 self.s = s
 
             def __str__(self):
                 return "T" + self.s
 
         _parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
         _parser.add_argument("--x", type=T, default=[T("1"), T("2")])
         _help = _parser.format_help()
         if _help:
             _help = _help.split("\n", maxsplit=1)[1].rstrip()
 
         self.assertEqual(
@@ -1191,16 +1218,16 @@
                 self.parser.format_usage(),
                 # usage: [--arg str]
                 "usage: [--arg str]\n",
             )
             self.assertEqual(
                 self.parser.format_help(),
                 # options:
-                #   --arg str  (optional)
-                f"options:\n" f"  {_O('--arg')} {_M('str')}  ({_K('optional')})\n",
+                #   --arg str  (default: None)
+                f"options:\n" f"  {_O('--arg')} {_M('str')}  ({_DNone()})\n",
             )
 
 
 class _NoColorTestMeta(type):
     """Metaclass to create versions of test classes that don't use colors."""
 
     def __new__(cls, name, bases, namespace, **kwds):  # pylint: disable=duplicate-code
@@ -1222,25 +1249,27 @@
     # manually inherit needed base class methods.
     _get_arg_help = TestCorgyHelpFormatterSingleArgs._get_arg_help
 
     def setUp(self):
         _COLOR_HELPER.crayons = None
         CorgyHelpFormatter.use_colors = False
         self.parser = ArgumentParser(
-            formatter_class=CorgyHelpFormatter, add_help=False, usage=SUPPRESS
+            formatter_class=CorgyHelpFormatter, add_help=False, usage=argparse.SUPPRESS
         )
 
 
 class TestCorgyHelpFormatterMultiArgsNoColor(
     TestCorgyHelpFormatterMultiArgs, metaclass=_NoColorTestMeta
 ):
     def setUp(self):
         _COLOR_HELPER.crayons = None
         CorgyHelpFormatter.use_colors = False
-        self.parser = ArgumentParser(formatter_class=CorgyHelpFormatter, usage=SUPPRESS)
+        self.parser = ArgumentParser(
+            formatter_class=CorgyHelpFormatter, usage=argparse.SUPPRESS
+        )
 
 
 class TestCorgyHelpFormatterWithCorgyAnnotationsNoColor(
     TestCorgyHelpFormatterWithCorgyAnnotations, metaclass=_NoColorTestMeta
 ):
     _get_help_for_corgy_cls = (
         TestCorgyHelpFormatterWithCorgyAnnotations._get_help_for_corgy_cls
```

### Comparing `corgy-6.0.0/PKG-INFO` & `corgy-7.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: corgy
-Version: 6.0.0
-Summary: Elegant command line parsing
+Version: 7.0.0
+Summary: Elegant data classes
 Home-page: https://github.com/jayanthkoushik/corgy
 License: MIT
-Keywords: argparse,argument parsing,command line parsing,cli
+Keywords: data classes,argparse,argument parsing,command line parsing,cli
 Author: Jayanth Koushik
-Author-email: jnkoushik@gmail.com
+Author-email: mail@jkoushik.me
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

