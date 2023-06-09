# Comparing `tmp/playwrightcapture-1.19.7.tar.gz` & `tmp/playwrightcapture-1.19.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playwrightcapture-1.19.7.tar", max compression
+gzip compressed data, was "playwrightcapture-1.19.8.tar", max compression
```

## Comparing `playwrightcapture-1.19.7.tar` & `playwrightcapture-1.19.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.7/LICENSE
--rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.7/README.md
--rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.7/playwrightcapture/__init__.py
--rw-r--r--   0        0        0    25570 2023-04-11 16:14:05.187692 playwrightcapture-1.19.7/playwrightcapture/capture.py
--rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.7/playwrightcapture/exceptions.py
--rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.7/playwrightcapture/helpers.py
--rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.7/playwrightcapture/py.typed
--rw-r--r--   0        0        0     1739 2023-04-11 16:15:38.885216 playwrightcapture-1.19.7/pyproject.toml
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.7/PKG-INFO
+-rw-r--r--   0        0        0     1775 2022-04-25 10:38:53.875053 playwrightcapture-1.19.8/LICENSE
+-rw-r--r--   0        0        0     1411 2022-05-19 22:11:30.974772 playwrightcapture-1.19.8/README.md
+-rw-r--r--   0        0        0      297 2022-09-29 12:50:02.947281 playwrightcapture-1.19.8/playwrightcapture/__init__.py
+-rw-r--r--   0        0        0    25697 2023-04-11 16:53:16.977815 playwrightcapture-1.19.8/playwrightcapture/capture.py
+-rw-r--r--   0        0        0      366 2022-09-29 12:49:52.363206 playwrightcapture-1.19.8/playwrightcapture/exceptions.py
+-rw-r--r--   0        0        0     2942 2022-12-29 11:15:05.546949 playwrightcapture-1.19.8/playwrightcapture/helpers.py
+-rw-r--r--   0        0        0        0 2022-04-19 13:10:37.241346 playwrightcapture-1.19.8/playwrightcapture/py.typed
+-rw-r--r--   0        0        0     1739 2023-04-11 16:54:23.726491 playwrightcapture-1.19.8/pyproject.toml
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 playwrightcapture-1.19.8/PKG-INFO
```

### Comparing `playwrightcapture-1.19.7/LICENSE` & `playwrightcapture-1.19.8/LICENSE`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.7/README.md` & `playwrightcapture-1.19.8/README.md`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.7/playwrightcapture/capture.py` & `playwrightcapture-1.19.8/playwrightcapture/capture.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,42 +491,42 @@
                     to_return['html'] = content
 
                 to_return['last_redirected_url'] = page.url
 
                 to_return['png'] = await self._failsafe_get_screenshot(page)
 
                 if depth > 0 and to_return.get('html') and to_return['html']:
-                    to_return['children'] = []
-                    depth -= 1
-                    child_urls = get_links_from_rendered_page(page.url, to_return['html'], rendered_hostname_only)
-                    total_urls = len(child_urls)
-                    max_capture_time = max_depth_capture_time / total_urls
-                    if max_capture_time < self.general_timeout:
-                        self.logger.warning(f'Too many URLs ({total_urls}) to capture in too little time ({max_capture_time}s), this will probably fail. Expected timeout for playwright: {self.general_timeout}.')
-                    self.logger.info(f'Capturing children, {total_urls} URLs')
-                    for index, url in enumerate(child_urls):
-                        self.logger.info(f'Capture child {url} - Timeout: {max_capture_time}s')
-                        start_time = time.time()
-                        try:
-                            child_capture = await asyncio.wait_for(
-                                self.capture_page(url=url, referer=page.url,
-                                                  page=page, depth=depth,
-                                                  rendered_hostname_only=rendered_hostname_only,
-                                                  max_depth_capture_time=max_capture_time),
-                                timeout=max_capture_time)
-                            to_return['children'].append(child_capture)  # type: ignore
-                        except (TimeoutError, asyncio.exceptions.TimeoutError):
-                            self.logger.warning(f'Timeout error, took more than {max_depth_capture_time}s. Unable to capture {url}.')
-                        else:
-                            runtime = time.time() - start_time
-                            self.logger.info(f'Successfully captured child URL: {url} in {runtime}s. {total_urls - index - 1} to go.')
-                        try:
-                            await page.go_back()
-                        except PlaywrightTimeoutError as e:
-                            self.logger.warning(f'Go back timed out, it is probably not a big deal: {e}')
+                    if child_urls := get_links_from_rendered_page(page.url, to_return['html'], rendered_hostname_only):
+                        to_return['children'] = []
+                        depth -= 1
+                        total_urls = len(child_urls)
+                        max_capture_time = max_depth_capture_time / total_urls
+                        if max_capture_time < (self.general_timeout / 1000):
+                            self.logger.warning(f'Too many URLs ({total_urls}) to capture in too little time ({max_capture_time}s), this will probably fail. Expected timeout for playwright: {self.general_timeout}.')
+                        self.logger.info(f'Capturing children, {total_urls} URLs')
+                        for index, url in enumerate(child_urls):
+                            self.logger.info(f'Capture child {url} - Timeout: {max_capture_time}s')
+                            start_time = time.time()
+                            try:
+                                child_capture = await asyncio.wait_for(
+                                    self.capture_page(url=url, referer=page.url,
+                                                      page=page, depth=depth,
+                                                      rendered_hostname_only=rendered_hostname_only,
+                                                      max_depth_capture_time=max_capture_time),
+                                    timeout=max_capture_time)
+                                to_return['children'].append(child_capture)  # type: ignore
+                            except (TimeoutError, asyncio.exceptions.TimeoutError):
+                                self.logger.warning(f'Timeout error, took more than {max_depth_capture_time}s. Unable to capture {url}.')
+                            else:
+                                runtime = int(time.time() - start_time)
+                                self.logger.info(f'Successfully captured child URL: {url} in {runtime}s. {total_urls - index - 1} to go.')
+                            try:
+                                await page.go_back()
+                            except PlaywrightTimeoutError as e:
+                                self.logger.warning(f'Go back timed out, it is probably not a big deal: {e}')
 
         except PlaywrightTimeoutError as e:
             to_return['error'] = f"The capture took too long - {e.message}"
             self.should_retry = True
         except Error as e:
             to_return['error'] = e.message
             # TODO: check e.name and figure out if it is worth retrying or not.
```

### Comparing `playwrightcapture-1.19.7/playwrightcapture/helpers.py` & `playwrightcapture-1.19.8/playwrightcapture/helpers.py`

 * *Files identical despite different names*

### Comparing `playwrightcapture-1.19.7/pyproject.toml` & `playwrightcapture-1.19.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PlaywrightCapture"
-version = "1.19.7"
+version = "1.19.8"
 description = "A simple library to capture websites using playwright"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/Lookyloo/PlaywrightCapture"
 readme = "README.md"
 
 classifiers=[
```

### Comparing `playwrightcapture-1.19.7/PKG-INFO` & `playwrightcapture-1.19.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playwrightcapture
-Version: 1.19.7
+Version: 1.19.8
 Summary: A simple library to capture websites using playwright
 Home-page: https://github.com/Lookyloo/PlaywrightCapture
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
```

