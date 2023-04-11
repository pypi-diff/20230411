# Comparing `tmp/sonos-websocket-0.0.3.tar.gz` & `tmp/sonos-websocket-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonos-websocket-0.0.3.tar", last modified: Mon Apr 10 02:59:36 2023, max compression
+gzip compressed data, was "sonos-websocket-0.0.4.tar", last modified: Tue Apr 11 02:45:55 2023, max compression
```

## Comparing `sonos-websocket-0.0.3.tar` & `sonos-websocket-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/sonos_websocket/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-04-10 02:59:25.000000 sonos-websocket-0.0.3/sonos_websocket/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 02:59:36.489954 sonos-websocket-0.0.3/sonos_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 02:59:36.000000 sonos-websocket-0.0.3/sonos_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:45:55.989349 sonos-websocket-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 02:45:55.985349 sonos-websocket-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 02:45:55.989349 sonos-websocket-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:45:55.985349 sonos-websocket-0.0.4/sonos_websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-11 02:45:40.000000 sonos-websocket-0.0.4/sonos_websocket/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 02:45:55.985349 sonos-websocket-0.0.4/sonos_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 02:45:55.000000 sonos-websocket-0.0.4/sonos_websocket.egg-info/top_level.txt
```

### Comparing `sonos-websocket-0.0.3/PKG-INFO` & `sonos-websocket-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.0.3
+Version: 0.0.4
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sonos-websocket-0.0.3/README.md` & `sonos-websocket-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.3/pyproject.toml` & `sonos-websocket-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.3/sonos_websocket/__main__.py` & `sonos-websocket-0.0.4/sonos_websocket/__main__.py`

 * *Files identical despite different names*

### Comparing `sonos-websocket-0.0.3/sonos_websocket/websocket.py` & `sonos-websocket-0.0.4/sonos_websocket/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,22 @@
         """Initialize the websocket instance."""
         self.uri = f"wss://{ip_addr}:1443/websocket/api"
         self._own_session = not session
         self.session = session or aiohttp.ClientSession()
         self.ws: aiohttp.ClientWebSocketResponse | None = None
         self._household_id = household_id
         self._player_id = player_id
+        self._connect_lock = asyncio.Lock()
 
     async def connect(self) -> None:
         """Open a persistent websocket connection and act on events."""
-        if self.ws and not self.ws.closed:
-            _LOGGER.warning("Websocket is already connected")
-            return
+        async with self._connect_lock:
+            if self.ws and not self.ws.closed:
+                _LOGGER.warning("Websocket is already connected")
+                return
 
         headers = {
             "X-Sonos-Api-Key": API_KEY,
             "Sec-WebSocket-Protocol": "v1.api.smartspeaker.audio",
         }
         try:
             self.ws = await self.session.ws_connect(
```

### Comparing `sonos-websocket-0.0.3/sonos_websocket.egg-info/PKG-INFO` & `sonos-websocket-0.0.4/sonos_websocket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonos-websocket
-Version: 0.0.3
+Version: 0.0.4
 Summary: An asynchronous Python library to communicate with Sonos devices over websockets.
 Author-email: Jason Lawrence <jjlawren@users.noreply.github.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/jjlawren/sonos-websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

