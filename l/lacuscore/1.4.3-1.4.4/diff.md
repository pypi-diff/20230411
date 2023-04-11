# Comparing `tmp/lacuscore-1.4.3.tar.gz` & `tmp/lacuscore-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lacuscore-1.4.3.tar", max compression
+gzip compressed data, was "lacuscore-1.4.4.tar", max compression
```

## Comparing `lacuscore-1.4.3.tar` & `lacuscore-1.4.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.3/LICENSE
--rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.3/README.md
--rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.3/lacuscore/__init__.py
--rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.3/lacuscore/lacus_monitoring.py
--rw-r--r--   0        0        0    27996 2023-04-10 16:22:59.484951 lacuscore-1.4.3/lacuscore/lacuscore.py
--rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.3/lacuscore/py.typed
--rw-r--r--   0        0        0     1470 2023-04-10 16:42:10.202694 lacuscore-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 lacuscore-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1516 2022-09-13 21:10:56.118975 lacuscore-1.4.4/LICENSE
+-rw-r--r--   0        0        0      941 2022-10-17 09:41:56.955953 lacuscore-1.4.4/README.md
+-rw-r--r--   0        0        0      169 2022-10-12 16:05:45.482302 lacuscore-1.4.4/lacuscore/__init__.py
+-rw-r--r--   0        0        0     1105 2022-10-13 11:42:38.221153 lacuscore-1.4.4/lacuscore/lacus_monitoring.py
+-rw-r--r--   0        0        0    28070 2023-04-11 13:29:09.084489 lacuscore-1.4.4/lacuscore/lacuscore.py
+-rw-r--r--   0        0        0        0 2022-09-13 21:10:56.122975 lacuscore-1.4.4/lacuscore/py.typed
+-rw-r--r--   0        0        0     1516 2023-04-11 13:38:50.450245 lacuscore-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 lacuscore-1.4.4/PKG-INFO
```

### Comparing `lacuscore-1.4.3/LICENSE` & `lacuscore-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.3/README.md` & `lacuscore-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.3/lacuscore/lacus_monitoring.py` & `lacuscore-1.4.4/lacuscore/lacus_monitoring.py`

 * *Files identical despite different names*

### Comparing `lacuscore-1.4.3/lacuscore/lacuscore.py` & `lacuscore-1.4.4/lacuscore/lacuscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,15 +522,16 @@
                     capture.viewport = to_capture.get('viewport')  # type: ignore
                     capture.user_agent = to_capture.get('user_agent')  # type: ignore
                     await capture.initialize_context()
                     playwright_result = await asyncio.wait_for(
                         capture.capture_page(
                             url, referer=to_capture.get('referer'),
                             depth=to_capture.get('depth', 0),
-                            rendered_hostname_only=to_capture.get('rendered_hostname_only', True)),
+                            rendered_hostname_only=to_capture.get('rendered_hostname_only', True),
+                            max_depth_capture_time=self.max_capture_time),
                         timeout=self.max_capture_time)
             except PlaywrightCaptureException as e:
                 logger.exception(f'Invalid parameters for the capture of {url} - {e}')
                 result = {'error': 'Invalid parameters for the capture of {url} - {e}'}
                 raise CaptureError
             except asyncio.CancelledError:
                 logger.warning(f'The capture of {url} has been cancelled.')
```

### Comparing `lacuscore-1.4.3/pyproject.toml` & `lacuscore-1.4.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lacuscore"
-version = "1.4.3"
+version = "1.4.4"
 description = "Core of Lacus, usable as a module"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/LacusCore"
 documentation = "https://lacuscore.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -17,25 +17,26 @@
     'Intended Audience :: Science/Research',
     'Intended Audience :: Telecommunications Industry',
     'Intended Audience :: Information Technology',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Security',
     'Topic :: Internet',
 ]
 
 include = ['README.md']
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.2"
 Sphinx = { version = "^6.1.3", optional = true }
-playwrightcapture = {extras = ["recaptcha"], version = "^1.19.3"}
+playwrightcapture = {extras = ["recaptcha"], version = "^1.19.4"}
 defang = "^0.5.3"
 ua-parser = "^0.16.1"
 redis = {version = "^4.5.4", extras = ["hiredis"]}
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
```

### Comparing `lacuscore-1.4.3/PKG-INFO` & `lacuscore-1.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lacuscore
-Version: 1.4.3
+Version: 1.4.4
 Summary: Core of Lacus, usable as a module
 Home-page: https://github.com/ail-project/LacusCore
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,22 +17,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
 Requires-Dist: defang (>=0.5.3,<0.6.0)
-Requires-Dist: playwrightcapture[recaptcha] (>=1.19.3,<2.0.0)
+Requires-Dist: playwrightcapture[recaptcha] (>=1.19.4,<2.0.0)
 Requires-Dist: redis[hiredis] (>=4.5.4,<5.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ua-parser (>=0.16.1,<0.17.0)
 Project-URL: Documentation, https://lacuscore.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ail-project/LacusCore
 Description-Content-Type: text/markdown
```

