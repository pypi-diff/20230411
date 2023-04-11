# Comparing `tmp/bitbucket_python-0.3.0.tar.gz` & `tmp/bitbucket_python-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbucket_python-0.3.0.tar", max compression
+gzip compressed data, was "bitbucket_python-0.3.1.tar", max compression
```

## Comparing `bitbucket_python-0.3.0.tar` & `bitbucket_python-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-03-27 21:06:04.140442 bitbucket_python-0.3.0/LICENSE
--rw-r--r--   0        0        0     2361 2023-04-01 19:06:34.079217 bitbucket_python-0.3.0/README.md
--rw-r--r--   0        0        0      117 2023-04-01 19:06:34.079408 bitbucket_python-0.3.0/bitbucket/__init__.py
--rw-r--r--   0        0        0    18076 2023-04-01 19:06:34.079592 bitbucket_python-0.3.0/bitbucket/aclient.py
--rw-r--r--   0        0        0     1096 2023-04-01 19:06:34.079743 bitbucket_python-0.3.0/bitbucket/base.py
--rw-r--r--   0        0        0    10719 2023-04-01 19:06:34.079945 bitbucket_python-0.3.0/bitbucket/client.py
--rw-r--r--   0        0        0      264 2023-03-27 21:06:04.140882 bitbucket_python-0.3.0/bitbucket/exceptions.py
--rw-r--r--   0        0        0      418 2023-04-01 19:06:34.081518 bitbucket_python-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3052 1970-01-01 00:00:00.000000 bitbucket_python-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-27 21:06:04.140442 bitbucket_python-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2762 2023-04-11 01:04:01.443767 bitbucket_python-0.3.1/README.md
+-rw-r--r--   0        0        0      117 2023-04-01 19:06:34.079408 bitbucket_python-0.3.1/bitbucket/__init__.py
+-rw-r--r--   0        0        0    19438 2023-04-11 01:04:01.443970 bitbucket_python-0.3.1/bitbucket/aclient.py
+-rw-r--r--   0        0        0     2265 2023-04-11 01:04:01.444132 bitbucket_python-0.3.1/bitbucket/base.py
+-rw-r--r--   0        0        0    12863 2023-04-11 01:04:01.444295 bitbucket_python-0.3.1/bitbucket/client.py
+-rw-r--r--   0        0        0      264 2023-03-27 21:06:04.140882 bitbucket_python-0.3.1/bitbucket/exceptions.py
+-rw-r--r--   0        0        0      501 2023-04-11 01:04:01.444667 bitbucket_python-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 bitbucket_python-0.3.1/PKG-INFO
```

### Comparing `bitbucket_python-0.3.0/LICENSE` & `bitbucket_python-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbucket_python-0.3.0/README.md` & `bitbucket_python-0.3.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 ## Installing
 ```
 pip install bitbucket-python
 ```
 
 ## Usage
 
-### Sync client
-
 ```python
 from bitbucket.client import Client
 from bitbucket import AsyncClient
 
 client = Client('EMAIL', 'PASSWORD')
 
 # Or to specify owner URL to find repo own by other user
@@ -20,14 +18,16 @@
 
 # Async client
 async with AsyncClient('EMAIL', 'PASSWORD') as client:
     ...
 
 ```
 
+### Methods
+
 Get user information
 ```
 response = client.get_user()
 ```
 
 Get account privileges for repositories
 ```
@@ -128,11 +128,26 @@
 ```
 
 Delete webhook
 ```
 response = client.delete_webhook('REPOSITORY_SLUG', 'WEBHOOK_ID')
 ```
 
+### Helper methods
+
+### all_pages
+
+The `all_pages` method is a helper function that makes it easy to retrieve all items from an API methods that uses pagination (see https://developer.atlassian.com/cloud/bitbucket/rest/intro/#pagination).
+
+```python
+client = Client()
+
+items = list(client.all_pages(client.get_repositories))
+```
+
+Note that the `all_pages` method uses a generator to return the results.
+
+
 ## Requirements
 
 - requests
 - [httpx](https://github.com/encode/httpx/)
```

### Comparing `bitbucket_python-0.3.0/bitbucket/aclient.py` & `bitbucket_python-0.3.1/bitbucket/aclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import typing
 import httpx
 
 from .base import BaseClient
 
 
 class Client(BaseClient):
     """
@@ -17,19 +18,14 @@
     ```
     async with Client('myusername', 'mypassword', 'myaccount') as client:
         response = await client.get_user()
         print(response)
     ```
     """
 
-    def __init__(self, user, password, owner=None):
-        self.user = user
-        self.password = password
-        self.username = owner
-
     async def __aenter__(self):
         self._session = httpx.AsyncClient(
             auth=(
                 self.user,
                 self.password,
             )
         )
@@ -46,14 +42,60 @@
         self,
         exc_type,
         exc_value,
         traceback,
     ) -> None:
         await self._session.aclose()
 
+    async def all_pages(
+        self,
+        method: typing.Callable[
+            ...,
+            typing.Awaitable[typing.Union[typing.Dict[str, typing.Any], None]],
+        ],
+        *args,
+        **kwargs
+    ) -> typing.AsyncGenerator[typing.Dict[str, typing.Any], None]:
+        """
+        Retrieves all pages from a BitBucket API list endpoint and yields a generator for the items in the
+        response.
+
+        Example:
+
+        ```python
+        async for item in client.all_pages(
+                client.get_issues,
+                "{726f1aab-826f-4c08-a127-1224347b3d09}"
+        ):
+            print(item["id"])
+        ```
+
+        Args:
+            method: A client class method to retrieve all pages from.
+            *args: Variable length argument list to be passed to the `method` callable.
+            **kwargs: Arbitrary keyword arguments to be passed to the `method` callable.
+
+        Returns:
+            An asynchronous generator that yields a dictionary of item data for each item in the response.
+
+        Raises:
+            Any exceptions raised by the `method` callable.
+        """
+        resp = await method(*args, **kwargs)
+        while True:
+            if resp is None:
+                break
+
+            for v in resp["values"]:
+                yield v
+
+            if "next" not in resp:
+                break
+            resp = await self._get(resp["next"])
+
     async def get_user(self, params=None):
         """
         Retrieves information about the current user.
 
         Args:
             params (dict, optional): A dictionary of query parameters to include
                 in the request.
@@ -96,15 +138,15 @@
         )
 
     async def create_repository(self, params=None, data=None, name=None, team=None):
         """
         Creates a new repository.
 
         Example data:
-        ```
+        ```json
         {
             "scm": "git",
             "project": {
                 "key": "MARS"
             }
         }
         ```
@@ -404,15 +446,18 @@
         Args:
             endpoint (str): The endpoint to send the GET request to.
             params (dict, optional): A dictionary of query parameters to include in the request.
 
         Returns:
             A dictionary containing the parsed response from the GET request.
         """
-        response = await self._session.get(self.BASE_URL + endpoint, params=params)
+        response = await self._session.get(
+            endpoint if endpoint.startswith("http") else self.BASE_URL + endpoint,
+            params=params,
+        )
         return self.parse(response)
 
     async def _post(self, endpoint, params=None, data=None):
         """
         Sends a POST request to the specified endpoint with the specified data and returns the parsed response.
 
         Args:
```

