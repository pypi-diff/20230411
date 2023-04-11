# Comparing `tmp/setuptools-monorepo-0.0.3.tar.gz` & `tmp/setuptools-monorepo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-monorepo-0.0.3.tar", last modified: Thu Sep 22 12:30:15 2022, max compression
+gzip compressed data, was "setuptools-monorepo-0.0.4.tar", last modified: Tue Apr 11 07:50:12 2023, max compression
```

## Comparing `setuptools-monorepo-0.0.3.tar` & `setuptools-monorepo-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2022-09-22 12:30:15.442950 setuptools-monorepo-0.0.3/
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)     1093 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.3/LICENSE
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)       43 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.3/MANIFEST.in
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      251 2022-09-22 12:30:15.442950 setuptools-monorepo-0.0.3/PKG-INFO
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)     1850 2022-06-24 08:45:24.000000 setuptools-monorepo-0.0.3/README.md
-drwxr-xr-x   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2022-09-22 12:30:15.441950 setuptools-monorepo-0.0.3/monorepo_loader/
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.3/monorepo_loader/__init__.py
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)     5971 2022-09-22 12:14:01.000000 setuptools-monorepo-0.0.3/monorepo_loader/setuptools_monorepo.py
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      190 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.3/pyproject.toml
-drwxr-xr-x   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2022-09-22 12:30:15.441950 setuptools-monorepo-0.0.3/requirements/
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      738 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.3/requirements/test.requirements.txt
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      442 2022-09-22 12:30:15.442950 setuptools-monorepo-0.0.3/setup.cfg
-drwxr-xr-x   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2022-09-22 12:30:15.442950 setuptools-monorepo-0.0.3/setuptools_monorepo.egg-info/
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      251 2022-09-22 12:30:15.000000 setuptools-monorepo-0.0.3/setuptools_monorepo.egg-info/PKG-INFO
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      374 2022-09-22 12:30:15.000000 setuptools-monorepo-0.0.3/setuptools_monorepo.egg-info/SOURCES.txt
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)        1 2022-09-22 12:30:15.000000 setuptools-monorepo-0.0.3/setuptools_monorepo.egg-info/dependency_links.txt
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      103 2022-09-22 12:30:15.000000 setuptools-monorepo-0.0.3/setuptools_monorepo.egg-info/entry_points.txt
--rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)       16 2022-09-22 12:30:15.000000 setuptools-monorepo-0.0.3/setuptools_monorepo.egg-info/top_level.txt
+drwxr-xr-x   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2023-04-11 07:50:12.315755 setuptools-monorepo-0.0.4/
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)     1093 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.4/LICENSE
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)       43 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.4/MANIFEST.in
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      251 2023-04-11 07:50:12.315755 setuptools-monorepo-0.0.4/PKG-INFO
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)     2061 2023-04-11 07:44:53.000000 setuptools-monorepo-0.0.4/README.md
+drwxr-xr-x   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2023-04-11 07:50:12.314755 setuptools-monorepo-0.0.4/monorepo_loader/
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.4/monorepo_loader/__init__.py
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)     7095 2023-04-11 07:44:53.000000 setuptools-monorepo-0.0.4/monorepo_loader/setuptools_monorepo.py
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      244 2023-04-11 07:44:53.000000 setuptools-monorepo-0.0.4/pyproject.toml
+drwxr-xr-x   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2023-04-11 07:50:12.314755 setuptools-monorepo-0.0.4/requirements/
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      738 2022-06-22 15:34:59.000000 setuptools-monorepo-0.0.4/requirements/test.requirements.txt
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      628 2023-04-11 07:50:12.315755 setuptools-monorepo-0.0.4/setup.cfg
+drwxr-xr-x   0 vladislavivanov  (1004) vladislavivanov  (1005)        0 2023-04-11 07:50:12.315755 setuptools-monorepo-0.0.4/setuptools_monorepo.egg-info/
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      251 2023-04-11 07:50:12.000000 setuptools-monorepo-0.0.4/setuptools_monorepo.egg-info/PKG-INFO
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      416 2023-04-11 07:50:12.000000 setuptools-monorepo-0.0.4/setuptools_monorepo.egg-info/SOURCES.txt
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)        1 2023-04-11 07:50:12.000000 setuptools-monorepo-0.0.4/setuptools_monorepo.egg-info/dependency_links.txt
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)      227 2023-04-11 07:50:12.000000 setuptools-monorepo-0.0.4/setuptools_monorepo.egg-info/entry_points.txt
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)       41 2023-04-11 07:50:12.000000 setuptools-monorepo-0.0.4/setuptools_monorepo.egg-info/requires.txt
+-rw-r--r--   0 vladislavivanov  (1004) vladislavivanov  (1005)       16 2023-04-11 07:50:12.000000 setuptools-monorepo-0.0.4/setuptools_monorepo.egg-info/top_level.txt
```

### Comparing `setuptools-monorepo-0.0.3/LICENSE` & `setuptools-monorepo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-monorepo-0.0.3/README.md` & `setuptools-monorepo-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-## setuptools-monorepo
+# setuptools-monorepo
 
 `setuptools-monorepo` is a plugin for `setuptools` that lets you discover and
 run Python scripts when your packages are installed from `git://` URL. This means
 that in a monorepo, multiple packages residing in different subfolders and referred
 to using `#subdirectory=` attribute can share common setup code.
 
-#### Use cases
+## Use cases
 
 * resolving dependencies within a monorepo
 * automatic generation of package metadata such as version
 * installation environment checks (compilers, libraries, native tools etc)
 
-### Usage
+## Usage
 
-#### Declaring monorepo scripts
+### Declaring monorepo scripts
 
 Any directory, except for the root of the repo, will be considered a script
 if it contains two files:
 
 ```
 script_name
 ├── entrypoint.py
 └── monorepo_script.toml
 ```
 
 `script_name` will be used to refer to the script. `monorepo_script.toml` is empty
-for now but is reserved for adding configuration options in future.
+for now but is reserved for adding configuration options in the future.
 
 `entrypoint.py` should contain a function declared as follows:
 
 ```python
 import setuptools
 
 def entrypoint(dist: setuptools.dist.Distribution, arg1: int, arg_n: str):
@@ -39,24 +39,38 @@
 The first argument of the function is a `Distribution` object that can be modified
 by the script. The rest of the args are arbitrary and will be matched by name during
 invocation.
 
 When scripts are loaded, parent directory of each script is added to `PYTHONPATH`. This
 makes it possible to load code shared between scripts.
 
-#### Calling monorepo scripts
+### Calling monorepo scripts
 
-Scripts can be invoked during installation using `monorepo_call` keyword in `setup.py`:
+#### With `pyproject.toml`
+
+Scripts can be invoked during installation using the following syntax in `pyproject.toml`:
+
+```toml
+[tool.setuptools_monorepo.test_script]
+arg_1 = [
+    "one_of_values_of_arg_1"
+]
+arg_2 = "some_value"
+```
+
+#### With `setup.py`
+
+For `setup.py`, use `monorepo_call` keyword:
 
 ```python
 from setuptools import setup
 
 if __name__ == '__main__':
     setup(
-        setup_requires=['setuptools-monorepo == 0.0.2'],
+        setup_requires=['setuptools-monorepo == 0.0.4'],
         monorepo_call={
             'target': 'test_script',
             'args': {
                 'arg1': 1,
                 'arg2': 'some_string',
             },
         },
```

### Comparing `setuptools-monorepo-0.0.3/monorepo_loader/setuptools_monorepo.py` & `setuptools-monorepo-0.0.4/monorepo_loader/setuptools_monorepo.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from dataclasses import dataclass
 from inspect import FullArgSpec
 from types import ModuleType
 from typing import Any, Dict, Iterable, List, Optional, Sequence
 
 import setuptools
 
+if sys.version_info < (3, 11):
+    import tomli as toml
+else:
+    import tomllib as toml
+
+
 SCRIPT_MARKER = "monorepo_script.toml"
 SCRIPT_ENTRYPOINT = "entrypoint.py"
 
 
 @dataclass
 class Script:
     name: str
@@ -132,18 +138,15 @@
         if spec.loader is None:
             raise RuntimeError("No spec loader available")
 
         spec.loader.exec_module(module)
         return module
 
 
-def _call_script(dist: setuptools.dist.Distribution, value: Dict[str, Any]):
-    target = value["target"]
-    args = value["args"] if "args" in value else {}
-
+def _call_script(dist: setuptools.dist.Distribution, target: str, args: Dict[str, Any]):
     _eprint(f"Looking for monorepo script {target}")
 
     repo_root = _get_repo_root()
     scripts = _discover_scripts(repo_root)
     target_script = next((s for s in scripts if s.name == target), None)
 
     if target_script is None:
@@ -175,20 +178,58 @@
         if maybe_error is not None:
             _eprint(maybe_error)
             raise RuntimeError()
 
     imported_script.entrypoint(dist, **args)
 
 
-def handle_monorepo_package(dist: setuptools.dist.Distribution, attr: str, value: Any):
+def handle_monorepo_keywords(dist: setuptools.dist.Distribution, attr: str, value: Any):
     validation_result = _validate_value(value)
 
     if validation_result is not None:
         _eprint(f"invalid argument passed: {validation_result}")
         raise RuntimeError()
 
-    if isinstance(value, Sequence):
-        for entry in value:
-            _call_script(dist, entry)
+    def _get_call_args(call: Dict[str, Any]):
+        call_target = call["target"]
+        call_args = call["args"] if "args" in call else {}
+        return call_target, call_args
+
+    def _make_sequence():
+        if isinstance(value, Sequence):
+            return value
+        else:
+            return [value]
+
+    values = _make_sequence()
+
+    for entry in values:
+        if not isinstance(entry, Dict):
+            _eprint(f"received invalid argument for setuptools-monorepo: not a dict")
+            raise RuntimeError()
+
+        target, args = _get_call_args(entry)
+        _call_script(dist, target, args)
+
+
+def handle_monorepo_dist(dist: setuptools.dist.Distribution):
+    pyproject_toml = os.path.join(os.getcwd(), "pyproject.toml")
+    if not os.path.exists(pyproject_toml):
+        return
+
+    def _parse_file():
+        with open(pyproject_toml, "rb") as f:
+            return toml.load(f)
+
+    project = _parse_file()
+    if "tool" not in project:
+        return
+
+    if "setuptools_monorepo" not in project["tool"]:
+        return
+
+    invocations = project["tool"]["setuptools_monorepo"]
+    if not isinstance(invocations, Dict):
         return
 
-    _call_script(dist, value)
+    for target, args in invocations.items():
+        _call_script(dist, target, args)
```

### Comparing `setuptools-monorepo-0.0.3/requirements/test.requirements.txt` & `setuptools-monorepo-0.0.4/requirements/test.requirements.txt`

 * *Files identical despite different names*

