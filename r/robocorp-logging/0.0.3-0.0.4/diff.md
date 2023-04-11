# Comparing `tmp/robocorp-logging-0.0.3.tar.gz` & `tmp/robocorp_logging-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp-logging-0.0.3.tar", last modified: Mon Apr 10 18:48:03 2023, max compression
+gzip compressed data, was "robocorp_logging-0.0.4.tar", max compression
```

## Comparing `robocorp-logging-0.0.3.tar` & `robocorp_logging-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:48:03.715091 robocorp-logging-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-10 18:48:03.715091 robocorp-logging-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:48:03.711091 robocorp-logging-0.0.3/robocorp_logging/
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_convert_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    48648 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_rewrite_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_rewrite_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_rewrite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_rewrite_filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/_rewrite_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    41740 2023-04-10 18:48:00.000000 robocorp-logging-0.0.3/robocorp_logging/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    46498 2023-04-10 18:48:02.000000 robocorp-logging-0.0.3/robocorp_logging/index_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/robocorp_logging/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:48:03.711091 robocorp-logging-0.0.3/robocorp_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-10 18:48:03.000000 robocorp-logging-0.0.3/robocorp_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-10 18:48:03.000000 robocorp-logging-0.0.3/robocorp_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:48:03.000000 robocorp-logging-0.0.3/robocorp_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:48:03.000000 robocorp-logging-0.0.3/robocorp_logging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-10 18:48:03.000000 robocorp-logging-0.0.3/robocorp_logging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-10 18:48:03.000000 robocorp-logging-0.0.3/robocorp_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:48:03.715091 robocorp-logging-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-10 18:47:32.000000 robocorp-logging-0.0.3/setup.py
+-rw-r--r--   0        0        0    10142 2023-04-11 16:19:13.172254 robocorp_logging-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1021 2023-04-11 16:19:13.172254 robocorp_logging-0.0.4/README.md
+-rw-r--r--   0        0        0      936 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9330 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/__init__.py
+-rw-r--r--   0        0        0     8075 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_ast_utils.py
+-rw-r--r--   0        0        0     4611 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     1857 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_config.py
+-rw-r--r--   0        0        0      572 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_convert_units.py
+-rw-r--r--   0        0        0     5764 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_decoder.py
+-rw-r--r--   0        0        0     1915 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0      493 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_logger_instances.py
+-rw-r--r--   0        0        0    10505 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0    12108 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12044 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_rewrite_importhook.py
+-rw-r--r--   0        0        0     8545 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_robo_logger.py
+-rw-r--r--   0        0        0    48615 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_robo_output_impl.py
+-rw-r--r--   0        0        0    41740 2023-04-11 16:20:11.080737 robocorp_logging-0.0.4/src/robo_log/index.py
+-rw-r--r--   0        0        0    46498 2023-04-11 16:20:14.248752 robocorp_logging-0.0.4/src/robo_log/index_v2.py
+-rw-r--r--   0        0        0      414 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/protocols.py
+-rw-r--r--   0        0        0        0 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/py.typed
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 robocorp_logging-0.0.4/PKG-INFO
```

### Comparing `robocorp-logging-0.0.3/PKG-INFO` & `robocorp_logging-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 Metadata-Version: 2.1
 Name: robocorp-logging
-Version: 0.0.3
-Summary: Structured logging for Robocorp Robots.
-Home-page: https://github.com/robocorp/robocorp-logging
-Author: Fabio Zadrozny
-License: Apache-2.0
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python
+Version: 0.0.4
+Summary: Automatic trace logging for Python
+Author: Fabio Z.
+Author-email: fabio@robocorp.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Provides-Extra: test
 
 # Logging for python based Robocorp projects
 
 Logging focused on RPA projects for Robocorp robots.
 
 > Note: The current version is still pre-alpha and the [format specified](/docs/format.md) may still change.
 
@@ -50,7 +41,8 @@
 
 * See: [Handling Sensitive Data](/docs/handling_sensitive_data.md)
 
 
 ## Internal structure
 
 * [Format specification](/docs/format.md)
+
```

### Comparing `robocorp-logging-0.0.3/README.md` & `robocorp_logging-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `robocorp-logging-0.0.3/robocorp_logging/__init__.py` & `robocorp_logging-0.0.4/src/robo_log/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,150 @@
+from contextlib import contextmanager
+from io import StringIO
+from pathlib import Path
+
 import datetime
 import json
+import functools
+import sys
+import threading
+import typing
+import weakref
+
 from typing import (
     Optional,
     Any,
     Iterator,
     List,
     Sequence,
     Dict,
     Union,
     Iterable,
     Literal,
 )
-import sys
-import functools
-from io import StringIO
-import weakref
-from contextlib import contextmanager
-from pathlib import Path
-import typing
-from ._rewrite_config import Filter
-import threading
-from robocorp_logging.protocols import OptExcInfo, LogHTMLStyle
+from ._config import Filter
+from ._logger_instances import _get_logger_instances
+from .protocols import OptExcInfo, LogHTMLStyle, Status
 
 if typing.TYPE_CHECKING:
-    from ._logger import _RobocorpLogger
+    from ._robo_logger import _RoboLogger
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 version_info = [int(x) for x in __version__.split(".")]
 
 
+# --- Logging methods for custom messaging.
+
+
+def critical(message: str) -> None:
+    for robo_logger in _get_logger_instances():
+        html = False
+        robo_logger.log_message(Status.ERROR, message, html)
+
+
+def info(message: str) -> None:
+    for robo_logger in _get_logger_instances():
+        html = False
+        robo_logger.log_message(Status.INFO, message, html)
+
+
+def warn(message: str) -> None:
+    for robo_logger in _get_logger_instances():
+        html = False
+        robo_logger.log_message(Status.WARN, message, html)
+
+
+# --- Methods related to hiding logging information.
+
+
+@contextmanager
+def stop_logging_methods():
+    """
+    Can be used so that method calls are no longer logged.
+    """
+    for robo_logger in _get_logger_instances():
+        robo_logger.stop_logging_methods()
+    try:
+        yield
+    finally:
+        start_logging_methods()
+
+
+def start_logging_methods():
+    """
+    Usually doesn't need to be called as `stop_logging_methods` should be used
+    as a context manager (which would automatically call this method).
+
+    Can still be used if `stop_logging_methods` with a try..finally if
+    `stop_logging_methods` isn't used as a context manager.
+    """
+    for robo_logger in _get_logger_instances():
+        robo_logger.start_logging_methods()
+
+
+@contextmanager
+def stop_logging_variables():
+    """
+    Can be used so that variables are no longer logged.
+    """
+    for robo_logger in _get_logger_instances():
+        robo_logger.stop_logging_variables()
+
+    try:
+        yield
+    finally:
+        start_logging_variables()
+
+
+def start_logging_variables():
+    """
+    Usually doesn't need to be called as `stop_logging_variables` should be used
+    as a context manager (which would automatically call this method).
+
+    Can still be used if `stop_logging_variables` with a try..finally if
+    `stop_logging_variables` isn't used as a context manager.
+    """
+    for robo_logger in _get_logger_instances():
+        robo_logger.start_logging_variables()
+
+
+def hide_from_output(string_to_hide: str) -> None:
+    """
+    Should be called to hide sensitive information from appearing in the output.
+
+    :param string_to_hide:
+        The string that should be hidden from the output.
+    """
+    for robo_logger in _get_logger_instances():
+        robo_logger.hide_from_output(string_to_hide)
+
+
+# --- Logging methods usually called automatically from the framework.
+
+
+def start_suite(name: str, suite_id: str, suite_source: str) -> None:
+    for robo_logger in _get_logger_instances():
+        robo_logger.start_suite(name, suite_id, suite_source)
+
+
+def end_suite(name: str, suite_id: str, status: str) -> None:
+    for robo_logger in _get_logger_instances():
+        robo_logger.end_suite(name, suite_id, status)
+
+
+def start_task(name: str, task_id: str, lineno: int, tags: Sequence[str]) -> None:
+    for robo_logger in _get_logger_instances():
+        robo_logger.start_task(name, task_id, lineno, tags)
+
+
+def end_task(name: str, task_id: str, status: str, message: str) -> None:
+    for robo_logger in _get_logger_instances():
+        robo_logger.end_task(name, task_id, status, message)
+
+
 def iter_decoded_log_format(stream) -> Iterator[dict]:
     """
     :param stream:
         The stream which should be iterated in (anything with a `readlines()` method).
 
     :returns:
         An iterator which will decode the messages and provides a dictionary for
@@ -91,166 +203,14 @@
         decoded = zlib.decompress(base64.b64decode(s))
         stream.write(decoded.decode("utf-8"))
 
     stream.seek(0)
     yield from iter_decoded_log_format(stream)
 
 
-# We could use a set, but we're using a dict to keep the order.
-__tlocal_log__ = threading.local()
-
-
-def _get_logger_instances() -> Dict["_RobocorpLogger", int]:
-    instances: Dict["_RobocorpLogger", int]
-    try:
-        instances = __tlocal_log__.instances
-    except AttributeError:
-        instances = __tlocal_log__.instances = {}
-    return instances
-
-
-class _OnExitContextManager:
-    def __init__(self, on_exit):
-        self.on_exit = on_exit
-
-    def __enter__(self):
-        pass
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.on_exit()
-
-
-def _register_callbacks(rewrite_hook_config):
-    # Make sure that this method should be called only once.
-    registered = getattr(_register_callbacks, "registered", False)
-    if registered:
-        import warnings
-
-        warnings.warn("Auto logging is already setup. 2nd call has no effect.")
-        return _OnExitContextManager(lambda: None)
-    _register_callbacks.registered = True
-
-    tid = threading.get_ident()
-
-    from robocorp_logging._rewrite_hook import RewriteHook
-    from ._rewrite_callbacks import (
-        before_method,
-        after_method,
-        method_return,
-        method_except,
-    )
-
-    hook = RewriteHook(rewrite_hook_config)
-    sys.meta_path.insert(0, hook)
-
-    status_stack = []
-
-    def call_before_method(
-        package: str,
-        mod_name: str,
-        filename: str,
-        name: str,
-        lineno: int,
-        args_dict: dict,
-    ) -> None:
-        if tid != threading.get_ident():
-            return
-
-        status_stack.append([package, name, "PASS"])
-        args = []
-        for key, val in args_dict.items():
-            for p in ("password", "passwd"):
-                if p in key:
-                    for robo_logger in _get_logger_instances():
-                        robo_logger.hide_from_output(val)
-                    break
-
-            args.append((f"{key}", f"{val!r}"))
-        for robo_logger in _get_logger_instances():
-            robo_logger.start_element(
-                name,
-                f"{package}.{mod_name}",
-                filename,
-                lineno,
-                "METHOD",
-                "",
-                args,
-                [],
-                [],
-            )
-
-    def call_after_method(
-        package: str, mod_name: str, filename: str, name: str, lineno: int
-    ) -> None:
-        if tid != threading.get_ident():
-            return
-
-        try:
-            pop_package, pop_name, status = status_stack.pop(-1)
-        except IndexError:
-            # oops, something bad happened, the stack is unsynchronized
-            log_error("On method return the status_stack was empty.")
-            return
-        else:
-            if pop_package != package or pop_name != name:
-                log_error(
-                    f"On method return status stack package/name was: {pop_package}.{pop_name}. Received: {package}.{name}."
-                )
-                return
-
-        for robo_logger in _get_logger_instances():
-            robo_logger.end_method(name, f"{package}.{mod_name}", status, [])
-
-    def call_on_method_except(
-        package: str,
-        mod_name: str,
-        filename: str,
-        name: str,
-        lineno: int,
-        exc_info: OptExcInfo,
-    ) -> None:
-        if tid != threading.get_ident():
-            return
-
-        try:
-            pop_package, pop_name, _curr_status = status_stack[-1]
-        except IndexError:
-            # oops, something bad happened, the stack is unsynchronized
-            log_error("On method except the status_stack was empty.")
-            return
-
-        if pop_package != package or pop_name != name:
-            log_error(
-                f"On method except status stack package/name was: {pop_package}.{pop_name}. Received: {package}.{name}."
-            )
-            return
-        status_stack[-1][2] = Status.ERROR
-
-        for robo_logger in _get_logger_instances():
-            robo_logger.log_method_except(
-                f"{package}.{mod_name}", filename, name, lineno, exc_info, False
-            )
-
-    before_method.register(call_before_method)
-    after_method.register(call_after_method)
-    method_except.register(call_on_method_except)
-
-    def _exit():
-        # If the user actually used the with ... statement we'll remove things now.
-        # Note: this is meant only for testing as it has caveats (mainly, modules
-        # already loaded won't be rewritten and will have the hooks based on
-        # the config which was set when it was loaded).
-        sys.meta_path.remove(hook)
-        before_method.unregister(call_before_method)
-        after_method.unregister(call_after_method)
-        _register_callbacks.registered = False
-
-    return _OnExitContextManager(_exit)
-
-
 def setup_auto_logging(
     tracked_folders: Optional[Sequence[Union[Path, str]]] = None,
     untracked_folders: Optional[Sequence[Union[Path, str]]] = None,
     filters: Sequence[Filter] = (),
 ):
     """
     :param tracked_folders:
@@ -268,15 +228,16 @@
 
         [
             Filter("mymodule.ignore", exclude=True, is_path=False),
             Filter("mymodule.rpa", exclude=False, is_path=False),
             Filter("**/check/**", exclude=True, is_path=True),
         ]
     """
-    from robocorp_logging._rewrite_config import ConfigFilesFiltering
+    from ._config import ConfigFilesFiltering
+    from ._auto_logging_setup import register_auto_logging_callbacks
 
     project_roots: Optional[Sequence[str]]
     if tracked_folders:
         project_roots = [
             (f if isinstance(f, str) else str(f.absolute())) for f in tracked_folders
         ]
     else:
@@ -286,174 +247,62 @@
     if untracked_folders:
         library_roots = [
             (f if isinstance(f, str) else str(f.absolute())) for f in untracked_folders
         ]
     else:
         library_roots = None
 
-    return _register_callbacks(
+    return register_auto_logging_callbacks(
         ConfigFilesFiltering(project_roots, library_roots, filters)
     )
 
 
 def add_log_output(
     output_dir: Optional[Union[str, Path]] = None,
     max_file_size: str = "1MB",
     max_files: int = 5,
     log_html: Optional[Union[str, Path]] = None,
     log_html_style: LogHTMLStyle = "standalone",
 ):
-    from ._logger import _RobocorpLogger  # @Reimport
+    from ._robo_logger import _RoboLogger  # @Reimport
+    from robo_log._auto_logging_setup import OnExitContextManager
 
     if log_html and not output_dir:
         raise RuntimeError(
             "When log_html is specified, the output_dir must also be specified."
         )
 
-    logger = _RobocorpLogger(
+    logger = _RoboLogger(
         output_dir, max_file_size, max_files, log_html, log_html_style=log_html_style
     )
     _get_logger_instances()[logger] = 1
 
     def _exit():
         _get_logger_instances().pop(logger, None)
         logger.close()
 
-    return _OnExitContextManager(_exit)
+    return OnExitContextManager(_exit)
 
 
 def close_log_outputs():
     """
     This method must be called to close loggers (note that some loggers such as
     the one which outputs html needs to bo closed to actually write the output).
     """
     while _get_logger_instances():
         logger = next(iter(_get_logger_instances()))
         _get_logger_instances().pop(logger, None)
         logger.close()
 
 
 def add_in_memory_log_output(write):
-    from ._logger import _RobocorpLogger  # @Reimport
+    from ._robo_logger import _RoboLogger  # @Reimport
+    from robo_log._auto_logging_setup import OnExitContextManager
 
-    logger = _RobocorpLogger(__write__=write)
+    logger = _RoboLogger(__write__=write)
     _get_logger_instances()[logger] = 1
 
     def _exit():
         _get_logger_instances().pop(logger, None)
         logger.close()
 
-    return _OnExitContextManager(_exit)
-
-
-# --- Actual logging methods
-
-
-class Status:
-    PASS = "PASS"
-    ERROR = "ERROR"
-    FAIL = "FAIL"
-    INFO = "INFO"
-    WARN = "WARN"
-
-
-def log_start_suite(name: str, suite_id: str, suite_source: str) -> None:
-    for robo_logger in _get_logger_instances():
-        robo_logger.start_suite(name, suite_id, suite_source)
-
-
-def log_end_suite(name: str, suite_id: str, status: str) -> None:
-    for robo_logger in _get_logger_instances():
-        robo_logger.end_suite(name, suite_id, status)
-
-
-def log_start_task(name: str, task_id: str, lineno: int, tags: Sequence[str]) -> None:
-    for robo_logger in _get_logger_instances():
-        robo_logger.start_task(name, task_id, lineno, tags)
-
-
-def log_end_task(name: str, task_id: str, status: str, message: str) -> None:
-    for robo_logger in _get_logger_instances():
-        robo_logger.end_task(name, task_id, status, message)
-
-
-def log_error(message: str) -> None:
-    for robo_logger in _get_logger_instances():
-        html = False
-        robo_logger.log_message(Status.ERROR, message, html)
-
-
-def log_info(message: str) -> None:
-    for robo_logger in _get_logger_instances():
-        html = False
-        robo_logger.log_message(Status.INFO, message, html)
-
-
-def log_warn(message: str) -> None:
-    for robo_logger in _get_logger_instances():
-        html = False
-        robo_logger.log_message(Status.WARN, message, html)
-
-
-# --- Methods related to hiding logging information.
-
-
-@contextmanager
-def stop_logging_methods():
-    """
-    Can be used so that method calls are no longer logged.
-    """
-    for robo_logger in _get_logger_instances():
-        robo_logger.stop_logging_methods()
-    try:
-        yield
-    finally:
-        start_logging_methods()
-
-
-def start_logging_methods():
-    """
-    Usually doesn't need to be called as `stop_logging_methods` should be used
-    as a context manager (which would automatically call this method).
-
-    Can still be used if `stop_logging_methods` with a try..finally if
-    `stop_logging_methods` isn't used as a context manager.
-    """
-    for robo_logger in _get_logger_instances():
-        robo_logger.start_logging_methods()
-
-
-@contextmanager
-def stop_logging_variables():
-    """
-    Can be used so that variables are no longer logged.
-    """
-    for robo_logger in _get_logger_instances():
-        robo_logger.stop_logging_variables()
-
-    try:
-        yield
-    finally:
-        start_logging_variables()
-
-
-def start_logging_variables():
-    """
-    Usually doesn't need to be called as `stop_logging_variables` should be used
-    as a context manager (which would automatically call this method).
-
-    Can still be used if `stop_logging_variables` with a try..finally if
-    `stop_logging_variables` isn't used as a context manager.
-    """
-    for robo_logger in _get_logger_instances():
-        robo_logger.start_logging_variables()
-
-
-def hide_from_output(string_to_hide: str) -> None:
-    """
-    Should be called to hide sensitive information from appearing in the output.
-
-    :param string_to_hide:
-        The string that should be hidden from the output.
-    """
-    for robo_logger in _get_logger_instances():
-        robo_logger.hide_from_output(string_to_hide)
+    return OnExitContextManager(_exit)
```

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_ast_utils.py` & `robocorp_logging-0.0.4/src/robo_log/_ast_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_convert_units.py` & `robocorp_logging-0.0.4/src/robo_log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_decoder.py` & `robocorp_logging-0.0.4/src/robo_log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_impl.py` & `robocorp_logging-0.0.4/src/robo_log/_robo_output_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import datetime
 from typing import Optional, Callable
 import os
 import traceback
 from contextlib import contextmanager
 import sys
 import weakref
-from robocorp_logging.protocols import OptExcInfo
+from robo_log.protocols import OptExcInfo
 from functools import partial
 
 
 _valid_chars = tuple(string.ascii_letters + string.digits)
 
 
 def _gen_id(level: int = 1) -> Iterator[str]:
@@ -193,15 +193,15 @@
 
     def __iter__(self):
         for stack_entry in self._queue:
             assert isinstance(stack_entry, _StackEntry)
             yield stack_entry
 
 
-class _RobotOutputImpl:
+class _RoboOutputImpl:
     def __init__(self, config: _Config):
         self._written_initial = False
         self._closed = False
 
         # Base memory for all streams (rotated or not)
         self._base_memo: Dict[str, str] = {}
 
@@ -696,23 +696,23 @@
             target = os.path.abspath(log_html)
             dirname = os.path.dirname(target)
             if not os.path.exists(dirname):
                 os.makedirs(dirname, exist_ok=True)
             print(f"Robocorp Log (html): {target}")
 
             if self._config.log_html_style == 1:
-                from robocorp_logging import index
+                from robo_log import index
             elif self._config.log_html_style == 2:
-                from robocorp_logging import index_v2 as index
+                from robo_log import index_v2 as index
             else:
                 raise ValueError(
                     "Unexpected log html style: {self._config.log_html_style}"
                 )
 
-            # from robocorp_logging import index
+            # from robo_log import index
 
             has_separate_bundle_js = "bundle.js" in index.FILE_CONTENTS
 
             for name, contents in index.FILE_CONTENTS.items():
                 if name == "index.html":
                     if has_separate_bundle_js:
                         self._write_simple(target, contents)
```

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_logger.py` & `robocorp_logging-0.0.4/src/robo_log/_robo_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import StringIO
 import functools
 from pathlib import Path
 from typing import Optional, Union, Sequence, Tuple
 import datetime
-from robocorp_logging.protocols import OptExcInfo, LogHTMLStyle
+from robo_log.protocols import OptExcInfo, LogHTMLStyle
 
 
 def _log_error(func):
     @functools.wraps(func)
     def new_func(self, *args, **kwargs):
         import traceback
 
@@ -15,34 +15,34 @@
             return func(self, *args, **kwargs)
         except Exception as e:
             s = StringIO()
             traceback.print_exc(file=s)
             traceback.print_exc()
             self._robot_output_impl.log_message(
                 "ERROR",
-                f"_RobocorpLogger internal error: {e}\n{s.getvalue()}",
+                f"_RoboLogger internal error: {e}\n{s.getvalue()}",
                 self._robot_output_impl.get_time_delta(),
                 False,
             )
 
     return new_func
 
 
-class _RobocorpLogger:
+class _RoboLogger:
     def __init__(
         self,
         output_dir: Optional[Union[str, Path]] = None,
         max_file_size: str = "1MB",
         max_files: int = 5,
         log_html: Optional[Union[Path, str]] = None,
         log_html_style: LogHTMLStyle = "standalone",
         **kwargs,
     ):
-        from robocorp_logging._impl import _RobotOutputImpl, _Config
-        from robocorp_logging._convert_units import _convert_to_bytes
+        from robo_log._robo_output_impl import _RoboOutputImpl, _Config
+        from robo_log._convert_units import _convert_to_bytes
 
         # Note: expected to be used just when used in-memory (not part of the public API).
         config = _Config(kwargs.get("__uuid__"))
         if log_html_style == "standalone":
             config.log_html_style = 2
         elif log_html_style == "vscode":
             config.log_html_style = 1
@@ -70,15 +70,15 @@
             )
 
         # Note: expected to be used just when used in-memory (not part of the public API).
         config.write = kwargs.get("__write__")
         config.initial_time = kwargs.get("__initial_time__")
         config.additional_info = kwargs.get("__additional_info__")
 
-        self._robot_output_impl = _RobotOutputImpl(config)
+        self._robot_output_impl = _RoboOutputImpl(config)
         self._skip_log_methods = 0
         self._skip_log_arguments = 0
 
     def hide_from_output(self, string_to_hide: str) -> None:
         self._robot_output_impl.hide_from_output(string_to_hide)
 
     @property
@@ -92,30 +92,30 @@
     def _get_time_delta(self) -> float:
         return self._robot_output_impl.get_time_delta()
 
     def start_logging_methods(self):
         if self._skip_log_methods <= 0:
             self._robot_output_impl.log_message(
                 "ERROR",
-                f"_RobocorpLogger error: start_logging_methods() called before stop_logging_methods() (call is ignored as logging is already on).",
+                f"_RoboLogger error: start_logging_methods() called before stop_logging_methods() (call is ignored as logging is already on).",
                 self._robot_output_impl.get_time_delta(),
                 False,
             )
             return
 
         self._skip_log_methods -= 1
 
     def stop_logging_methods(self):
         self._skip_log_methods += 1
 
     def start_logging_variables(self):
         if self._skip_log_arguments <= 0:
             self._robot_output_impl.log_message(
                 "ERROR",
-                f"_RobocorpLogger error: start_logging_variables() called before stop_logging_variables() (call is ignored as logging is already on).",
+                f"_RoboLogger error: start_logging_variables() called before stop_logging_variables() (call is ignored as logging is already on).",
                 self._robot_output_impl.get_time_delta(),
                 False,
             )
             return
 
         self._skip_log_arguments -= 1
```

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_rewrite_ast.py` & `robocorp_logging-0.0.4/src/robo_log/_rewrite_ast_add_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 from typing import Optional, Any, Union, List
 import sys
 from . import _ast_utils
-from ._rewrite_config import BaseConfig
+from ._config import BaseConfig
 
 DEBUG = False
 
 
 def is_rewrite_disabled(docstring: str) -> bool:
     return "NO_LOG" in docstring
 
@@ -57,26 +57,24 @@
     else:
         lineno = item.lineno
     # Now actually insert the special imports.
     if sys.version_info >= (3, 10):
         aliases = [
             ast.alias("builtins", "@py_builtins", lineno=lineno, col_offset=0),
             ast.alias(
-                "robocorp_logging._rewrite_callbacks",
+                "robo_log._lifecycle_hooks",
                 "@robocorp_rewrite_callbacks",
                 lineno=lineno,
                 col_offset=0,
             ),
         ]
     else:
         aliases = [
             ast.alias("builtins", "@py_builtins"),
-            ast.alias(
-                "robocorp_logging._rewrite_callbacks", "@robocorp_rewrite_callbacks"
-            ),
+            ast.alias("robo_log._lifecycle_hooks", "@robocorp_rewrite_callbacks"),
         ]
 
     imports = [ast.Import([alias], lineno=lineno, col_offset=0) for alias in aliases]
     mod.body[pos:pos] = imports
 
     it: Any = _ast_utils.iter_and_replace_nodes(mod)
     node: Any
```

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_rewrite_callbacks.py` & `robocorp_logging-0.0.4/src/robo_log/_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_rewrite_config.py` & `robocorp_logging-0.0.4/src/robo_log/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,20 +29,20 @@
 
     def __init__(
         self,
         project_roots: Optional[Sequence[str]] = None,
         library_roots: Optional[Sequence[str]] = None,
         filters: Sequence[Filter] = (),
     ):
-        from robocorp_logging._rewrite_filtering import FilesFiltering
+        from robo_log._rewrite_filtering import FilesFiltering
 
         self._files_filtering = FilesFiltering(project_roots, library_roots, filters)
 
     def can_rewrite_module_name(self, module_name: str) -> bool:
-        if module_name.startswith("robocorp_logging"):
+        if module_name.startswith("robo_log"):
             # We can't rewrite our own modules (we could end up recursing).
             if "check" in module_name:
                 # Exception just for testing.
                 return True
             return False
 
         return self._files_filtering.accept_module_name(module_name)
```

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_rewrite_filtering.py` & `robocorp_logging-0.0.4/src/robo_log/_rewrite_filtering.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os.path
 import sys
 
 import platform
 import logging
 from typing import Sequence, Optional, List, Dict, Any
 import threading
-from ._rewrite_config import Filter
+from ._config import Filter
 
 log = logging.getLogger(__name__)
 
 
 def normcase(s, NORMCASE_CACHE={}):
     try:
         return NORMCASE_CACHE[s]
```

### Comparing `robocorp-logging-0.0.3/robocorp_logging/_rewrite_hook.py` & `robocorp_logging-0.0.4/src/robo_log/_rewrite_importhook.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,25 +35,26 @@
 from typing import Callable
 from typing import Dict
 from typing import IO
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import Union
-from ._rewrite_config import BaseConfig
-from ._rewrite_ast import rewrite_ast_add_callbacks
+from ._config import BaseConfig
+from ._rewrite_ast_add_callbacks import rewrite_ast_add_callbacks
 
 
 # caches rewritten pycs in pycache dirs
 # 0.0.1: Initial version
 # 0.0.2: Bugfix: docstrings must be kept as the first statement
 # 0.0.3: Support for exception handlers
 # 0.0.4: Add __name__
-version = "0.0.4"
-PYTEST_TAG = f"{sys.implementation.cache_tag}-robocorp-{version}"
+# 0.0.5: Renames of internal modules.
+version = "0.0.5"
+PYTEST_TAG = f"{sys.implementation.cache_tag}-robo_log-{version}"
 PYC_EXT = ".py" + (__debug__ and "c" or "o")
 PYC_TAIL = "." + PYTEST_TAG + PYC_EXT
 
 FORCE_CODE_GENERATION = False
 DEBUG = False
```

### Comparing `robocorp-logging-0.0.3/robocorp_logging/index.py` & `robocorp_logging-0.0.4/src/robo_log/index.py`

 * *Files identical despite different names*

### Comparing `robocorp-logging-0.0.3/robocorp_logging/index_v2.py` & `robocorp_logging-0.0.4/src/robo_log/index_v2.py`

 * *Files identical despite different names*

