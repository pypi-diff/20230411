# Comparing `tmp/httpx-0.9.5.tar.gz` & `tmp/httpx-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/httpx-0.9.5.tar", last modified: Fri Dec 20 11:19:03 2019, max compression
+gzip compressed data, was "dist/httpx-1.0.0b0.tar", last modified: Tue Sep 14 08:48:22 2021, max compression
```

## Comparing `httpx-0.9.5.tar` & `httpx-1.0.0b0.tar`

### file list

```diff
@@ -1,45 +1,41 @@
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-12-20 11:19:03.000000 httpx-0.9.5/
--rw-r--r--   0 tomchristie   (501) staff       (20)     9632 2019-12-20 11:18:44.000000 httpx-0.9.5/CHANGELOG.md
--rw-r--r--   0 tomchristie   (501) staff       (20)     1518 2019-07-25 14:28:08.000000 httpx-0.9.5/LICENSE.md
--rw-r--r--   0 tomchristie   (501) staff       (20)       81 2019-11-15 12:08:53.000000 httpx-0.9.5/MANIFEST.in
--rw-r--r--   0 tomchristie   (501) staff       (20)    18145 2019-12-20 11:19:03.000000 httpx-0.9.5/PKG-INFO
--rw-r--r--   0 tomchristie   (501) staff       (20)     4610 2019-12-09 09:57:16.000000 httpx-0.9.5/README.md
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx/
--rw-r--r--   0 tomchristie   (501) staff       (20)     1923 2019-12-09 10:12:15.000000 httpx-0.9.5/httpx/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)      107 2019-12-20 11:18:44.000000 httpx-0.9.5/httpx/__version__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    10958 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/api.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     8221 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/auth.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    31480 2019-12-20 10:25:54.000000 httpx-0.9.5/httpx/client.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx/concurrency/
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2019-12-02 15:51:02.000000 httpx-0.9.5/httpx/concurrency/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     9883 2019-12-17 12:00:50.000000 httpx-0.9.5/httpx/concurrency/asyncio.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     1713 2019-12-12 11:58:42.000000 httpx-0.9.5/httpx/concurrency/auto.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     3417 2019-12-12 11:58:42.000000 httpx-0.9.5/httpx/concurrency/base.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     5735 2019-12-12 11:58:42.000000 httpx-0.9.5/httpx/concurrency/trio.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    11087 2019-12-09 11:01:28.000000 httpx-0.9.5/httpx/config.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     5208 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/content.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     8734 2019-12-02 10:58:35.000000 httpx-0.9.5/httpx/decoders.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx/dispatch/
--rw-r--r--   0 tomchristie   (501) staff       (20)      205 2019-11-27 10:44:13.000000 httpx-0.9.5/httpx/dispatch/__init__.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     4136 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/dispatch/asgi.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2267 2019-12-18 12:18:13.000000 httpx-0.9.5/httpx/dispatch/base.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     6863 2019-12-18 12:18:13.000000 httpx-0.9.5/httpx/dispatch/connection.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     7554 2019-12-18 12:18:13.000000 httpx-0.9.5/httpx/dispatch/connection_pool.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     7114 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/dispatch/http11.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    10910 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/dispatch/http2.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     7550 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/dispatch/proxy_http.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     2795 2019-12-05 09:44:58.000000 httpx-0.9.5/httpx/exceptions.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    36491 2019-12-20 10:51:03.000000 httpx-0.9.5/httpx/models.py
--rw-r--r--   0 tomchristie   (501) staff       (20)     4211 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/multipart.py
--rw-r--r--   0 tomchristie   (501) staff       (20)        0 2019-08-16 10:36:45.000000 httpx-0.9.5/httpx/py.typed
--rw-r--r--   0 tomchristie   (501) staff       (20)     5181 2019-12-02 10:58:35.000000 httpx-0.9.5/httpx/status_codes.py
--rw-r--r--   0 tomchristie   (501) staff       (20)    10723 2019-12-20 10:03:04.000000 httpx-0.9.5/httpx/utils.py
-drwxr-xr-x   0 tomchristie   (501) staff       (20)        0 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx.egg-info/
--rw-r--r--   0 tomchristie   (501) staff       (20)    18145 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx.egg-info/PKG-INFO
--rw-r--r--   0 tomchristie   (501) staff       (20)      827 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx.egg-info/SOURCES.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)        1 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx.egg-info/dependency_links.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)        1 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx.egg-info/not-zip-safe
--rw-r--r--   0 tomchristie   (501) staff       (20)       91 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx.egg-info/requires.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)       39 2019-12-20 11:19:03.000000 httpx-0.9.5/httpx.egg-info/top_level.txt
--rw-r--r--   0 tomchristie   (501) staff       (20)      747 2019-12-20 11:19:03.000000 httpx-0.9.5/setup.cfg
--rw-r--r--   0 tomchristie   (501) staff       (20)     2111 2019-12-04 10:09:29.000000 httpx-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 08:48:22.000000 httpx-1.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (121)    42271 2021-09-14 08:47:46.000000 httpx-1.0.0b0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1508 2021-09-14 08:47:46.000000 httpx-1.0.0b0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-09-14 08:47:46.000000 httpx-1.0.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    56930 2021-09-14 08:48:22.000000 httpx-1.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5206 2021-09-14 08:47:46.000000 httpx-1.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx/
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11713 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10242 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    64159 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11842 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6916 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10155 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7796 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12722 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68824 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6803 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_multipart.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5586 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_status_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx/_transports/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4942 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_transports/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4589 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_transports/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9324 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_transports/default.py
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_transports/mock.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4405 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_transports/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3833 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16568 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-14 08:47:46.000000 httpx-1.0.0b0/httpx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    56930 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-14 08:48:14.000000 httpx-1.0.0b0/httpx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2021-09-14 08:48:22.000000 httpx-1.0.0b0/httpx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      725 2021-09-14 08:48:22.000000 httpx-1.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2021-09-14 08:47:46.000000 httpx-1.0.0b0/setup.py
```

### Comparing `httpx-0.9.5/LICENSE.md` & `httpx-1.0.0b0/LICENSE.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,12 @@
 Copyright © 2019, [Encode OSS Ltd](https://www.encode.io/).
 All rights reserved.
 
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
 
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
+* Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
 
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
+* Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
 
-* Neither the name of the copyright holder nor the names of its
-  contributors may be used to endorse or promote products derived from
-  this software without specific prior written permission.
+* Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `httpx-0.9.5/httpx/api.py` & `httpx-1.0.0b0/httpx/_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,414 +1,438 @@
+import json
+import sys
 import typing
 
-from .auth import AuthTypes
-from .client import Client, StreamContextManager
-from .config import DEFAULT_TIMEOUT_CONFIG, CertTypes, TimeoutTypes, VerifyTypes
-from .models import (
-    CookieTypes,
-    HeaderTypes,
-    QueryParamTypes,
-    Request,
-    RequestData,
-    RequestFiles,
-    Response,
-    URLTypes,
-)
-
-
-async def request(
-    method: str,
-    url: URLTypes,
-    *,
-    params: QueryParamTypes = None,
-    data: RequestData = None,
-    files: RequestFiles = None,
-    json: typing.Any = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    auth: AuthTypes = None,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    allow_redirects: bool = True,
-    verify: VerifyTypes = True,
-    cert: CertTypes = None,
-    stream: bool = False,
-    trust_env: bool = True,
-) -> Response:
-    """
-    Sends an HTTP request.
-
-    **Parameters:**
-
-    * **method** - HTTP method for the new `Request` object: `GET`, `OPTIONS`,
-    `HEAD`, `POST`, `PUT`, `PATCH`, or `DELETE`.
-    * **url** - URL for the new `Request` object.
-    * **params** - *(optional)* Query parameters to include in the URL, as a
-    string, dictionary, or list of two-tuples.
-    * **data** - *(optional)* Data to include in the body of the request, as a
-    dictionary
-    * **files** - *(optional)* A dictionary of upload files to include in the
-    body of the request.
-    * **json** - *(optional)* A JSON serializable object to include in the body
-    of the request.
-    * **headers** - *(optional)* Dictionary of HTTP headers to include in the
-    request.
-    * **cookies** - *(optional)* Dictionary of Cookie items to include in the
-    request.
-    * **auth** - *(optional)* An authentication class to use when sending the
-    request.
-    * **timeout** - *(optional)* The timeout configuration to use when sending
-    the request.
-    * **allow_redirects** - *(optional)* Enables or disables HTTP redirects.
-    * **verify** - *(optional)* SSL certificates (a.k.a CA bundle) used to
-    verify the identity of requested hosts. Either `True` (default CA bundle),
-    a path to an SSL certificate file, or `False` (disable verification).
-    * **cert** - *(optional)* An SSL certificate used by the requested host
-    to authenticate the client. Either a path to an SSL certificate file, or
-    two-tuple of (certificate file, key file), or a three-tuple of (certificate
-    file, key file, password).
-    * **trust_env** - *(optional)* Enables or disables usage of environment
-    variables for configuration.
-    * **proxies** - *(optional)* A dictionary mapping HTTP protocols to proxy
-    URLs.
-
-    **Returns:** `Response`
-
-    Usage:
-
-    ```
-    >>> import httpx
-    >>> response = await httpx.request('GET', 'https://httpbin.org/get')
-    >>> response
-    <Response [200 OK]>
-    ```
-    """
-    async with Client(
-        cert=cert, verify=verify, timeout=timeout, trust_env=trust_env,
-    ) as client:
-        return await client.request(
-            method=method,
-            url=url,
-            data=data,
-            files=files,
-            json=json,
-            params=params,
-            headers=headers,
-            cookies=cookies,
-            stream=stream,
-            auth=auth,
-            allow_redirects=allow_redirects,
-        )
-
-
-def stream(
-    method: str,
-    url: URLTypes,
-    *,
-    params: QueryParamTypes = None,
-    data: RequestData = None,
-    files: RequestFiles = None,
-    json: typing.Any = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    auth: AuthTypes = None,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    allow_redirects: bool = True,
-    verify: VerifyTypes = True,
-    cert: CertTypes = None,
-    trust_env: bool = True,
-) -> StreamContextManager:
-    client = Client(cert=cert, verify=verify, trust_env=trust_env)
-    request = Request(
-        method=method,
-        url=url,
-        params=params,
-        data=data,
-        files=files,
-        json=json,
-        headers=headers,
-        cookies=cookies,
-    )
-    return StreamContextManager(
-        client=client,
-        request=request,
-        auth=auth,
-        timeout=timeout,
-        allow_redirects=allow_redirects,
-        close_client=True,
+import click
+import pygments.lexers
+import pygments.util
+import rich.console
+import rich.progress
+import rich.syntax
+
+from ._client import Client
+from ._exceptions import RequestError
+from ._models import Request, Response
+
+
+def print_help() -> None:
+    console = rich.console.Console()
+
+    console.print("[bold]HTTPX :butterfly:", justify="center")
+    console.print()
+    console.print("A next generation HTTP client.", justify="center")
+    console.print()
+    console.print(
+        "Usage: [bold]httpx[/bold] [cyan]<URL> [OPTIONS][/cyan] ", justify="left"
     )
+    console.print()
 
-
-async def get(
-    url: URLTypes,
-    *,
-    params: QueryParamTypes = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    stream: bool = False,
-    auth: AuthTypes = None,
-    allow_redirects: bool = True,
-    cert: CertTypes = None,
-    verify: VerifyTypes = True,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    trust_env: bool = True,
-) -> Response:
-    """
-    Sends a `GET` request.
-
-    **Parameters**: See `httpx.request`.
-
-    Note that the `data`, `files`, and `json` parameters are not available on
-    this function, as `GET` requests should not include a request body.
-    """
-    return await request(
-        "GET",
-        url,
-        params=params,
-        headers=headers,
-        cookies=cookies,
-        stream=stream,
-        auth=auth,
-        allow_redirects=allow_redirects,
-        cert=cert,
-        verify=verify,
-        timeout=timeout,
-        trust_env=trust_env,
+    table = rich.table.Table.grid(padding=1, pad_edge=True)
+    table.add_column("Parameter", no_wrap=True, justify="left", style="bold")
+    table.add_column("Description")
+    table.add_row(
+        "-m, --method [cyan]METHOD",
+        "Request method, such as GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD.\n"
+        "[Default: GET, or POST if a request body is included]",
     )
-
-
-async def options(
-    url: URLTypes,
-    *,
-    params: QueryParamTypes = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    stream: bool = False,
-    auth: AuthTypes = None,
-    allow_redirects: bool = True,
-    cert: CertTypes = None,
-    verify: VerifyTypes = True,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    trust_env: bool = True,
-) -> Response:
-    """
-    Sends an `OPTIONS` request.
-
-    **Parameters**: See `httpx.request`.
-
-    Note that the `data`, `files`, and `json` parameters are not available on
-    this function, as `OPTIONS` requests should not include a request body.
-    """
-    return await request(
-        "OPTIONS",
-        url,
-        params=params,
-        headers=headers,
-        cookies=cookies,
-        stream=stream,
-        auth=auth,
-        allow_redirects=allow_redirects,
-        cert=cert,
-        verify=verify,
-        timeout=timeout,
-        trust_env=trust_env,
+    table.add_row(
+        "-p, --params [cyan]<NAME VALUE> ...",
+        "Query parameters to include in the request URL.",
     )
-
-
-async def head(
-    url: URLTypes,
-    *,
-    params: QueryParamTypes = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    stream: bool = False,
-    auth: AuthTypes = None,
-    allow_redirects: bool = False,  # Note: Differs to usual default.
-    cert: CertTypes = None,
-    verify: VerifyTypes = True,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    trust_env: bool = True,
-) -> Response:
-    """
-    Sends a `HEAD` request.
-
-    **Parameters**: See `httpx.request`.
-
-    Note that the `data`, `files`, and `json` parameters are not available on
-    this function, as `HEAD` requests should not include a request body. The
-    `HEAD` method also differs from the other cases in that `allow_redirects`
-    defaults to `False`.
-    """
-    return await request(
-        "HEAD",
-        url,
-        params=params,
-        headers=headers,
-        cookies=cookies,
-        stream=stream,
-        auth=auth,
-        allow_redirects=allow_redirects,
-        cert=cert,
-        verify=verify,
-        timeout=timeout,
-        trust_env=trust_env,
+    table.add_row(
+        "-c, --content [cyan]TEXT", "Byte content to include in the request body."
     )
-
-
-async def post(
-    url: URLTypes,
-    *,
-    data: RequestData = None,
-    files: RequestFiles = None,
-    json: typing.Any = None,
-    params: QueryParamTypes = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    stream: bool = False,
-    auth: AuthTypes = None,
-    allow_redirects: bool = True,
-    cert: CertTypes = None,
-    verify: VerifyTypes = True,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    trust_env: bool = True,
-) -> Response:
-    """
-    Sends a `POST` request.
-
-    **Parameters**: See `httpx.request`.
-    """
-    return await request(
-        "POST",
-        url,
-        data=data,
-        files=files,
-        json=json,
-        params=params,
-        headers=headers,
-        cookies=cookies,
-        stream=stream,
-        auth=auth,
-        allow_redirects=allow_redirects,
-        cert=cert,
-        verify=verify,
-        timeout=timeout,
-        trust_env=trust_env,
+    table.add_row(
+        "-d, --data [cyan]<NAME VALUE> ...", "Form data to include in the request body."
     )
-
-
-async def put(
-    url: URLTypes,
-    *,
-    data: RequestData = None,
-    files: RequestFiles = None,
-    json: typing.Any = None,
-    params: QueryParamTypes = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    stream: bool = False,
-    auth: AuthTypes = None,
-    allow_redirects: bool = True,
-    cert: CertTypes = None,
-    verify: VerifyTypes = True,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    trust_env: bool = True,
-) -> Response:
-    """
-    Sends a `PUT` request.
-
-    **Parameters**: See `httpx.request`.
-    """
-    return await request(
-        "PUT",
-        url,
-        data=data,
-        files=files,
-        json=json,
-        params=params,
-        headers=headers,
-        cookies=cookies,
-        stream=stream,
-        auth=auth,
-        allow_redirects=allow_redirects,
-        cert=cert,
-        verify=verify,
-        timeout=timeout,
-        trust_env=trust_env,
+    table.add_row(
+        "-f, --files [cyan]<NAME FILENAME> ...",
+        "Form files to include in the request body.",
+    )
+    table.add_row("-j, --json [cyan]TEXT", "JSON data to include in the request body.")
+    table.add_row(
+        "-h, --headers [cyan]<NAME VALUE> ...",
+        "Include additional HTTP headers in the request.",
+    )
+    table.add_row(
+        "--cookies [cyan]<NAME VALUE> ...", "Cookies to include in the request."
+    )
+    table.add_row(
+        "--auth [cyan]<USER PASS>",
+        "Username and password to include in the request. Specify '-' for the password to use "
+        "a password prompt. Note that using --verbose/-v will expose the Authorization "
+        "header, including the password encoding in a trivially reverisible format.",
     )
 
+    table.add_row(
+        "--proxy [cyan]URL",
+        "Send the request via a proxy. Should be the URL giving the proxy address.",
+    )
 
-async def patch(
-    url: URLTypes,
-    *,
-    data: RequestData = None,
-    files: RequestFiles = None,
-    json: typing.Any = None,
-    params: QueryParamTypes = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    stream: bool = False,
-    auth: AuthTypes = None,
-    allow_redirects: bool = True,
-    cert: CertTypes = None,
-    verify: VerifyTypes = True,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    trust_env: bool = True,
-) -> Response:
-    """
-    Sends a `PATCH` request.
-
-    **Parameters**: See `httpx.request`.
-    """
-    return await request(
-        "PATCH",
-        url,
-        data=data,
-        files=files,
-        json=json,
-        params=params,
-        headers=headers,
-        cookies=cookies,
-        stream=stream,
-        auth=auth,
-        allow_redirects=allow_redirects,
-        cert=cert,
-        verify=verify,
-        timeout=timeout,
-        trust_env=trust_env,
+    table.add_row(
+        "--timeout [cyan]FLOAT",
+        "Timeout value to use for network operations, such as establishing the connection, "
+        "reading some data, etc... [Default: 5.0]",
     )
 
+    table.add_row("--follow-redirects", "Automatically follow redirects.")
+    table.add_row("--no-verify", "Disable SSL verification.")
+    table.add_row(
+        "--http2", "Send the request using HTTP/2, if the remote server supports it."
+    )
 
-async def delete(
-    url: URLTypes,
-    *,
-    params: QueryParamTypes = None,
-    headers: HeaderTypes = None,
-    cookies: CookieTypes = None,
-    stream: bool = False,
-    auth: AuthTypes = None,
-    allow_redirects: bool = True,
-    cert: CertTypes = None,
-    verify: VerifyTypes = True,
-    timeout: TimeoutTypes = DEFAULT_TIMEOUT_CONFIG,
-    trust_env: bool = True,
-) -> Response:
-    """
-    Sends a `DELETE` request.
+    table.add_row(
+        "--download [cyan]FILE",
+        "Save the response content as a file, rather than displaying it.",
+    )
 
-    **Parameters**: See `httpx.request`.
+    table.add_row("-v, --verbose", "Verbose output. Show request as well as response.")
+    table.add_row("--help", "Show this message and exit.")
+    console.print(table)
+
+
+def get_lexer_for_response(response: Response) -> str:
+    content_type = response.headers.get("Content-Type")
+    if content_type is not None:
+        mime_type, _, _ = content_type.partition(";")
+        try:
+            return pygments.lexers.get_lexer_for_mimetype(mime_type.strip()).name
+        except pygments.util.ClassNotFound:  # pragma: nocover
+            pass
+    return ""  # pragma: nocover
+
+
+def format_request_headers(request: Request) -> str:
+    target = request.url.raw[-1].decode("ascii")
+    lines = [f"{request.method} {target} HTTP/1.1"] + [
+        f"{name.decode('ascii')}: {value.decode('ascii')}"
+        for name, value in request.headers.raw
+    ]
+    return "\n".join(lines)
+
+
+def format_response_headers(response: Response) -> str:
+    lines = [
+        f"{response.http_version} {response.status_code} {response.reason_phrase}"
+    ] + [
+        f"{name.decode('ascii')}: {value.decode('ascii')}"
+        for name, value in response.headers.raw
+    ]
+    return "\n".join(lines)
+
+
+def print_request_headers(request: Request) -> None:
+    console = rich.console.Console()
+    http_text = format_request_headers(request)
+    syntax = rich.syntax.Syntax(http_text, "http", theme="ansi_dark", word_wrap=True)
+    console.print(syntax)
+    syntax = rich.syntax.Syntax("", "http", theme="ansi_dark", word_wrap=True)
+    console.print(syntax)
+
+
+def print_response_headers(response: Response) -> None:
+    console = rich.console.Console()
+    http_text = format_response_headers(response)
+    syntax = rich.syntax.Syntax(http_text, "http", theme="ansi_dark", word_wrap=True)
+    console.print(syntax)
+
+
+def print_delimiter() -> None:
+    console = rich.console.Console()
+    syntax = rich.syntax.Syntax("", "http", theme="ansi_dark", word_wrap=True)
+    console.print(syntax)
+
+
+def print_redirects(response: Response) -> None:
+    if response.has_redirect_location:
+        response.read()
+        print_response_headers(response)
+        print_response(response)
+
+
+def print_response(response: Response) -> None:
+    console = rich.console.Console()
+    lexer_name = get_lexer_for_response(response)
+    if lexer_name:
+        if lexer_name.lower() == "json":
+            try:
+                data = response.json()
+                text = json.dumps(data, indent=4)
+            except ValueError:  # pragma: nocover
+                text = response.text
+        else:
+            text = response.text
+        syntax = rich.syntax.Syntax(text, lexer_name, theme="ansi_dark", word_wrap=True)
+        console.print(syntax)
+    else:  # pragma: nocover
+        console.print(response.text)
+
+
+def download_response(response: Response, download: typing.BinaryIO) -> None:
+    console = rich.console.Console()
+    syntax = rich.syntax.Syntax("", "http", theme="ansi_dark", word_wrap=True)
+    console.print(syntax)
+
+    content_length = response.headers.get("Content-Length")
+    kwargs = {"total": int(content_length)} if content_length else {}
+    with rich.progress.Progress(
+        "[progress.description]{task.description}",
+        "[progress.percentage]{task.percentage:>3.0f}%",
+        rich.progress.BarColumn(bar_width=None),
+        rich.progress.DownloadColumn(),
+        rich.progress.TransferSpeedColumn(),
+    ) as progress:
+        description = f"Downloading [bold]{download.name}"
+        download_task = progress.add_task(description, **kwargs)  # type: ignore
+        for chunk in response.iter_bytes():
+            download.write(chunk)
+            progress.update(download_task, completed=response.num_bytes_downloaded)
+
+
+def validate_json(
+    ctx: click.Context,
+    param: typing.Union[click.Option, click.Parameter],
+    value: typing.Any,
+) -> typing.Any:
+    if value is None:
+        return None
+
+    try:
+        return json.loads(value)
+    except json.JSONDecodeError:  # pragma: nocover
+        raise click.BadParameter("Not valid JSON")
+
+
+def validate_auth(
+    ctx: click.Context,
+    param: typing.Union[click.Option, click.Parameter],
+    value: typing.Any,
+) -> typing.Any:
+    if value == (None, None):
+        return None
+
+    username, password = value
+    if password == "-":  # pragma: nocover
+        password = click.prompt("Password", hide_input=True)
+    return (username, password)
+
+
+def handle_help(
+    ctx: click.Context,
+    param: typing.Union[click.Option, click.Parameter],
+    value: typing.Any,
+) -> None:
+    if not value or ctx.resilient_parsing:
+        return
+
+    print_help()
+    ctx.exit()
+
+
+@click.command(add_help_option=False)
+@click.argument("url", type=str)
+@click.option(
+    "--method",
+    "-m",
+    "method",
+    type=str,
+    help=(
+        "Request method, such as GET, POST, PUT, PATCH, DELETE, OPTIONS, HEAD. "
+        "[Default: GET, or POST if a request body is included]"
+    ),
+)
+@click.option(
+    "--params",
+    "-p",
+    "params",
+    type=(str, str),
+    multiple=True,
+    help="Query parameters to include in the request URL.",
+)
+@click.option(
+    "--content",
+    "-c",
+    "content",
+    type=str,
+    help="Byte content to include in the request body.",
+)
+@click.option(
+    "--data",
+    "-d",
+    "data",
+    type=(str, str),
+    multiple=True,
+    help="Form data to include in the request body.",
+)
+@click.option(
+    "--files",
+    "-f",
+    "files",
+    type=(str, click.File(mode="rb")),
+    multiple=True,
+    help="Form files to include in the request body.",
+)
+@click.option(
+    "--json",
+    "-j",
+    "json",
+    type=str,
+    callback=validate_json,
+    help="JSON data to include in the request body.",
+)
+@click.option(
+    "--headers",
+    "-h",
+    "headers",
+    type=(str, str),
+    multiple=True,
+    help="Include additional HTTP headers in the request.",
+)
+@click.option(
+    "--cookies",
+    "cookies",
+    type=(str, str),
+    multiple=True,
+    help="Cookies to include in the request.",
+)
+@click.option(
+    "--auth",
+    "auth",
+    type=(str, str),
+    default=(None, None),
+    callback=validate_auth,
+    help=(
+        "Username and password to include in the request. "
+        "Specify '-' for the password to use a password prompt. "
+        "Note that using --verbose/-v will expose the Authorization header, "
+        "including the password encoding in a trivially reverisible format."
+    ),
+)
+@click.option(
+    "--proxies",
+    "proxies",
+    type=str,
+    default=None,
+    help="Send the request via a proxy. Should be the URL giving the proxy address.",
+)
+@click.option(
+    "--timeout",
+    "timeout",
+    type=float,
+    default=5.0,
+    help=(
+        "Timeout value to use for network operations, such as establishing the "
+        "connection, reading some data, etc... [Default: 5.0]"
+    ),
+)
+@click.option(
+    "--follow-redirects",
+    "follow_redirects",
+    is_flag=True,
+    default=False,
+    help="Automatically follow redirects.",
+)
+@click.option(
+    "--no-verify",
+    "verify",
+    is_flag=True,
+    default=True,
+    help="Disable SSL verification.",
+)
+@click.option(
+    "--http2",
+    "http2",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Send the request using HTTP/2, if the remote server supports it.",
+)
+@click.option(
+    "--download",
+    type=click.File("wb"),
+    help="Save the response content as a file, rather than displaying it.",
+)
+@click.option(
+    "--verbose",
+    "-v",
+    type=bool,
+    is_flag=True,
+    default=False,
+    help="Verbose. Show request as well as response.",
+)
+@click.option(
+    "--help",
+    is_flag=True,
+    is_eager=True,
+    expose_value=False,
+    callback=handle_help,
+    help="Show this message and exit.",
+)
+def main(
+    url: str,
+    method: str,
+    params: typing.List[typing.Tuple[str, str]],
+    content: str,
+    data: typing.List[typing.Tuple[str, str]],
+    files: typing.List[typing.Tuple[str, click.File]],
+    json: str,
+    headers: typing.List[typing.Tuple[str, str]],
+    cookies: typing.List[typing.Tuple[str, str]],
+    auth: typing.Optional[typing.Tuple[str, str]],
+    proxies: str,
+    timeout: float,
+    follow_redirects: bool,
+    verify: bool,
+    http2: bool,
+    download: typing.Optional[typing.BinaryIO],
+    verbose: bool,
+) -> None:
+    """
+    An HTTP command line client.
+    Sends a request and displays the response.
+    """
+    if not method:
+        method = "POST" if content or data or files or json else "GET"
+
+    event_hooks: typing.Dict[str, typing.List[typing.Callable]] = {}
+    if verbose:
+        event_hooks["request"] = [print_request_headers]
+    if follow_redirects:
+        event_hooks["response"] = [print_redirects]
+
+    try:
+        with Client(
+            proxies=proxies,
+            timeout=timeout,
+            verify=verify,
+            http2=http2,
+            event_hooks=event_hooks,
+        ) as client:
+            with client.stream(
+                method,
+                url,
+                params=list(params),
+                content=content,
+                data=dict(data),
+                files=files,  # type: ignore
+                json=json,
+                headers=headers,
+                cookies=dict(cookies),
+                auth=auth,
+                follow_redirects=follow_redirects,
+            ) as response:
+                print_response_headers(response)
+
+                if download is not None:
+                    download_response(response, download)
+                else:
+                    response.read()
+                    if response.content:
+                        print_delimiter()
+                        print_response(response)
+
+    except RequestError as exc:
+        console = rich.console.Console()
+        console.print(f"{type(exc).__name__}: {exc}")
+        sys.exit(1)
 
-    Note that the `data`, `files`, and `json` parameters are not available on
-    this function, as `DELETE` requests should not include a request body.
-    """
-    return await request(
-        "DELETE",
-        url,
-        params=params,
-        headers=headers,
-        cookies=cookies,
-        stream=stream,
-        auth=auth,
-        allow_redirects=allow_redirects,
-        cert=cert,
-        verify=verify,
-        timeout=timeout,
-        trust_env=trust_env,
-    )
+    sys.exit(0 if response.is_success else 1)
```

### Comparing `httpx-0.9.5/httpx/auth.py` & `httpx-1.0.0b0/httpx/_auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,33 +2,36 @@
 import os
 import re
 import time
 import typing
 from base64 import b64encode
 from urllib.request import parse_http_list
 
-from .exceptions import ProtocolError
-from .models import Request, Response
-from .utils import to_bytes, to_str, unquote
-
-AuthFlow = typing.Generator[Request, Response, None]
-
-AuthTypes = typing.Union[
-    typing.Tuple[typing.Union[str, bytes], typing.Union[str, bytes]],
-    typing.Callable[["Request"], "Request"],
-    "Auth",
-]
+from ._exceptions import ProtocolError
+from ._models import Request, Response
+from ._utils import to_bytes, to_str, unquote
 
 
 class Auth:
     """
     Base class for all authentication schemes.
+
+    To implement a custom authentication scheme, subclass `Auth` and override
+    the `.auth_flow()` method.
+
+    If the authentication scheme does I/O such as disk access or network calls, or uses
+    synchronization primitives such as locks, you should override `.sync_auth_flow()`
+    and/or `.async_auth_flow()` instead of `.auth_flow()` to provide specialized
+    implementations that will be used by `Client` and `AsyncClient` respectively.
     """
 
-    def __call__(self, request: Request) -> AuthFlow:
+    requires_request_body = False
+    requires_response_body = False
+
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
         """
         Execute the authentication flow.
 
         To dispatch a request, `yield` it:
 
         ```
         yield request
@@ -44,118 +47,202 @@
         A `return` (or reaching the end of the generator) will result in the
         client returning the last response obtained from the server.
 
         You can dispatch as many requests as is necessary.
         """
         yield request
 
+    def sync_auth_flow(
+        self, request: Request
+    ) -> typing.Generator[Request, Response, None]:
+        """
+        Execute the authentication flow synchronously.
+
+        By default, this defers to `.auth_flow()`. You should override this method
+        when the authentication scheme does I/O and/or uses concurrency primitives.
+        """
+        if self.requires_request_body:
+            request.read()
+
+        flow = self.auth_flow(request)
+        request = next(flow)
+
+        while True:
+            response = yield request
+            if self.requires_response_body:
+                response.read()
+
+            try:
+                request = flow.send(response)
+            except StopIteration:
+                break
+
+    async def async_auth_flow(
+        self, request: Request
+    ) -> typing.AsyncGenerator[Request, Response]:
+        """
+        Execute the authentication flow asynchronously.
+
+        By default, this defers to `.auth_flow()`. You should override this method
+        when the authentication scheme does I/O and/or uses concurrency primitives.
+        """
+        if self.requires_request_body:
+            await request.aread()
+
+        flow = self.auth_flow(request)
+        request = next(flow)
+
+        while True:
+            response = yield request
+            if self.requires_response_body:
+                await response.aread()
+
+            try:
+                request = flow.send(response)
+            except StopIteration:
+                break
+
 
 class FunctionAuth(Auth):
     """
     Allows the 'auth' argument to be passed as a simple callable function,
     that takes the request, and returns a new, modified request.
     """
 
     def __init__(self, func: typing.Callable[[Request], Request]) -> None:
-        self.func = func
+        self._func = func
 
-    def __call__(self, request: Request) -> AuthFlow:
-        yield self.func(request)
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
+        yield self._func(request)
 
 
 class BasicAuth(Auth):
     """
     Allows the 'auth' argument to be passed as a (username, password) pair,
     and uses HTTP Basic authentication.
     """
 
     def __init__(
         self, username: typing.Union[str, bytes], password: typing.Union[str, bytes]
     ):
-        self.auth_header = self.build_auth_header(username, password)
+        self._auth_header = self._build_auth_header(username, password)
 
-    def __call__(self, request: Request) -> AuthFlow:
-        request.headers["Authorization"] = self.auth_header
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
+        request.headers["Authorization"] = self._auth_header
         yield request
 
-    def build_auth_header(
+    def _build_auth_header(
         self, username: typing.Union[str, bytes], password: typing.Union[str, bytes]
     ) -> str:
         userpass = b":".join((to_bytes(username), to_bytes(password)))
-        token = b64encode(userpass).decode().strip()
+        token = b64encode(userpass).decode()
         return f"Basic {token}"
 
 
 class DigestAuth(Auth):
-    ALGORITHM_TO_HASH_FUNCTION: typing.Dict[str, typing.Callable] = {
+    _ALGORITHM_TO_HASH_FUNCTION: typing.Dict[str, typing.Callable] = {
         "MD5": hashlib.md5,
         "MD5-SESS": hashlib.md5,
         "SHA": hashlib.sha1,
         "SHA-SESS": hashlib.sha1,
         "SHA-256": hashlib.sha256,
         "SHA-256-SESS": hashlib.sha256,
         "SHA-512": hashlib.sha512,
         "SHA-512-SESS": hashlib.sha512,
     }
 
     def __init__(
         self, username: typing.Union[str, bytes], password: typing.Union[str, bytes]
     ) -> None:
-        self.username = to_bytes(username)
-        self.password = to_bytes(password)
+        self._username = to_bytes(username)
+        self._password = to_bytes(password)
 
-    def __call__(self, request: Request) -> AuthFlow:
+    def auth_flow(self, request: Request) -> typing.Generator[Request, Response, None]:
         response = yield request
 
         if response.status_code != 401 or "www-authenticate" not in response.headers:
-            # If the response is not a 401 WWW-Authenticate, then we don't
+            # If the response is not a 401 then we don't
             # need to build an authenticated request.
             return
 
-        header = response.headers["www-authenticate"]
-        try:
-            challenge = DigestAuthChallenge.from_header(header)
-        except ValueError:
-            raise ProtocolError("Malformed Digest authentication header")
+        for auth_header in response.headers.get_list("www-authenticate"):
+            if auth_header.lower().startswith("digest "):
+                break
+        else:
+            # If the response does not include a 'WWW-Authenticate: Digest ...'
+            # header, then we don't need to build an authenticated request.
+            return
 
+        challenge = self._parse_challenge(request, response, auth_header)
         request.headers["Authorization"] = self._build_auth_header(request, challenge)
         yield request
 
+    def _parse_challenge(
+        self, request: Request, response: Response, auth_header: str
+    ) -> "_DigestAuthChallenge":
+        """
+        Returns a challenge from a Digest WWW-Authenticate header.
+        These take the form of:
+        `Digest realm="realm@host.com",qop="auth,auth-int",nonce="abc",opaque="xyz"`
+        """
+        scheme, _, fields = auth_header.partition(" ")
+
+        # This method should only ever have been called with a Digest auth header.
+        assert scheme.lower() == "digest"
+
+        header_dict: typing.Dict[str, str] = {}
+        for field in parse_http_list(fields):
+            key, value = field.strip().split("=", 1)
+            header_dict[key] = unquote(value)
+
+        try:
+            realm = header_dict["realm"].encode()
+            nonce = header_dict["nonce"].encode()
+            algorithm = header_dict.get("algorithm", "MD5")
+            opaque = header_dict["opaque"].encode() if "opaque" in header_dict else None
+            qop = header_dict["qop"].encode() if "qop" in header_dict else None
+            return _DigestAuthChallenge(
+                realm=realm, nonce=nonce, algorithm=algorithm, opaque=opaque, qop=qop
+            )
+        except KeyError as exc:
+            message = "Malformed Digest WWW-Authenticate header"
+            raise ProtocolError(message, request=request) from exc
+
     def _build_auth_header(
-        self, request: Request, challenge: "DigestAuthChallenge"
+        self, request: Request, challenge: "_DigestAuthChallenge"
     ) -> str:
-        hash_func = self.ALGORITHM_TO_HASH_FUNCTION[challenge.algorithm]
+        hash_func = self._ALGORITHM_TO_HASH_FUNCTION[challenge.algorithm]
 
         def digest(data: bytes) -> bytes:
             return hash_func(data).hexdigest().encode()
 
-        A1 = b":".join((self.username, challenge.realm, self.password))
+        A1 = b":".join((self._username, challenge.realm, self._password))
 
-        path = request.url.full_path.encode("utf-8")
+        path = request.url.raw_path
         A2 = b":".join((request.method.encode(), path))
         # TODO: implement auth-int
         HA2 = digest(A2)
 
         nonce_count = 1  # TODO: implement nonce counting
         nc_value = b"%08x" % nonce_count
         cnonce = self._get_client_nonce(nonce_count, challenge.nonce)
 
         HA1 = digest(A1)
         if challenge.algorithm.lower().endswith("-sess"):
             HA1 = digest(b":".join((HA1, challenge.nonce, cnonce)))
 
-        qop = self._resolve_qop(challenge.qop)
+        qop = self._resolve_qop(challenge.qop, request=request)
         if qop is None:
             digest_data = [HA1, challenge.nonce, HA2]
         else:
             digest_data = [challenge.nonce, nc_value, cnonce, qop, HA2]
         key_digest = b":".join(digest_data)
 
         format_args = {
-            "username": self.username,
+            "username": self._username,
             "realm": challenge.realm,
             "nonce": challenge.nonce,
             "uri": path,
             "response": digest(b":".join((HA1, key_digest))),
             "algorithm": challenge.algorithm.encode(),
         }
         if challenge.opaque:
@@ -189,65 +276,29 @@
                 if field not in NON_QUOTED_FIELDS
                 else NON_QUOTED_TEMPLATE
             )
             header_value += template.format(field, to_str(value))
 
         return header_value
 
-    def _resolve_qop(self, qop: typing.Optional[bytes]) -> typing.Optional[bytes]:
+    def _resolve_qop(
+        self, qop: typing.Optional[bytes], request: Request
+    ) -> typing.Optional[bytes]:
         if qop is None:
             return None
         qops = re.split(b", ?", qop)
         if b"auth" in qops:
             return b"auth"
 
         if qops == [b"auth-int"]:
             raise NotImplementedError("Digest auth-int support is not yet implemented")
 
-        raise ProtocolError(f'Unexpected qop value "{qop!r}" in digest auth')
+        message = f'Unexpected qop value "{qop!r}" in digest auth'
+        raise ProtocolError(message, request=request)
 
 
-class DigestAuthChallenge:
-    def __init__(
-        self,
-        realm: bytes,
-        nonce: bytes,
-        algorithm: str = None,
-        opaque: typing.Optional[bytes] = None,
-        qop: typing.Optional[bytes] = None,
-    ) -> None:
-        self.realm = realm
-        self.nonce = nonce
-        self.algorithm = algorithm or "MD5"
-        self.opaque = opaque
-        self.qop = qop
-
-    @classmethod
-    def from_header(cls, header: str) -> "DigestAuthChallenge":
-        """Returns a challenge from a Digest WWW-Authenticate header.
-        These take the form of:
-        `Digest realm="realm@host.com",qop="auth,auth-int",nonce="abc",opaque="xyz"`
-        """
-        scheme, _, fields = header.partition(" ")
-        if scheme.lower() != "digest":
-            raise ValueError("Header does not start with 'Digest'")
-
-        header_dict: typing.Dict[str, str] = {}
-        for field in parse_http_list(fields):
-            key, value = field.strip().split("=", 1)
-            header_dict[key] = unquote(value)
-
-        try:
-            return cls.from_header_dict(header_dict)
-        except KeyError as exc:
-            raise ValueError("Malformed Digest WWW-Authenticate header") from exc
-
-    @classmethod
-    def from_header_dict(cls, header_dict: dict) -> "DigestAuthChallenge":
-        realm = header_dict["realm"].encode()
-        nonce = header_dict["nonce"].encode()
-        qop = header_dict["qop"].encode() if "qop" in header_dict else None
-        opaque = header_dict["opaque"].encode() if "opaque" in header_dict else None
-        algorithm = header_dict.get("algorithm")
-        return cls(
-            realm=realm, nonce=nonce, qop=qop, opaque=opaque, algorithm=algorithm
-        )
+class _DigestAuthChallenge(typing.NamedTuple):
+    realm: bytes
+    nonce: bytes
+    algorithm: str
+    opaque: typing.Optional[bytes]
+    qop: typing.Optional[bytes]
```

### Comparing `httpx-0.9.5/httpx/config.py` & `httpx-1.0.0b0/httpx/_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import os
 import ssl
 import typing
+from base64 import b64encode
 from pathlib import Path
 
 import certifi
 
-from .__version__ import __version__
-from .utils import get_ca_bundle_from_env, get_logger
-
-CertTypes = typing.Union[str, typing.Tuple[str, str], typing.Tuple[str, str, str]]
-VerifyTypes = typing.Union[str, bool, ssl.SSLContext]
-TimeoutTypes = typing.Union[float, typing.Tuple[float, float, float, float], "Timeout"]
-
-
-USER_AGENT = f"python-httpx/{__version__}"
+from ._compat import set_minimum_tls_version_1_2
+from ._models import URL, Headers
+from ._types import CertTypes, HeaderTypes, TimeoutTypes, URLTypes, VerifyTypes
+from ._utils import get_ca_bundle_from_env, get_logger
 
 DEFAULT_CIPHERS = ":".join(
     [
         "ECDHE+AESGCM",
         "ECDHE+CHACHA20",
         "DHE+AESGCM",
         "DHE+CHACHA20",
@@ -41,110 +37,94 @@
 class UnsetType:
     pass  # pragma: nocover
 
 
 UNSET = UnsetType()
 
 
+def create_ssl_context(
+    cert: CertTypes = None,
+    verify: VerifyTypes = True,
+    trust_env: bool = True,
+    http2: bool = False,
+) -> ssl.SSLContext:
+    return SSLConfig(
+        cert=cert, verify=verify, trust_env=trust_env, http2=http2
+    ).ssl_context
+
+
 class SSLConfig:
     """
     SSL Configuration.
     """
 
     DEFAULT_CA_BUNDLE_PATH = Path(certifi.where())
 
     def __init__(
         self,
         *,
         cert: CertTypes = None,
         verify: VerifyTypes = True,
-        trust_env: bool = None,
+        trust_env: bool = True,
+        http2: bool = False,
     ):
         self.cert = cert
-
-        # Allow passing in our own SSLContext object that's pre-configured.
-        # If you do this we assume that you want verify=True as well.
-        ssl_context = None
-        if isinstance(verify, ssl.SSLContext):
-            ssl_context = verify
-            verify = True
-            self._load_client_certs(ssl_context)
-
-        self.ssl_context: typing.Optional[ssl.SSLContext] = ssl_context
-        self.verify: typing.Union[str, bool] = verify
+        self.verify = verify
         self.trust_env = trust_env
+        self.http2 = http2
+        self.ssl_context = self.load_ssl_context()
 
-    def __eq__(self, other: typing.Any) -> bool:
-        return (
-            isinstance(other, self.__class__)
-            and self.cert == other.cert
-            and self.verify == other.verify
-        )
-
-    def __repr__(self) -> str:
-        class_name = self.__class__.__name__
-        return f"{class_name}(cert={self.cert}, verify={self.verify})"
-
-    def with_overrides(
-        self, cert: CertTypes = None, verify: VerifyTypes = None
-    ) -> "SSLConfig":
-        cert = self.cert if cert is None else cert
-        verify = self.verify if verify is None else verify
-        if (cert == self.cert) and (verify == self.verify):
-            return self
-        return SSLConfig(cert=cert, verify=verify)
-
-    def load_ssl_context(self, http2: bool = False) -> ssl.SSLContext:
+    def load_ssl_context(self) -> ssl.SSLContext:
         logger.trace(
             f"load_ssl_context "
             f"verify={self.verify!r} "
             f"cert={self.cert!r} "
             f"trust_env={self.trust_env!r} "
-            f"http2={http2!r}"
+            f"http2={self.http2!r}"
         )
 
-        if self.ssl_context is None:
-            self.ssl_context = (
-                self.load_ssl_context_verify(http2=http2)
-                if self.verify
-                else self.load_ssl_context_no_verify(http2=http2)
-            )
-
-        assert self.ssl_context is not None
-        return self.ssl_context
+        if self.verify:
+            return self.load_ssl_context_verify()
+        return self.load_ssl_context_no_verify()
 
-    def load_ssl_context_no_verify(self, http2: bool = False) -> ssl.SSLContext:
+    def load_ssl_context_no_verify(self) -> ssl.SSLContext:
         """
         Return an SSL context for unverified connections.
         """
-        context = self._create_default_ssl_context(http2=http2)
-        context.verify_mode = ssl.CERT_NONE
+        context = self._create_default_ssl_context()
         context.check_hostname = False
+        context.verify_mode = ssl.CERT_NONE
+        self._load_client_certs(context)
         return context
 
-    def load_ssl_context_verify(self, http2: bool = False) -> ssl.SSLContext:
+    def load_ssl_context_verify(self) -> ssl.SSLContext:
         """
         Return an SSL context for verified connections.
         """
         if self.trust_env and self.verify is True:
             ca_bundle = get_ca_bundle_from_env()
             if ca_bundle is not None:
-                self.verify = ca_bundle  # type: ignore
+                self.verify = ca_bundle
 
-        if isinstance(self.verify, bool):
+        if isinstance(self.verify, ssl.SSLContext):
+            # Allow passing in our own SSLContext object that's pre-configured.
+            context = self.verify
+            self._load_client_certs(context)
+            return context
+        elif isinstance(self.verify, bool):
             ca_bundle_path = self.DEFAULT_CA_BUNDLE_PATH
         elif Path(self.verify).exists():
             ca_bundle_path = Path(self.verify)
         else:
             raise IOError(
                 "Could not find a suitable TLS CA certificate bundle, "
                 "invalid path: {}".format(self.verify)
             )
 
-        context = self._create_default_ssl_context(http2=http2)
+        context = self._create_default_ssl_context()
         context.verify_mode = ssl.CERT_REQUIRED
         context.check_hostname = True
 
         # Signal to server support for PHA in TLS 1.3. Raises an
         # AttributeError if only read-only access is implemented.
         try:
             context.post_handshake_auth = True  # type: ignore
@@ -165,32 +145,29 @@
             logger.trace(f"load_verify_locations capath={ca_bundle_path!s}")
             context.load_verify_locations(capath=str(ca_bundle_path))
 
         self._load_client_certs(context)
 
         return context
 
-    def _create_default_ssl_context(self, http2: bool) -> ssl.SSLContext:
+    def _create_default_ssl_context(self) -> ssl.SSLContext:
         """
         Creates the default SSLContext object that's used for both verified
         and unverified connections.
         """
-        context = ssl.SSLContext(ssl.PROTOCOL_TLS)
-        context.options |= ssl.OP_NO_SSLv2
-        context.options |= ssl.OP_NO_SSLv3
-        context.options |= ssl.OP_NO_TLSv1
-        context.options |= ssl.OP_NO_TLSv1_1
+        context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+        set_minimum_tls_version_1_2(context)
         context.options |= ssl.OP_NO_COMPRESSION
         context.set_ciphers(DEFAULT_CIPHERS)
 
         if ssl.HAS_ALPN:
-            alpn_idents = ["http/1.1", "h2"] if http2 else ["http/1.1"]
+            alpn_idents = ["http/1.1", "h2"] if self.http2 else ["http/1.1"]
             context.set_alpn_protocols(alpn_idents)
 
-        if hasattr(context, "keylog_filename"):
+        if hasattr(context, "keylog_filename"):  # pragma: nocover (Available in 3.8+)
             keylogfile = os.environ.get("SSLKEYLOGFILE")
             if keylogfile and self.trust_env:
                 context.keylog_filename = keylogfile  # type: ignore
 
         return context
 
     def _load_client_certs(self, ssl_context: ssl.SSLContext) -> None:
@@ -212,117 +189,161 @@
 
 class Timeout:
     """
     Timeout configuration.
 
     **Usage**:
 
-    Timeout()                           # No timeout.
-    Timeout(5.0)                        # 5s timeout on all operations.
-    Timeout(connect_timeout=5.0)        # 5s timeout on connect, no other timeouts.
-    Timeout(5.0, connect_timeout=10.0)  # 10s timeout on connect. 5s timeout elsewhere.
-    Timeout(5.0, pool_timeout=None)     # No timeout on acquiring connection from pool.
-                                        # 5s timeout elsewhere.
+    Timeout(None)               # No timeouts.
+    Timeout(5.0)                # 5s timeout on all operations.
+    Timeout(None, connect=5.0)  # 5s timeout on connect, no other timeouts.
+    Timeout(5.0, connect=10.0)  # 10s timeout on connect. 5s timeout elsewhere.
+    Timeout(5.0, pool=None)     # No timeout on acquiring connection from pool.
+                                # 5s timeout elsewhere.
     """
 
     def __init__(
         self,
-        timeout: TimeoutTypes = None,
+        timeout: typing.Union[TimeoutTypes, UnsetType] = UNSET,
         *,
-        connect_timeout: typing.Union[None, float, UnsetType] = UNSET,
-        read_timeout: typing.Union[None, float, UnsetType] = UNSET,
-        write_timeout: typing.Union[None, float, UnsetType] = UNSET,
-        pool_timeout: typing.Union[None, float, UnsetType] = UNSET,
+        connect: typing.Union[None, float, UnsetType] = UNSET,
+        read: typing.Union[None, float, UnsetType] = UNSET,
+        write: typing.Union[None, float, UnsetType] = UNSET,
+        pool: typing.Union[None, float, UnsetType] = UNSET,
     ):
         if isinstance(timeout, Timeout):
             # Passed as a single explicit Timeout.
-            assert connect_timeout is UNSET
-            assert read_timeout is UNSET
-            assert write_timeout is UNSET
-            assert pool_timeout is UNSET
-            self.connect_timeout = (
-                timeout.connect_timeout
-            )  # type: typing.Optional[float]
-            self.read_timeout = timeout.read_timeout  # type: typing.Optional[float]
-            self.write_timeout = timeout.write_timeout  # type: typing.Optional[float]
-            self.pool_timeout = timeout.pool_timeout  # type: typing.Optional[float]
+            assert connect is UNSET
+            assert read is UNSET
+            assert write is UNSET
+            assert pool is UNSET
+            self.connect = timeout.connect  # type: typing.Optional[float]
+            self.read = timeout.read  # type: typing.Optional[float]
+            self.write = timeout.write  # type: typing.Optional[float]
+            self.pool = timeout.pool  # type: typing.Optional[float]
         elif isinstance(timeout, tuple):
             # Passed as a tuple.
-            self.connect_timeout = timeout[0]
-            self.read_timeout = timeout[1]
-            self.write_timeout = None if len(timeout) < 3 else timeout[2]
-            self.pool_timeout = None if len(timeout) < 4 else timeout[3]
+            self.connect = timeout[0]
+            self.read = timeout[1]
+            self.write = None if len(timeout) < 3 else timeout[2]
+            self.pool = None if len(timeout) < 4 else timeout[3]
+        elif not (
+            isinstance(connect, UnsetType)
+            or isinstance(read, UnsetType)
+            or isinstance(write, UnsetType)
+            or isinstance(pool, UnsetType)
+        ):
+            self.connect = connect
+            self.read = read
+            self.write = write
+            self.pool = pool
         else:
-            self.connect_timeout = (
-                timeout if isinstance(connect_timeout, UnsetType) else connect_timeout
-            )
-            self.read_timeout = (
-                timeout if isinstance(read_timeout, UnsetType) else read_timeout
-            )
-            self.write_timeout = (
-                timeout if isinstance(write_timeout, UnsetType) else write_timeout
-            )
-            self.pool_timeout = (
-                timeout if isinstance(pool_timeout, UnsetType) else pool_timeout
-            )
+            if isinstance(timeout, UnsetType):
+                raise ValueError(
+                    "httpx.Timeout must either include a default, or set all "
+                    "four parameters explicitly."
+                )
+            self.connect = timeout if isinstance(connect, UnsetType) else connect
+            self.read = timeout if isinstance(read, UnsetType) else read
+            self.write = timeout if isinstance(write, UnsetType) else write
+            self.pool = timeout if isinstance(pool, UnsetType) else pool
+
+    def as_dict(self) -> typing.Dict[str, typing.Optional[float]]:
+        return {
+            "connect": self.connect,
+            "read": self.read,
+            "write": self.write,
+            "pool": self.pool,
+        }
 
     def __eq__(self, other: typing.Any) -> bool:
         return (
             isinstance(other, self.__class__)
-            and self.connect_timeout == other.connect_timeout
-            and self.read_timeout == other.read_timeout
-            and self.write_timeout == other.write_timeout
-            and self.pool_timeout == other.pool_timeout
+            and self.connect == other.connect
+            and self.read == other.read
+            and self.write == other.write
+            and self.pool == other.pool
         )
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
-        if (
-            len(
-                {
-                    self.connect_timeout,
-                    self.read_timeout,
-                    self.write_timeout,
-                    self.pool_timeout,
-                }
-            )
-            == 1
-        ):
-            return f"{class_name}(timeout={self.connect_timeout})"
+        if len({self.connect, self.read, self.write, self.pool}) == 1:
+            return f"{class_name}(timeout={self.connect})"
         return (
-            f"{class_name}(connect_timeout={self.connect_timeout}, "
-            f"read_timeout={self.read_timeout}, write_timeout={self.write_timeout}, "
-            f"pool_timeout={self.pool_timeout})"
+            f"{class_name}(connect={self.connect}, "
+            f"read={self.read}, write={self.write}, pool={self.pool})"
         )
 
 
-class PoolLimits:
+class Limits:
     """
-    Limits on the number of connections in a connection pool.
+    Configuration for limits to various client behaviors.
+
+    **Parameters:**
+
+    * **max_connections** - The maximum number of concurrent connections that may be
+            established.
+    * **max_keepalive_connections** - Allow the connection pool to maintain
+            keep-alive connections below this point. Should be less than or equal
+            to `max_connections`.
     """
 
     def __init__(
-        self, *, soft_limit: int = None, hard_limit: int = None,
+        self,
+        *,
+        max_connections: int = None,
+        max_keepalive_connections: int = None,
+        keepalive_expiry: typing.Optional[float] = 5.0,
     ):
-        self.soft_limit = soft_limit
-        self.hard_limit = hard_limit
+        self.max_connections = max_connections
+        self.max_keepalive_connections = max_keepalive_connections
+        self.keepalive_expiry = keepalive_expiry
 
     def __eq__(self, other: typing.Any) -> bool:
         return (
             isinstance(other, self.__class__)
-            and self.soft_limit == other.soft_limit
-            and self.hard_limit == other.hard_limit
+            and self.max_connections == other.max_connections
+            and self.max_keepalive_connections == other.max_keepalive_connections
+            and self.keepalive_expiry == other.keepalive_expiry
         )
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
         return (
-            f"{class_name}(soft_limit={self.soft_limit}, hard_limit={self.hard_limit})"
+            f"{class_name}(max_connections={self.max_connections}, "
+            f"max_keepalive_connections={self.max_keepalive_connections}, "
+            f"keepalive_expiry={self.keepalive_expiry})"
         )
 
 
-TimeoutConfig = Timeout  # Synonym for backwards compat
+class Proxy:
+    def __init__(self, url: URLTypes, *, headers: HeaderTypes = None):
+        url = URL(url)
+        headers = Headers(headers)
+
+        if url.scheme not in ("http", "https"):
+            raise ValueError(f"Unknown scheme for proxy URL {url!r}")
+
+        if url.username or url.password:
+            headers.setdefault(
+                "Proxy-Authorization",
+                self._build_auth_header(url.username, url.password),
+            )
+            # Remove userinfo from the URL authority, e.g.:
+            # 'username:password@proxy_host:proxy_port' -> 'proxy_host:proxy_port'
+            url = url.copy_with(username=None, password=None)
+
+        self.url = url
+        self.headers = headers
+
+    def _build_auth_header(self, username: str, password: str) -> str:
+        userpass = (username.encode("utf-8"), password.encode("utf-8"))
+        token = b64encode(b":".join(userpass)).decode()
+        return f"Basic {token}"
+
+    def __repr__(self) -> str:
+        return f"Proxy(url={str(self.url)!r}, headers={dict(self.headers)!r})"
 
 
 DEFAULT_TIMEOUT_CONFIG = Timeout(timeout=5.0)
-DEFAULT_POOL_LIMITS = PoolLimits(soft_limit=10, hard_limit=100)
+DEFAULT_LIMITS = Limits(max_connections=100, max_keepalive_connections=20)
 DEFAULT_MAX_REDIRECTS = 20
```

### Comparing `httpx-0.9.5/httpx/decoders.py` & `httpx-1.0.0b0/httpx/_decoders.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,151 @@
 """
 Handlers for Content-Encoding.
 
 See: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Encoding
 """
 import codecs
+import io
 import typing
 import zlib
 
-import chardet
+from ._compat import brotli
+from ._exceptions import DecodingError
 
-from .exceptions import DecodingError
 
-try:
-    import brotli
-except ImportError:  # pragma: nocover
-    brotli = None
-
-
-class Decoder:
+class ContentDecoder:
     def decode(self, data: bytes) -> bytes:
         raise NotImplementedError()  # pragma: nocover
 
     def flush(self) -> bytes:
         raise NotImplementedError()  # pragma: nocover
 
 
-class IdentityDecoder(Decoder):
+class IdentityDecoder(ContentDecoder):
     """
     Handle unencoded data.
     """
 
     def decode(self, data: bytes) -> bytes:
         return data
 
     def flush(self) -> bytes:
         return b""
 
 
-class DeflateDecoder(Decoder):
+class DeflateDecoder(ContentDecoder):
     """
     Handle 'deflate' decoding.
 
     See: https://stackoverflow.com/questions/1838699
     """
 
     def __init__(self) -> None:
-        self.decompressor = zlib.decompressobj(-zlib.MAX_WBITS)
+        self.first_attempt = True
+        self.decompressor = zlib.decompressobj()
 
     def decode(self, data: bytes) -> bytes:
+        was_first_attempt = self.first_attempt
+        self.first_attempt = False
         try:
             return self.decompressor.decompress(data)
         except zlib.error as exc:
-            raise DecodingError from exc
+            if was_first_attempt:
+                self.decompressor = zlib.decompressobj(-zlib.MAX_WBITS)
+                return self.decode(data)
+            raise DecodingError(str(exc)) from exc
 
     def flush(self) -> bytes:
         try:
             return self.decompressor.flush()
         except zlib.error as exc:  # pragma: nocover
-            raise DecodingError from exc
+            raise DecodingError(str(exc)) from exc
 
 
-class GZipDecoder(Decoder):
+class GZipDecoder(ContentDecoder):
     """
     Handle 'gzip' decoding.
 
     See: https://stackoverflow.com/questions/1838699
     """
 
     def __init__(self) -> None:
         self.decompressor = zlib.decompressobj(zlib.MAX_WBITS | 16)
 
     def decode(self, data: bytes) -> bytes:
         try:
             return self.decompressor.decompress(data)
         except zlib.error as exc:
-            raise DecodingError from exc
+            raise DecodingError(str(exc)) from exc
 
     def flush(self) -> bytes:
         try:
             return self.decompressor.flush()
         except zlib.error as exc:  # pragma: nocover
-            raise DecodingError from exc
+            raise DecodingError(str(exc)) from exc
 
 
-class BrotliDecoder(Decoder):
+class BrotliDecoder(ContentDecoder):
     """
     Handle 'brotli' decoding.
 
     Requires `pip install brotlipy`. See: https://brotlipy.readthedocs.io/
         or   `pip install brotli`. See https://github.com/google/brotli
     Supports both 'brotlipy' and 'Brotli' packages since they share an import
     name. The top branches are for 'brotlipy' and bottom branches for 'Brotli'
     """
 
     def __init__(self) -> None:
-        assert (
-            brotli is not None
-        ), "The 'brotlipy' or 'brotli' library must be installed to use 'BrotliDecoder'"
+        if brotli is None:  # pragma: nocover
+            raise ImportError(
+                "Using 'BrotliDecoder', but neither of the 'brotlicffi' or 'brotli' "
+                "packages have been installed. "
+                "Make sure to install httpx using `pip install httpx[brotli]`."
+            ) from None
+
         self.decompressor = brotli.Decompressor()
         self.seen_data = False
+        if hasattr(self.decompressor, "decompress"):
+            # The 'brotlicffi' package.
+            self._decompress = self.decompressor.decompress  # pragma: nocover
+        else:
+            # The 'brotli' package.
+            self._decompress = self.decompressor.process  # pragma: nocover
 
     def decode(self, data: bytes) -> bytes:
         if not data:
             return b""
         self.seen_data = True
         try:
-            if hasattr(self.decompressor, "decompress"):
-                return self.decompressor.decompress(data)
-            return self.decompressor.process(data)  # pragma: nocover
+            return self._decompress(data)
         except brotli.error as exc:
-            raise DecodingError from exc
+            raise DecodingError(str(exc)) from exc
 
     def flush(self) -> bytes:
         if not self.seen_data:
             return b""
         try:
             if hasattr(self.decompressor, "finish"):
-                self.decompressor.finish()
+                # Only available in the 'brotlicffi' package.
+
+                # As the decompressor decompresses eagerly, this
+                # will never actually emit any data. However, it will potentially throw
+                # errors if a truncated or damaged data stream has been used.
+                self.decompressor.finish()  # pragma: nocover
             return b""
         except brotli.error as exc:  # pragma: nocover
-            raise DecodingError from exc
+            raise DecodingError(str(exc)) from exc
 
 
-class MultiDecoder(Decoder):
+class MultiDecoder(ContentDecoder):
     """
     Handle the case where multiple encodings have been applied.
     """
 
-    def __init__(self, children: typing.Sequence[Decoder]) -> None:
+    def __init__(self, children: typing.Sequence[ContentDecoder]) -> None:
         """
         'children' should be a sequence of decoders in the order in which
         each was applied.
         """
         # Note that we reverse the order for decoding.
         self.children = list(reversed(children))
 
@@ -143,76 +157,105 @@
     def flush(self) -> bytes:
         data = b""
         for child in self.children:
             data = child.decode(data) + child.flush()
         return data
 
 
+class ByteChunker:
+    """
+    Handles returning byte content in fixed-size chunks.
+    """
+
+    def __init__(self, chunk_size: int = None) -> None:
+        self._buffer = io.BytesIO()
+        self._chunk_size = chunk_size
+
+    def decode(self, content: bytes) -> typing.List[bytes]:
+        if self._chunk_size is None:
+            return [content]
+
+        self._buffer.write(content)
+        if self._buffer.tell() >= self._chunk_size:
+            value = self._buffer.getvalue()
+            chunks = [
+                value[i : i + self._chunk_size]
+                for i in range(0, len(value), self._chunk_size)
+            ]
+            if len(chunks[-1]) == self._chunk_size:
+                self._buffer.seek(0)
+                self._buffer.truncate()
+                return chunks
+            else:
+                self._buffer.seek(0)
+                self._buffer.write(chunks[-1])
+                self._buffer.truncate()
+                return chunks[:-1]
+        else:
+            return []
+
+    def flush(self) -> typing.List[bytes]:
+        value = self._buffer.getvalue()
+        self._buffer.seek(0)
+        self._buffer.truncate()
+        return [value] if value else []
+
+
+class TextChunker:
+    """
+    Handles returning text content in fixed-size chunks.
+    """
+
+    def __init__(self, chunk_size: int = None) -> None:
+        self._buffer = io.StringIO()
+        self._chunk_size = chunk_size
+
+    def decode(self, content: str) -> typing.List[str]:
+        if self._chunk_size is None:
+            return [content]
+
+        self._buffer.write(content)
+        if self._buffer.tell() >= self._chunk_size:
+            value = self._buffer.getvalue()
+            chunks = [
+                value[i : i + self._chunk_size]
+                for i in range(0, len(value), self._chunk_size)
+            ]
+            if len(chunks[-1]) == self._chunk_size:
+                self._buffer.seek(0)
+                self._buffer.truncate()
+                return chunks
+            else:
+                self._buffer.seek(0)
+                self._buffer.write(chunks[-1])
+                self._buffer.truncate()
+                return chunks[:-1]
+        else:
+            return []
+
+    def flush(self) -> typing.List[str]:
+        value = self._buffer.getvalue()
+        self._buffer.seek(0)
+        self._buffer.truncate()
+        return [value] if value else []
+
+
 class TextDecoder:
     """
     Handles incrementally decoding bytes into text
     """
 
-    def __init__(self, encoding: typing.Optional[str] = None):
-        self.decoder: typing.Optional[codecs.IncrementalDecoder] = (
-            None if encoding is None else codecs.getincrementaldecoder(encoding)()
-        )
-        self.detector = chardet.universaldetector.UniversalDetector()
-
-        # This buffer is only needed if 'decoder' is 'None'
-        # we want to trigger errors if data is getting added to
-        # our internal buffer for some silly reason while
-        # a decoder is discovered.
-        self.buffer: typing.Optional[bytearray] = None if self.decoder else bytearray()
+    def __init__(self, encoding: str = "utf-8"):
+        self.decoder = codecs.getincrementaldecoder(encoding)(errors="replace")
 
     def decode(self, data: bytes) -> str:
-        try:
-            if self.decoder is not None:
-                text = self.decoder.decode(data)
-            else:
-                assert self.buffer is not None
-                text = ""
-                self.detector.feed(data)
-                self.buffer += data
-
-                # Should be more than enough data to process, we don't
-                # want to buffer too long as chardet will wait until
-                # detector.close() is used to give back common
-                # encodings like 'utf-8'.
-                if len(self.buffer) >= 4096:
-                    self.decoder = codecs.getincrementaldecoder(
-                        self._detector_result()
-                    )()
-                    text = self.decoder.decode(bytes(self.buffer), False)
-                    self.buffer = None
-
-            return text
-        except UnicodeDecodeError:  # pragma: nocover
-            raise DecodingError() from None
+        return self.decoder.decode(data)
 
     def flush(self) -> str:
-        try:
-            if self.decoder is None:
-                # Empty string case as chardet is guaranteed to not have a guess.
-                assert self.buffer is not None
-                if len(self.buffer) == 0:
-                    return ""
-                return bytes(self.buffer).decode(self._detector_result())
-
-            return self.decoder.decode(b"", True)
-        except UnicodeDecodeError:  # pragma: nocover
-            raise DecodingError() from None
-
-    def _detector_result(self) -> str:
-        self.detector.close()
-        result = self.detector.result["encoding"]
-        if not result:  # pragma: nocover
-            raise DecodingError("Unable to determine encoding of content")
-
-        return result
+        return self.decoder.decode(b"", True)
 
 
 class LineDecoder:
     """
     Handles incrementally reading lines from text.
 
     Uses universal line decoding, supporting any of `\n`, `\r`, or `\r\n`
@@ -221,20 +264,26 @@
 
     def __init__(self) -> None:
         self.buffer = ""
 
     def decode(self, text: str) -> typing.List[str]:
         lines = []
 
-        if text.startswith("\n") and self.buffer and self.buffer[-1] == "\r":
-            # Handle the case where we have an "\r\n" split across
-            # our previous input, and our new chunk.
-            lines.append(self.buffer[:-1] + "\n")
-            self.buffer = ""
-            text = text[1:]
+        if text and self.buffer and self.buffer[-1] == "\r":
+            if text.startswith("\n"):
+                # Handle the case where we have an "\r\n" split across
+                # our previous input, and our new chunk.
+                lines.append(self.buffer[:-1] + "\n")
+                self.buffer = ""
+                text = text[1:]
+            else:
+                # Handle the case where we have "\r" at the end of our
+                # previous input.
+                lines.append(self.buffer[:-1] + "\n")
+                self.buffer = ""
 
         while text:
             num_chars = len(text)
             for idx in range(num_chars):
                 char = text[idx]
                 next_char = None if idx + 1 == num_chars else text[idx + 1]
                 if char == "\n":
@@ -249,15 +298,15 @@
                     break
                 elif char == "\r" and next_char is not None:
                     lines.append(self.buffer + text[:idx] + "\n")
                     self.buffer = ""
                     text = text[idx + 1 :]
                     break
                 elif next_char is None:
-                    self.buffer = text
+                    self.buffer += text
                     text = ""
                     break
 
         return lines
 
     def flush(self) -> typing.List[str]:
         if self.buffer.endswith("\r"):
@@ -278,12 +327,7 @@
     "deflate": DeflateDecoder,
     "br": BrotliDecoder,
 }
 
 
 if brotli is None:
     SUPPORTED_DECODERS.pop("br")  # pragma: nocover
-
-
-ACCEPT_ENCODING = ", ".join(
-    [key for key in SUPPORTED_DECODERS.keys() if key != "identity"]
-)
```

### Comparing `httpx-0.9.5/httpx/dispatch/asgi.py` & `httpx-1.0.0b0/httpx/_transports/asgi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,62 @@
 import typing
 
-from ..config import CertTypes, TimeoutTypes, VerifyTypes
-from ..models import Request, Response
-from .base import Dispatcher
+import sniffio
 
+from .._models import Request, Response
+from .._types import AsyncByteStream
+from .base import AsyncBaseTransport
 
-class ASGIDispatch(Dispatcher):
-    """
-    A custom dispatcher that handles sending requests directly to an ASGI app.
+if typing.TYPE_CHECKING:  # pragma: no cover
+    import asyncio
+
+    import trio
+
+    Event = typing.Union[asyncio.Event, trio.Event]
+
+
+def create_event() -> "Event":
+    if sniffio.current_async_library() == "trio":
+        import trio
+
+        return trio.Event()
+    else:
+        import asyncio
+
+        return asyncio.Event()
+
+
+class ASGIResponseStream(AsyncByteStream):
+    def __init__(self, body: typing.List[bytes]) -> None:
+        self._body = body
 
+    async def __aiter__(self) -> typing.AsyncIterator[bytes]:
+        yield b"".join(self._body)
+
+
+class ASGITransport(AsyncBaseTransport):
+    """
+    A custom AsyncTransport that handles sending requests directly to an ASGI app.
     The simplest way to use this functionality is to use the `app` argument.
-    This will automatically infer if 'app' is a WSGI or an ASGI application,
-    and will setup an appropriate dispatch class:
 
     ```
-    client = httpx.Client(app=app)
+    client = httpx.AsyncClient(app=app)
     ```
 
-    Alternatively, you can setup the dispatch instance explicitly.
+    Alternatively, you can setup the transport instance explicitly.
     This allows you to include any additional configuration arguments specific
-    to the ASGIDispatch class:
+    to the ASGITransport class:
 
     ```
-    dispatch = httpx.ASGIDispatch(
+    transport = httpx.ASGITransport(
         app=app,
         root_path="/submount",
         client=("1.2.3.4", 123)
     )
-    client = httpx.Client(dispatch=dispatch)
+    client = httpx.AsyncClient(transport=transport)
     ```
 
     Arguments:
 
     * `app` - The ASGI application.
     * `raise_app_exceptions` - Boolean indicating if exceptions in the application
        should be raised. Default to `True`. Can be set to `False` for use cases
@@ -49,81 +74,90 @@
         client: typing.Tuple[str, int] = ("127.0.0.1", 123),
     ) -> None:
         self.app = app
         self.raise_app_exceptions = raise_app_exceptions
         self.root_path = root_path
         self.client = client
 
-    async def send(
+    async def handle_async_request(
         self,
         request: Request,
-        verify: VerifyTypes = None,
-        cert: CertTypes = None,
-        timeout: TimeoutTypes = None,
     ) -> Response:
+        assert isinstance(request.stream, AsyncByteStream)
 
+        # ASGI scope.
         scope = {
             "type": "http",
             "asgi": {"version": "3.0"},
             "http_version": "1.1",
             "method": request.method,
-            "headers": request.headers.raw,
+            "headers": [(k.lower(), v) for (k, v) in request.headers.raw],
             "scheme": request.url.scheme,
             "path": request.url.path,
-            "query_string": request.url.query.encode("ascii"),
-            "server": request.url.host,
+            "raw_path": request.url.raw_path,
+            "query_string": request.url.query,
+            "server": (request.url.host, request.url.port),
             "client": self.client,
             "root_path": self.root_path,
         }
+
+        # Request.
+        request_body_chunks = request.stream.__aiter__()
+        request_complete = False
+
+        # Response.
         status_code = None
-        headers = None
+        response_headers = None
         body_parts = []
-        request_stream = request.stream()
         response_started = False
-        response_complete = False
+        response_complete = create_event()
+
+        # ASGI callables.
 
         async def receive() -> dict:
+            nonlocal request_complete
+
+            if request_complete:
+                await response_complete.wait()
+                return {"type": "http.disconnect"}
+
             try:
-                body = await request_stream.__anext__()
+                body = await request_body_chunks.__anext__()
             except StopAsyncIteration:
+                request_complete = True
                 return {"type": "http.request", "body": b"", "more_body": False}
             return {"type": "http.request", "body": body, "more_body": True}
 
         async def send(message: dict) -> None:
-            nonlocal status_code, headers, body_parts
-            nonlocal response_started, response_complete
+            nonlocal status_code, response_headers, response_started
 
             if message["type"] == "http.response.start":
                 assert not response_started
 
                 status_code = message["status"]
-                headers = message.get("headers", [])
+                response_headers = message.get("headers", [])
                 response_started = True
 
             elif message["type"] == "http.response.body":
-                assert not response_complete
+                assert not response_complete.is_set()
                 body = message.get("body", b"")
                 more_body = message.get("more_body", False)
 
                 if body and request.method != "HEAD":
                     body_parts.append(body)
 
                 if not more_body:
-                    response_complete = True
+                    response_complete.set()
 
         try:
             await self.app(scope, receive, send)
         except Exception:
-            if self.raise_app_exceptions or not response_complete:
+            if self.raise_app_exceptions or not response_complete.is_set():
                 raise
 
-        assert response_complete
+        assert response_complete.is_set()
         assert status_code is not None
-        assert headers is not None
+        assert response_headers is not None
+
+        stream = ASGIResponseStream(body_parts)
 
-        return Response(
-            status_code=status_code,
-            http_version="HTTP/1.1",
-            headers=headers,
-            content=b"".join(body_parts),
-            request=request,
-        )
+        return Response(status_code, headers=response_headers, stream=stream)
```

### Comparing `httpx-0.9.5/httpx/status_codes.py` & `httpx-1.0.0b0/httpx/_status_codes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,94 @@
 from enum import IntEnum
 
 
-class StatusCode(IntEnum):
+class codes(IntEnum):
     """HTTP status codes and reason phrases
+
     Status codes from the following RFCs are all observed:
+
         * RFC 7231: Hypertext Transfer Protocol (HTTP/1.1), obsoletes 2616
         * RFC 6585: Additional HTTP Status Codes
         * RFC 3229: Delta encoding in HTTP
         * RFC 4918: HTTP Extensions for WebDAV, obsoletes 2518
         * RFC 5842: Binding Extensions to WebDAV
         * RFC 7238: Permanent Redirect
         * RFC 2295: Transparent Content Negotiation in HTTP
         * RFC 2774: An HTTP Extension Framework
         * RFC 7540: Hypertext Transfer Protocol Version 2 (HTTP/2)
         * RFC 2324: Hyper Text Coffee Pot Control Protocol (HTCPCP/1.0)
         * RFC 7725: An HTTP Status Code to Report Legal Obstacles
+        * RFC 8297: An HTTP Status Code for Indicating Hints
+        * RFC 8470: Using Early Data in HTTP
     """
 
-    def __new__(cls, value: int, phrase: str = "") -> "StatusCode":
+    def __new__(cls, value: int, phrase: str = "") -> "codes":
         obj = int.__new__(cls, value)  # type: ignore
         obj._value_ = value
 
-        obj.phrase = phrase
+        obj.phrase = phrase  # type: ignore
         return obj
 
     def __str__(self) -> str:
         return str(self.value)
 
     @classmethod
     def get_reason_phrase(cls, value: int) -> str:
         try:
-            return StatusCode(value).phrase  # type: ignore
+            return codes(value).phrase  # type: ignore
         except ValueError:
             return ""
 
     @classmethod
-    def is_redirect(cls, value: int) -> bool:
-        return value in (
-            # 301 (Cacheable redirect. Method may change to GET.)
-            StatusCode.MOVED_PERMANENTLY,
-            # 302 (Uncacheable redirect. Method may change to GET.)
-            StatusCode.FOUND,
-            # 303 (Client should make a GET or HEAD request.)
-            StatusCode.SEE_OTHER,
-            # 307 (Equiv. 302, but retain method)
-            StatusCode.TEMPORARY_REDIRECT,
-            # 308 (Equiv. 301, but retain method)
-            StatusCode.PERMANENT_REDIRECT,
-        )
+    def is_informational(cls, value: int) -> bool:
+        """
+        Returns `True` for 1xx status codes, `False` otherwise.
+        """
+        return 100 <= value <= 199
 
     @classmethod
-    def is_error(cls, value: int) -> bool:
-        return 400 <= value <= 599
+    def is_success(cls, value: int) -> bool:
+        """
+        Returns `True` for 2xx status codes, `False` otherwise.
+        """
+        return 200 <= value <= 299
+
+    @classmethod
+    def is_redirect(cls, value: int) -> bool:
+        """
+        Returns `True` for 3xx status codes, `False` otherwise.
+        """
+        return 300 <= value <= 399
 
     @classmethod
     def is_client_error(cls, value: int) -> bool:
+        """
+        Returns `True` for 4xx status codes, `False` otherwise.
+        """
         return 400 <= value <= 499
 
     @classmethod
     def is_server_error(cls, value: int) -> bool:
+        """
+        Returns `True` for 5xx status codes, `False` otherwise.
+        """
         return 500 <= value <= 599
 
+    @classmethod
+    def is_error(cls, value: int) -> bool:
+        """
+        Returns `True` for 4xx or 5xx status codes, `False` otherwise.
+        """
+        return 400 <= value <= 599
+
     # informational
     CONTINUE = 100, "Continue"
     SWITCHING_PROTOCOLS = 101, "Switching Protocols"
     PROCESSING = 102, "Processing"
+    EARLY_HINTS = 103, "Early Hints"
 
     # success
     OK = 200, "OK"
     CREATED = 201, "Created"
     ACCEPTED = 202, "Accepted"
     NON_AUTHORITATIVE_INFORMATION = 203, "Non-Authoritative Information"
     NO_CONTENT = 204, "No Content"
@@ -108,14 +128,15 @@
     REQUESTED_RANGE_NOT_SATISFIABLE = 416, "Requested Range Not Satisfiable"
     EXPECTATION_FAILED = 417, "Expectation Failed"
     IM_A_TEAPOT = 418, "I'm a teapot"
     MISDIRECTED_REQUEST = 421, "Misdirected Request"
     UNPROCESSABLE_ENTITY = 422, "Unprocessable Entity"
     LOCKED = 423, "Locked"
     FAILED_DEPENDENCY = 424, "Failed Dependency"
+    TOO_EARLY = 425, "Too Early"
     UPGRADE_REQUIRED = 426, "Upgrade Required"
     PRECONDITION_REQUIRED = 428, "Precondition Required"
     TOO_MANY_REQUESTS = 429, "Too Many Requests"
     REQUEST_HEADER_FIELDS_TOO_LARGE = 431, "Request Header Fields Too Large"
     UNAVAILABLE_FOR_LEGAL_REASONS = 451, "Unavailable For Legal Reasons"
 
     # server errors
@@ -128,12 +149,10 @@
     VARIANT_ALSO_NEGOTIATES = 506, "Variant Also Negotiates"
     INSUFFICIENT_STORAGE = 507, "Insufficient Storage"
     LOOP_DETECTED = 508, "Loop Detected"
     NOT_EXTENDED = 510, "Not Extended"
     NETWORK_AUTHENTICATION_REQUIRED = 511, "Network Authentication Required"
 
 
-codes = StatusCode
-
-#  Include lower-case styles for `requests` compatibility.
+# Include lower-case styles for `requests` compatibility.
 for code in codes:
     setattr(codes, code._name_.lower(), int(code))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `httpx-0.9.5/httpx.egg-info/SOURCES.txt` & `httpx-1.0.0b0/httpx.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -2,38 +2,35 @@
 LICENSE.md
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 httpx/__init__.py
 httpx/__version__.py
-httpx/api.py
-httpx/auth.py
-httpx/client.py
-httpx/config.py
-httpx/content.py
-httpx/decoders.py
-httpx/exceptions.py
-httpx/models.py
-httpx/multipart.py
+httpx/_api.py
+httpx/_auth.py
+httpx/_client.py
+httpx/_compat.py
+httpx/_config.py
+httpx/_content.py
+httpx/_decoders.py
+httpx/_exceptions.py
+httpx/_main.py
+httpx/_models.py
+httpx/_multipart.py
+httpx/_status_codes.py
+httpx/_types.py
+httpx/_utils.py
 httpx/py.typed
-httpx/status_codes.py
-httpx/utils.py
 httpx.egg-info/PKG-INFO
 httpx.egg-info/SOURCES.txt
 httpx.egg-info/dependency_links.txt
+httpx.egg-info/entry_points.txt
 httpx.egg-info/not-zip-safe
 httpx.egg-info/requires.txt
 httpx.egg-info/top_level.txt
-httpx/concurrency/__init__.py
-httpx/concurrency/asyncio.py
-httpx/concurrency/auto.py
-httpx/concurrency/base.py
-httpx/concurrency/trio.py
-httpx/dispatch/__init__.py
-httpx/dispatch/asgi.py
-httpx/dispatch/base.py
-httpx/dispatch/connection.py
-httpx/dispatch/connection_pool.py
-httpx/dispatch/http11.py
-httpx/dispatch/http2.py
-httpx/dispatch/proxy_http.py
+httpx/_transports/__init__.py
+httpx/_transports/asgi.py
+httpx/_transports/base.py
+httpx/_transports/default.py
+httpx/_transports/mock.py
+httpx/_transports/wsgi.py
```

### Comparing `httpx-0.9.5/setup.py` & `httpx-1.0.0b0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,42 +36,63 @@
 
 
 setup(
     name="httpx",
     python_requires=">=3.6",
     version=get_version("httpx"),
     url="https://github.com/encode/httpx",
+    project_urls={
+        "Changelog": "https://github.com/encode/httpx/blob/master/CHANGELOG.md",
+        "Documentation": "https://www.python-httpx.org",
+        "Source": "https://github.com/encode/httpx",
+    },
     license="BSD",
     description="The next generation HTTP client.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Tom Christie",
     author_email="tom@tomchristie.com",
     package_data={"httpx": ["py.typed"]},
     packages=get_packages("httpx"),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         "certifi",
-        "hstspreload",
-        "chardet==3.*",
-        "h11==0.8.*",
-        "h2==3.*",
-        "idna==2.*",
-        "rfc3986>=1.3,<2",
-        "sniffio==1.*",
+        "charset_normalizer",
+        "sniffio",
+        "rfc3986[idna2008]>=1.3,<2",
+        "httpcore>=0.13.3,<0.14.0",
+        "async_generator; python_version < '3.7'"
     ],
+    extras_require={
+        "http2": "h2>=3,<5",
+        "brotli": [
+            "brotli; platform_python_implementation == 'CPython'",
+            "brotlicffi; platform_python_implementation != 'CPython'"
+        ],
+        "cli": [
+            "click==8.*",
+            "rich==10.*",
+            "pygments==2.*"
+        ]
+    },
+    entry_points = {
+        "console_scripts": "httpx=httpx:main"
+    },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Topic :: Internet :: WWW/HTTP",
         "Framework :: AsyncIO",
         "Framework :: Trio",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3 :: Only",
     ],
 )
```

