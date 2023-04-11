# Comparing `tmp/pytypest-0.1.0.tar.gz` & `tmp/pytypest-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytypest-0.1.0.tar", last modified: Tue Apr 11 11:50:14 2023, max compression
+gzip compressed data, was "pytypest-1.0.0.tar", last modified: Tue Apr 11 12:17:54 2023, max compression
```

## Comparing `pytypest-0.1.0.tar` & `pytypest-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
--rw-r--r--   0        0        0       95 2023-04-04 11:31:55.259002 pytypest-0.1.0/.gitignore
--rw-r--r--   0        0        0      325 2023-03-15 11:14:58.709292 pytypest-0.1.0/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2023-03-15 11:14:58.705292 pytypest-0.1.0/LICENSE
--rw-r--r--   0        0        0     1196 2023-04-11 11:41:04.971735 pytypest-0.1.0/README.md
--rw-r--r--   0        0        0     3795 2023-04-04 11:20:52.164125 pytypest-0.1.0/Taskfile.yml
--rw-r--r--   0        0        0      648 2023-04-11 11:23:15.886640 pytypest-0.1.0/docs/api.md
--rw-r--r--   0        0        0      481 2023-04-07 08:31:31.406064 pytypest-0.1.0/docs/conf.py
--rw-r--r--   0        0        0      286 2023-04-07 10:03:44.441925 pytypest-0.1.0/docs/experimental.md
--rw-r--r--   0        0        0     4986 2023-04-07 09:48:51.821941 pytypest-0.1.0/docs/fixture.md
--rw-r--r--   0        0        0      819 2023-04-07 08:12:57.708705 pytypest-0.1.0/docs/fixtures.md
--rw-r--r--   0        0        0      236 2023-04-09 11:08:27.011713 pytypest-0.1.0/docs/index.md
--rw-r--r--   0        0        0     3498 2023-04-06 07:29:08.032613 pytypest-0.1.0/docs/motivation.md
--rw-r--r--   0        0        0     3551 2023-04-06 06:44:13.022673 pytypest-0.1.0/docs/parametrize.md
--rw-r--r--   0        0        0      614 2023-04-11 11:05:46.253127 pytypest-0.1.0/docs/recipes.md
--rw-r--r--   0        0        0        0 2023-03-13 09:10:32.373445 pytypest-0.1.0/integration/__init__.py
--rw-r--r--   0        0        0      604 2023-03-15 11:12:48.826448 pytypest-0.1.0/integration/test_args.py
--rw-r--r--   0        0        0      620 2023-03-15 11:12:48.826448 pytypest-0.1.0/integration/test_args_n_teardown.py
--rw-r--r--   0        0        0      512 2023-04-04 12:23:06.755963 pytypest-0.1.0/integration/test_attr.py
--rw-r--r--   0        0        0      461 2023-03-15 11:12:48.826448 pytypest-0.1.0/integration/test_parametrize.py
--rw-r--r--   0        0        0      749 2023-03-15 11:12:48.822448 pytypest-0.1.0/integration/test_scope_class.py
--rw-r--r--   0        0        0      183 2023-03-15 10:15:34.530881 pytypest-0.1.0/integration/test_simple.py
--rw-r--r--   0        0        0      415 2023-03-15 11:12:48.826448 pytypest-0.1.0/integration/test_teardown.py
--rw-r--r--   0        0        0      727 2023-03-15 11:12:48.826448 pytypest-0.1.0/integration/test_unwrap.py
--rw-r--r--   0        0        0     2003 2023-04-07 07:23:00.393574 pytypest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      417 2023-03-18 14:48:43.981074 pytypest-0.1.0/pytypest/__init__.py
--rw-r--r--   0        0        0      573 2023-03-23 13:03:15.225463 pytypest-0.1.0/pytypest/_autouse.py
--rw-r--r--   0        0        0     1704 2023-04-06 06:44:13.022673 pytypest-0.1.0/pytypest/_case.py
--rw-r--r--   0        0        0     3418 2023-04-06 06:44:13.022673 pytypest-0.1.0/pytypest/_fixture.py
--rw-r--r--   0        0        0     3919 2023-04-06 06:44:13.022673 pytypest-0.1.0/pytypest/_fixture_factory.py
--rw-r--r--   0        0        0      656 2023-04-06 06:44:13.022673 pytypest-0.1.0/pytypest/_hub.py
--rw-r--r--   0        0        0     1350 2023-04-06 06:44:13.022673 pytypest-0.1.0/pytypest/_manager.py
--rw-r--r--   0        0        0     1409 2023-04-06 06:44:13.022673 pytypest-0.1.0/pytypest/_parametrize.py
--rw-r--r--   0        0        0     1139 2023-03-17 12:46:39.555924 pytypest-0.1.0/pytypest/_plugin.py
--rw-r--r--   0        0        0      707 2023-04-07 09:56:33.555717 pytypest-0.1.0/pytypest/_scope.py
--rw-r--r--   0        0        0      601 2023-03-15 11:12:48.834448 pytypest-0.1.0/pytypest/_scope_manager.py
--rw-r--r--   0        0        0       86 2023-04-04 12:21:14.093205 pytypest-0.1.0/pytypest/experimental/__init__.py
--rw-r--r--   0        0        0     1295 2023-04-04 12:22:08.060603 pytypest-0.1.0/pytypest/experimental/_attr.py
--rw-r--r--   0        0        0     1383 2023-04-06 06:44:13.022673 pytypest-0.1.0/pytypest/experimental/_patcher.py
--rw-r--r--   0        0        0      620 2023-04-06 07:00:03.669764 pytypest-0.1.0/pytypest/fixtures/__init__.py
--rw-r--r--   0        0        0      598 2023-04-06 06:44:13.022673 pytypest-0.1.0/pytypest/fixtures/_helpers.py
--rw-r--r--   0        0        0     3076 2023-04-07 08:37:22.761582 pytypest-0.1.0/pytypest/fixtures/_misc.py
--rw-r--r--   0        0        0     5395 2023-04-07 08:38:24.872793 pytypest-0.1.0/pytypest/fixtures/_pytest.py
--rw-r--r--   0        0        0       66 2023-03-13 09:33:44.392708 pytypest-0.1.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-15 11:19:28.610448 pytypest-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      907 2023-03-17 12:46:44.731852 pytypest-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0      668 2023-03-17 12:46:44.731852 pytypest-0.1.0/tests/test_autouse.py
--rw-r--r--   0        0        0     1207 2023-04-04 12:22:03.072658 pytypest-0.1.0/tests/test_experimental.py
--rw-r--r--   0        0        0     6286 2023-04-07 08:04:58.519726 pytypest-0.1.0/tests/test_fixtrues.py
--rw-r--r--   0        0        0     2051 2023-04-04 12:20:36.469634 pytypest-0.1.0/tests/test_fixture.py
--rw-r--r--   0        0        0     1185 2023-04-11 11:05:20.027797 pytypest-0.1.0/tests/test_parametrize.py
--rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 pytypest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1121 2023-04-11 12:17:10.353741 pytypest-1.0.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       95 2023-04-04 11:31:55.259002 pytypest-1.0.0/.gitignore
+-rw-r--r--   0        0        0      325 2023-03-15 11:14:58.709292 pytypest-1.0.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2023-03-15 11:14:58.705292 pytypest-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1331 2023-04-11 12:01:06.546979 pytypest-1.0.0/README.md
+-rw-r--r--   0        0        0     3795 2023-04-04 11:20:52.164125 pytypest-1.0.0/Taskfile.yml
+-rw-r--r--   0        0        0      648 2023-04-11 11:23:15.886640 pytypest-1.0.0/docs/api.md
+-rw-r--r--   0        0        0      481 2023-04-07 08:31:31.406064 pytypest-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0      286 2023-04-07 10:03:44.441925 pytypest-1.0.0/docs/experimental.md
+-rw-r--r--   0        0        0     4986 2023-04-07 09:48:51.821941 pytypest-1.0.0/docs/fixture.md
+-rw-r--r--   0        0        0      819 2023-04-07 08:12:57.708705 pytypest-1.0.0/docs/fixtures.md
+-rw-r--r--   0        0        0      334 2023-04-11 12:01:38.442612 pytypest-1.0.0/docs/index.md
+-rw-r--r--   0        0        0     3498 2023-04-06 07:29:08.032613 pytypest-1.0.0/docs/motivation.md
+-rw-r--r--   0        0        0     3551 2023-04-06 06:44:13.022673 pytypest-1.0.0/docs/parametrize.md
+-rw-r--r--   0        0        0      614 2023-04-11 11:05:46.253127 pytypest-1.0.0/docs/recipes.md
+-rw-r--r--   0        0        0        0 2023-03-13 09:10:32.373445 pytypest-1.0.0/integration/__init__.py
+-rw-r--r--   0        0        0      604 2023-03-15 11:12:48.826448 pytypest-1.0.0/integration/test_args.py
+-rw-r--r--   0        0        0      620 2023-03-15 11:12:48.826448 pytypest-1.0.0/integration/test_args_n_teardown.py
+-rw-r--r--   0        0        0      512 2023-04-04 12:23:06.755963 pytypest-1.0.0/integration/test_attr.py
+-rw-r--r--   0        0        0      461 2023-03-15 11:12:48.826448 pytypest-1.0.0/integration/test_parametrize.py
+-rw-r--r--   0        0        0      749 2023-03-15 11:12:48.822448 pytypest-1.0.0/integration/test_scope_class.py
+-rw-r--r--   0        0        0      183 2023-03-15 10:15:34.530881 pytypest-1.0.0/integration/test_simple.py
+-rw-r--r--   0        0        0      415 2023-03-15 11:12:48.826448 pytypest-1.0.0/integration/test_teardown.py
+-rw-r--r--   0        0        0      727 2023-03-15 11:12:48.826448 pytypest-1.0.0/integration/test_unwrap.py
+-rwxr-xr-x   0        0        0      107 2023-04-11 11:54:12.366727 pytypest-1.0.0/netlify.sh
+-rw-r--r--   0        0        0       95 2023-04-11 11:54:12.370727 pytypest-1.0.0/netlify.toml
+-rw-r--r--   0        0        0     2034 2023-04-11 12:17:10.353741 pytypest-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      417 2023-04-11 12:17:38.397238 pytypest-1.0.0/pytypest/__init__.py
+-rw-r--r--   0        0        0      573 2023-03-23 13:03:15.225463 pytypest-1.0.0/pytypest/_autouse.py
+-rw-r--r--   0        0        0     1734 2023-04-11 12:17:10.353741 pytypest-1.0.0/pytypest/_case.py
+-rw-r--r--   0        0        0     3448 2023-04-11 12:17:10.353741 pytypest-1.0.0/pytypest/_fixture.py
+-rw-r--r--   0        0        0     3953 2023-04-11 12:17:10.353741 pytypest-1.0.0/pytypest/_fixture_factory.py
+-rw-r--r--   0        0        0      656 2023-04-06 06:44:13.022673 pytypest-1.0.0/pytypest/_hub.py
+-rw-r--r--   0        0        0     1350 2023-04-06 06:44:13.022673 pytypest-1.0.0/pytypest/_manager.py
+-rw-r--r--   0        0        0     1438 2023-04-11 12:17:10.353741 pytypest-1.0.0/pytypest/_parametrize.py
+-rw-r--r--   0        0        0     1139 2023-03-17 12:46:39.555924 pytypest-1.0.0/pytypest/_plugin.py
+-rw-r--r--   0        0        0      707 2023-04-07 09:56:33.555717 pytypest-1.0.0/pytypest/_scope.py
+-rw-r--r--   0        0        0      601 2023-03-15 11:12:48.834448 pytypest-1.0.0/pytypest/_scope_manager.py
+-rw-r--r--   0        0        0       86 2023-04-04 12:21:14.093205 pytypest-1.0.0/pytypest/experimental/__init__.py
+-rw-r--r--   0        0        0     1325 2023-04-11 12:17:10.353741 pytypest-1.0.0/pytypest/experimental/_attr.py
+-rw-r--r--   0        0        0     1383 2023-04-06 06:44:13.022673 pytypest-1.0.0/pytypest/experimental/_patcher.py
+-rw-r--r--   0        0        0      620 2023-04-06 07:00:03.669764 pytypest-1.0.0/pytypest/fixtures/__init__.py
+-rw-r--r--   0        0        0      598 2023-04-06 06:44:13.022673 pytypest-1.0.0/pytypest/fixtures/_helpers.py
+-rw-r--r--   0        0        0     3076 2023-04-07 08:37:22.761582 pytypest-1.0.0/pytypest/fixtures/_misc.py
+-rw-r--r--   0        0        0     5395 2023-04-07 08:38:24.872793 pytypest-1.0.0/pytypest/fixtures/_pytest.py
+-rw-r--r--   0        0        0       66 2023-03-13 09:33:44.392708 pytypest-1.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-03-15 11:19:28.610448 pytypest-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      907 2023-03-17 12:46:44.731852 pytypest-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      668 2023-03-17 12:46:44.731852 pytypest-1.0.0/tests/test_autouse.py
+-rw-r--r--   0        0        0     1207 2023-04-04 12:22:03.072658 pytypest-1.0.0/tests/test_experimental.py
+-rw-r--r--   0        0        0     6286 2023-04-07 08:04:58.519726 pytypest-1.0.0/tests/test_fixtrues.py
+-rw-r--r--   0        0        0     2051 2023-04-04 12:20:36.469634 pytypest-1.0.0/tests/test_fixture.py
+-rw-r--r--   0        0        0     1185 2023-04-11 11:05:20.027797 pytypest-1.0.0/tests/test_parametrize.py
+-rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pytypest-1.0.0/PKG-INFO
```

### Comparing `pytypest-0.1.0/LICENSE` & `pytypest-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/README.md` & `pytypest-1.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pytypest
 
-Type-safe and maintainable fixtures and parametrization for pytest.
+Type-safe and maintainable fixtures and parametrization for [pytest](https://github.com/pytest-dev/pytest).
 
 Features:
 
 + 100% type safe.
-+ Great IDE integration, go-todefinition always takes you in the right place.
++ Great IDE integration, go-to-definition always takes you in the right place.
 + Test parametrization that is redable even with many arguments.
 + Plug-and-play integration with pytest.
 + No vendor-lock, you can use only the features you need and don't touch the rest.
 + Fixtures can be cached, and you are in control of for how long.
 + Fixtures can accept arguments.
 
 ## Installation
@@ -35,7 +35,9 @@
 
 def test_user() -> None:
     u = get_user(anonymous=False)
     assert u.anonymous is False
 ```
 
 Compared to built-in pytest fixtures, these are explicit, type-safe, can accept arguments, support go-to-definition in IDE, and can be used as context managers. And like pytest fixtures, they are cached and can be scoped to the module or the whole session.
+
+Read more in the **documentation**: [pytypest.orsinium.dev](https://pytypest.orsinium.dev/).
```

### Comparing `pytypest-0.1.0/Taskfile.yml` & `pytypest-1.0.0/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/docs/api.md` & `pytypest-1.0.0/docs/api.md`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/docs/fixture.md` & `pytypest-1.0.0/docs/fixture.md`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/docs/fixtures.md` & `pytypest-1.0.0/docs/fixtures.md`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/docs/motivation.md` & `pytypest-1.0.0/docs/motivation.md`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/docs/parametrize.md` & `pytypest-1.0.0/docs/parametrize.md`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/docs/recipes.md` & `pytypest-1.0.0/docs/recipes.md`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/integration/test_args.py` & `pytypest-1.0.0/integration/test_args.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/integration/test_args_n_teardown.py` & `pytypest-1.0.0/integration/test_args_n_teardown.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/integration/test_attr.py` & `pytypest-1.0.0/integration/test_attr.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/integration/test_scope_class.py` & `pytypest-1.0.0/integration/test_scope_class.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/integration/test_unwrap.py` & `pytypest-1.0.0/integration/test_unwrap.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pyproject.toml` & `pytypest-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,18 @@
 keywords = [
     "pytest",
     "tests",
     "testing",
     "framework",
     "fixtures",
 ]
-dependencies = ["pytest"]
+dependencies = [
+    "pytest",
+    "typing-extensions",
+]
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
     "requests",
 ]
@@ -48,15 +51,15 @@
 
 
 [project.urls]
 Source = "https://github.com/orsinium-labs/pytypest"
 
 [tool.mypy]
 files = ["pytypest", "tests", "integration"]
-python_version = "3.10"
+python_version = "3.8"
 ignore_missing_imports = true
 # follow_imports = "silent"
 show_error_codes = true
 check_untyped_defs = true
 no_implicit_optional = true
 strict_equality = true
 warn_redundant_casts = true
```

### Comparing `pytypest-0.1.0/pytypest/_autouse.py` & `pytypest-1.0.0/pytypest/_autouse.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/_case.py` & `pytypest-1.0.0/pytypest/_case.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
-from typing import Any, Generic, ParamSpec, TypeVar
+from typing import Any, Generic, TypeVar
+
+from typing_extensions import ParamSpec
 
 
 P = ParamSpec('P')
 S = TypeVar('S')
 
 
 @dataclasses.dataclass(frozen=True)
```

### Comparing `pytypest-0.1.0/pytypest/_fixture.py` & `pytypest-1.0.0/pytypest/_fixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import inspect
 from dataclasses import dataclass, field
 from enum import Enum
-from typing import Callable, Generic, Iterator, Literal, ParamSpec, TypeVar
+from typing import Callable, Generic, Iterator, Literal, TypeVar
+
+from typing_extensions import ParamSpec
 
 from ._manager import defer
 from ._scope import Scope
 
 
 R = TypeVar('R')
 P = ParamSpec('P')
```

### Comparing `pytypest-0.1.0/pytypest/_fixture_factory.py` & `pytypest-1.0.0/pytypest/_fixture_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from typing import TYPE_CHECKING, Protocol, overload
 
 from ._fixture import Fixture
 from ._scope import Scope
 
 
 if TYPE_CHECKING:
-    from typing import Callable, Iterator, Literal, ParamSpec, TypeVar
+    from typing import Callable, Iterator, Literal, TypeVar
+
+    from typing_extensions import ParamSpec
 
     R = TypeVar('R')
     P = ParamSpec('P')
 
 
 class FixtureMaker(Protocol):
     """
```

### Comparing `pytypest-0.1.0/pytypest/_hub.py` & `pytypest-1.0.0/pytypest/_hub.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/_manager.py` & `pytypest-1.0.0/pytypest/_manager.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/_parametrize.py` & `pytypest-1.0.0/pytypest/_parametrize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import inspect
-from typing import TYPE_CHECKING, Callable, ParamSpec
+from typing import TYPE_CHECKING, Callable
 
 import pytest
+from typing_extensions import ParamSpec
 
 from ._case import Case
 
 
 if TYPE_CHECKING:
     from _pytest.mark import ParameterSet
```

### Comparing `pytypest-0.1.0/pytypest/_plugin.py` & `pytypest-1.0.0/pytypest/_plugin.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/_scope.py` & `pytypest-1.0.0/pytypest/_scope.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/_scope_manager.py` & `pytypest-1.0.0/pytypest/_scope_manager.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/experimental/_attr.py` & `pytypest-1.0.0/pytypest/experimental/_attr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, Generic, ParamSpec, TypeVar, overload
+from typing import TYPE_CHECKING, Any, Generic, TypeVar, overload
+
+from typing_extensions import ParamSpec
 
 
 if TYPE_CHECKING:
     from .._fixture import Fixture
 
 
 P = ParamSpec('P')
```

### Comparing `pytypest-0.1.0/pytypest/experimental/_patcher.py` & `pytypest-1.0.0/pytypest/experimental/_patcher.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/fixtures/__init__.py` & `pytypest-1.0.0/pytypest/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/fixtures/_helpers.py` & `pytypest-1.0.0/pytypest/fixtures/_helpers.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/fixtures/_misc.py` & `pytypest-1.0.0/pytypest/fixtures/_misc.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/pytypest/fixtures/_pytest.py` & `pytypest-1.0.0/pytypest/fixtures/_pytest.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/tests/conftest.py` & `pytypest-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/tests/test_autouse.py` & `pytypest-1.0.0/tests/test_autouse.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/tests/test_experimental.py` & `pytypest-1.0.0/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/tests/test_fixtrues.py` & `pytypest-1.0.0/tests/test_fixtrues.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/tests/test_fixture.py` & `pytypest-1.0.0/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/tests/test_parametrize.py` & `pytypest-1.0.0/tests/test_parametrize.py`

 * *Files identical despite different names*

### Comparing `pytypest-0.1.0/PKG-INFO` & `pytypest-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pytypest
-Version: 0.1.0
+Version: 1.0.0
 Summary: Type-safe and maintainable fixtures and parametrization for pytest.
 Keywords: pytest,tests,testing,framework,fixtures
 Author-email: Gram <git@orsinium.dev>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Typing :: Typed
 Requires-Dist: pytest
+Requires-Dist: typing-extensions
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: myst-parser ; extra == "docs"
 Requires-Dist: flake8 ; extra == "lint"
 Requires-Dist: isort ; extra == "lint"
 Requires-Dist: mypy ; extra == "lint"
 Requires-Dist: unify ; extra == "lint"
 Requires-Dist: types-requests ; extra == "lint"
@@ -26,20 +27,20 @@
 Project-URL: Source, https://github.com/orsinium-labs/pytypest
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: test
 
 # pytypest
 
-Type-safe and maintainable fixtures and parametrization for pytest.
+Type-safe and maintainable fixtures and parametrization for [pytest](https://github.com/pytest-dev/pytest).
 
 Features:
 
 + 100% type safe.
-+ Great IDE integration, go-todefinition always takes you in the right place.
++ Great IDE integration, go-to-definition always takes you in the right place.
 + Test parametrization that is redable even with many arguments.
 + Plug-and-play integration with pytest.
 + No vendor-lock, you can use only the features you need and don't touch the rest.
 + Fixtures can be cached, and you are in control of for how long.
 + Fixtures can accept arguments.
 
 ## Installation
@@ -66,7 +67,9 @@
 def test_user() -> None:
     u = get_user(anonymous=False)
     assert u.anonymous is False
 ```
 
 Compared to built-in pytest fixtures, these are explicit, type-safe, can accept arguments, support go-to-definition in IDE, and can be used as context managers. And like pytest fixtures, they are cached and can be scoped to the module or the whole session.
 
+Read more in the **documentation**: [pytypest.orsinium.dev](https://pytypest.orsinium.dev/).
+
```

