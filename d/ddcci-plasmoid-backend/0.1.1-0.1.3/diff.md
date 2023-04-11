# Comparing `tmp/ddcci_plasmoid_backend-0.1.1.tar.gz` & `tmp/ddcci_plasmoid_backend-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddcci_plasmoid_backend-0.1.1.tar", max compression
+gzip compressed data, was "ddcci_plasmoid_backend-0.1.3.tar", max compression
```

## Comparing `ddcci_plasmoid_backend-0.1.1.tar` & `ddcci_plasmoid_backend-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1276 2023-04-09 11:20:03.343482 ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/__init__.py
--rw-r--r--   0        0        0     2718 2023-04-09 16:12:30.293937 ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/__main__.py
--rw-r--r--   0        0        0     3053 2023-04-09 11:37:36.411064 ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/ddcci.py
--rw-r--r--   0        0        0     2426 2023-04-08 18:58:49.286640 ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/ddcutil_parser.py
--rw-r--r--   0        0        0      400 2023-04-09 16:10:53.377359 ddcci_plasmoid_backend-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3126 2023-04-11 20:59:26.584966 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/Node.py
+-rw-r--r--   0        0        0     3393 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/Node_test.py
+-rw-r--r--   0        0        0      889 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/__init__.py
+-rw-r--r--   0        0        0     3253 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/__main__.py
+-rw-r--r--   0        0        0     5512 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/ddcci.py
+-rw-r--r--   0        0        0     1941 2023-04-11 20:59:26.588299 ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/ddcci_test.py
+-rw-r--r--   0        0        0      631 2023-04-11 20:59:42.701439 ddcci_plasmoid_backend-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      468 1970-01-01 00:00:00.000000 ddcci_plasmoid_backend-0.1.3/PKG-INFO
```

### Comparing `ddcci_plasmoid_backend-0.1.1/ddcci_plasmoid_backend/__main__.py` & `ddcci_plasmoid_backend-0.1.3/ddcci_plasmoid_backend/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 import asyncio
 import json
 import logging
+import os
 import subprocess
 import sys
 import tempfile
 from importlib.metadata import version
 from pathlib import Path
-import os
 from typing import NoReturn
 
 import fasteners
 
-from ddcci_plasmoid_backend import arguments
 from ddcci_plasmoid_backend import ddcci
+from ddcci_plasmoid_backend.__init__ import get_parser
+
+arguments = vars(get_parser().parse_args())
 
+logging.basicConfig(format='%(levelname)s %(name)s: %(message)s',
+                    level=logging.DEBUG if arguments['debug'] else logging.INFO)
+# supress log message `DEBUG asyncio: Using selector: EpollSelector`
+logging.getLogger('asyncio').setLevel(logging.WARNING)
 logger = logging.getLogger(__name__)
+logger.debug('Run in debug mode')
 
 
 def handle_error(error: str | subprocess.CalledProcessError) -> NoReturn:
     if isinstance(error, subprocess.CalledProcessError):
         error = err.stderr.decode() if err.stderr else err.stdout.decode()
     print(json.dumps({
         'command': arguments['command'],
@@ -39,26 +46,31 @@
     with fasteners.InterProcessLock(Path(tempfile.gettempdir()) / f'ddcci_plasmoid_backend-{os.getlogin()}.lock'):
         if arguments['command'] == 'detect':
             try:
                 result = asyncio.run(ddcci.detect())
             except subprocess.CalledProcessError as err:
                 handle_error(err)
 
+            count = len(result)
             # Remove objects that are errors
-            filtered_results = [report for report in result if isinstance(report, dict)]
+            for report in result:
+                if isinstance(report, Exception):
+                    logger.debug(report)
+                    result.remove(report)
+            # filtered_results = [report for report in result if isinstance(report, dict)]
 
-            filtered_count = len(filtered_results)
-            remaining_count = len(result) - filtered_count
+            filtered_count = len(result)
+            remaining_count = count - filtered_count
 
             logger.debug(f'Detected {filtered_count} working monitor {"bus" if filtered_count == 1 else "busses"}, '
                          f'{remaining_count} non-working {"bus" if remaining_count == 1 else "busses"}.')
 
             print(json.dumps({
                 'command': 'detect',
-                'value': filtered_results
+                'value': result
             }))
         elif arguments['command'] == 'set-brightness':
             bus_id = arguments['bus']
             brightness = arguments['brightness']
             if brightness < 0 or brightness > 100:
                 handle_error(f'Illegal value {brightness} for `brightness`, must be between 0 and 100')
```

