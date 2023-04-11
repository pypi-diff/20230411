# Comparing `tmp/robocorp_logging-0.0.4.tar.gz` & `tmp/robocorp_logging-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_logging-0.0.4.tar", max compression
+gzip compressed data, was "robocorp_logging-0.0.5.tar", max compression
```

## Comparing `robocorp_logging-0.0.4.tar` & `robocorp_logging-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    10142 2023-04-11 16:19:13.172254 robocorp_logging-0.0.4/LICENSE
--rw-r--r--   0        0        0     1021 2023-04-11 16:19:13.172254 robocorp_logging-0.0.4/README.md
--rw-r--r--   0        0        0      936 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     9330 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/__init__.py
--rw-r--r--   0        0        0     8075 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_ast_utils.py
--rw-r--r--   0        0        0     4611 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_auto_logging_setup.py
--rw-r--r--   0        0        0     1857 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_config.py
--rw-r--r--   0        0        0      572 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_convert_units.py
--rw-r--r--   0        0        0     5764 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_decoder.py
--rw-r--r--   0        0        0     1915 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_lifecycle_hooks.py
--rw-r--r--   0        0        0      493 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_logger_instances.py
--rw-r--r--   0        0        0    10505 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_rewrite_ast_add_callbacks.py
--rw-r--r--   0        0        0    12108 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_rewrite_filtering.py
--rw-r--r--   0        0        0    12044 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_rewrite_importhook.py
--rw-r--r--   0        0        0     8545 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_robo_logger.py
--rw-r--r--   0        0        0    48615 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/_robo_output_impl.py
--rw-r--r--   0        0        0    41740 2023-04-11 16:20:11.080737 robocorp_logging-0.0.4/src/robo_log/index.py
--rw-r--r--   0        0        0    46498 2023-04-11 16:20:14.248752 robocorp_logging-0.0.4/src/robo_log/index_v2.py
--rw-r--r--   0        0        0      414 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/protocols.py
--rw-r--r--   0        0        0        0 2023-04-11 16:19:13.176254 robocorp_logging-0.0.4/src/robo_log/py.typed
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 robocorp_logging-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-04-11 19:37:26.385516 robocorp_logging-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1021 2023-04-11 19:37:26.385516 robocorp_logging-0.0.5/README.md
+-rw-r--r--   0        0        0      936 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     9979 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/__init__.py
+-rw-r--r--   0        0        0     8075 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_ast_utils.py
+-rw-r--r--   0        0        0     4611 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_auto_logging_setup.py
+-rw-r--r--   0        0        0     1857 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_config.py
+-rw-r--r--   0        0        0      572 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_convert_units.py
+-rw-r--r--   0        0        0     5764 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_decoder.py
+-rw-r--r--   0        0        0     1915 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_lifecycle_hooks.py
+-rw-r--r--   0        0        0      493 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_logger_instances.py
+-rw-r--r--   0        0        0    10505 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_rewrite_ast_add_callbacks.py
+-rw-r--r--   0        0        0    12108 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_rewrite_filtering.py
+-rw-r--r--   0        0        0    12044 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_rewrite_importhook.py
+-rw-r--r--   0        0        0     8545 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_robo_logger.py
+-rw-r--r--   0        0        0    48615 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/_robo_output_impl.py
+-rw-r--r--   0        0        0    41740 2023-04-11 19:38:29.861820 robocorp_logging-0.0.5/src/robo_log/index.py
+-rw-r--r--   0        0        0    46498 2023-04-11 19:38:33.333835 robocorp_logging-0.0.5/src/robo_log/index_v2.py
+-rw-r--r--   0        0        0      414 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/protocols.py
+-rw-r--r--   0        0        0        0 2023-04-11 19:37:26.393516 robocorp_logging-0.0.5/src/robo_log/py.typed
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 robocorp_logging-0.0.5/PKG-INFO
```

### Comparing `robocorp_logging-0.0.4/LICENSE` & `robocorp_logging-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/README.md` & `robocorp_logging-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/pyproject.toml` & `robocorp_logging-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-logging"
-version = "0.0.4"
+version = "0.0.5"
 description = "Automatic trace logging for Python"
 authors = [
     "Fabio Z. <fabio@robocorp.com>",
     "Ossi R. <ossi@robocorp.com>",
     "Kerkko P. <kerkko@robocorp.com>",
 ]
 readme = "README.md"
```

### Comparing `robocorp_logging-0.0.4/src/robo_log/__init__.py` & `robocorp_logging-0.0.5/src/robo_log/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,37 +24,57 @@
 from ._config import Filter
 from ._logger_instances import _get_logger_instances
 from .protocols import OptExcInfo, LogHTMLStyle, Status
 
 if typing.TYPE_CHECKING:
     from ._robo_logger import _RoboLogger
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 # --- Logging methods for custom messaging.
 
 
-def critical(message: str) -> None:
+def critical(message: str, html: bool = False) -> None:
+    """
+    Adds a new logging message with a critical (error) level.
+
+    Args:
+        message: The message which should be logged.
+        html: If True the message passed should be rendered as HTML.
+    """
     for robo_logger in _get_logger_instances():
         html = False
         robo_logger.log_message(Status.ERROR, message, html)
 
 
-def info(message: str) -> None:
+def warn(message: str, html: bool = False) -> None:
+    """
+    Adds a new logging message with a warn level.
+
+    Args:
+        message: The message which should be logged.
+        html: If True the message passed should be rendered as HTML.
+    """
     for robo_logger in _get_logger_instances():
         html = False
-        robo_logger.log_message(Status.INFO, message, html)
+        robo_logger.log_message(Status.WARN, message, html)
 
 
-def warn(message: str) -> None:
+def info(message: str, html: bool = False) -> None:
+    """
+    Adds a new logging message with an info level.
+
+    Args:
+        message: The message which should be logged.
+        html: If True the message passed should be rendered as HTML.
+    """
     for robo_logger in _get_logger_instances():
-        html = False
-        robo_logger.log_message(Status.WARN, message, html)
+        robo_logger.log_message(Status.INFO, message, html)
 
 
 # --- Methods related to hiding logging information.
 
 
 @contextmanager
 def stop_logging_methods():
```

### Comparing `robocorp_logging-0.0.4/src/robo_log/_ast_utils.py` & `robocorp_logging-0.0.5/src/robo_log/_ast_utils.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_auto_logging_setup.py` & `robocorp_logging-0.0.5/src/robo_log/_auto_logging_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_config.py` & `robocorp_logging-0.0.5/src/robo_log/_config.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_convert_units.py` & `robocorp_logging-0.0.5/src/robo_log/_convert_units.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_decoder.py` & `robocorp_logging-0.0.5/src/robo_log/_decoder.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_lifecycle_hooks.py` & `robocorp_logging-0.0.5/src/robo_log/_lifecycle_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_rewrite_ast_add_callbacks.py` & `robocorp_logging-0.0.5/src/robo_log/_rewrite_ast_add_callbacks.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_rewrite_filtering.py` & `robocorp_logging-0.0.5/src/robo_log/_rewrite_filtering.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_rewrite_importhook.py` & `robocorp_logging-0.0.5/src/robo_log/_rewrite_importhook.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_robo_logger.py` & `robocorp_logging-0.0.5/src/robo_log/_robo_logger.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/_robo_output_impl.py` & `robocorp_logging-0.0.5/src/robo_log/_robo_output_impl.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/index.py` & `robocorp_logging-0.0.5/src/robo_log/index.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/src/robo_log/index_v2.py` & `robocorp_logging-0.0.5/src/robo_log/index_v2.py`

 * *Files identical despite different names*

### Comparing `robocorp_logging-0.0.4/PKG-INFO` & `robocorp_logging-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-logging
-Version: 0.0.4
+Version: 0.0.5
 Summary: Automatic trace logging for Python
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

