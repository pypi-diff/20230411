# Comparing `tmp/playwrightcapture-1.19.4.tar.gz` & `tmp/playwrightcapture-1.19.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.19.4.tar", max compression
+gzip compressed data, was "playwrightcapture-1.19.5.tar", max compression
```

## Comparing `playwrightcapture-1.19.4.tar` & `playwrightcapture-1.19.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.4/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.4/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.4/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    24984 2023-04-11 13:25:21.919269 playwrightcapture-1.19.4/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.4/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.4/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.4/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1739 2023-04-11 13:25:53.704089 playwrightcapture-1.19.4/pyproject.toml
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.4/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.5/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.5/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.5/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    25250 2023-04-11 15:25:18.395074 playwrightcapture-1.19.5/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.5/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.5/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.5/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1739 2023-04-11 15:27:35.593140 playwrightcapture-1.19.5/pyproject.toml
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.5/PKG-INFO
```

### Comparing `playwrightcapture-1.19.4/LICENSE` & `playwrightcapture-1.19.5/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.4/README.md` & `playwrightcapture-1.19.5/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.4/playwrightcapture/capture.py` & `playwrightcapture-1.19.5/playwrightcapture/capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 import asyncio
 import json
+import logging
 import os
 import random
-import logging
+import time
 
 from tempfile import NamedTemporaryFile
 from typing import Optional, Dict, List, Union, Any, TypedDict, Literal
 
 import dateparser
 
 from playwright.async_api import async_playwright, ProxySettings, Frame, ViewportSize, Cookie, Error, Page
@@ -493,29 +494,32 @@
 
                 to_return['png'] = await self._failsafe_get_screenshot(page)
 
                 if depth > 0 and to_return.get('html') and to_return['html']:
                     to_return['children'] = []
                     depth -= 1
                     child_urls = get_links_from_rendered_page(page.url, to_return['html'], rendered_hostname_only)
-                    self.logger.info(f'Capturing children, {len(child_urls)} URLs')
-                    for url in child_urls:
-                        self.logger.info(f'Capture child {url}')
+                    total_urls = len(child_urls)
+                    self.logger.info(f'Capturing children, {total_urls} URLs')
+                    for index, url in enumerate(child_urls):
+                        self.logger.info(f'Capture child {url} - Timeout: {max_depth_capture_time}s')
+                        start_time = time.time()
                         try:
                             child_capture = await asyncio.wait_for(
                                 self.capture_page(url=url, referer=page.url,
                                                   page=page, depth=depth,
                                                   rendered_hostname_only=rendered_hostname_only,
-                                                  max_depth_capture_time=max_depth_capture_time / len(child_urls)),
+                                                  max_depth_capture_time=max_depth_capture_time / total_urls),
                                 timeout=max_depth_capture_time)
                             to_return['children'].append(child_capture)  # type: ignore
                         except (TimeoutError, asyncio.exceptions.TimeoutError):
                             self.logger.warning(f'Timeout error, took more than {max_depth_capture_time}s. Unable to capture {url}.')
                         else:
-                            self.logger.info(f'Successfully captured child UR: {url}')
+                            runtime = time.time() - start_time
+                            self.logger.info(f'Successfully captured child URL: {url} in {runtime}s. {total_urls - index - 1} to go.')
                         try:
                             await page.go_back()
                         except PlaywrightTimeoutError as e:
                             self.logger.warning(f'Go back timed out, it is probably not a big deal: {e}')
 
         except PlaywrightTimeoutError as e:
             to_return['error'] = f"The capture took too long - {e.message}"
```

### Comparing `playwrightcapture-1.19.4/playwrightcapture/helpers.py` & `playwrightcapture-1.19.5/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.4/pyproject.toml` & `playwrightcapture-1.19.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.19.4"
+version = "1.19.5"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.19.4/PKG-INFO` & `playwrightcapture-1.19.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.19.4
+Version: 1.19.5
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

