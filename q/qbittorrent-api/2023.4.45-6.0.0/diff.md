# Comparing `tmp/qbittorrent-api-2023.4.45.tar.gz` & `tmp/qbittorrent-api-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbittorrent-api-2023.4.45.tar", last modified: Tue Apr 11 19:12:20 2023, max compression
+gzip compressed data, was "dist/qbittorrent-api-6.0.0.tar", last modified: Thu Apr 23 04:02:29 2020, max compression
```

## Comparing `qbittorrent-api-2023.4.45.tar` & `qbittorrent-api-6.0.0.tar`

### file list

```diff
@@ -1,64 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:12:20.185085 qbittorrent-api-2023.4.45/
--rw-r--r--   0 runner    (1001) docker     (123)    10435 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-04-11 19:12:20.185085 qbittorrent-api-2023.4.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-11 19:12:20.185085 qbittorrent-api-2023.4.45/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:12:20.165085 qbittorrent-api-2023.4.45/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:12:20.169085 qbittorrent-api-2023.4.45/src/qbittorrent_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-04-11 19:12:20.000000 qbittorrent-api-2023.4.45/src/qbittorrent_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-11 19:12:20.000000 qbittorrent-api-2023.4.45/src/qbittorrent_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:12:20.000000 qbittorrent-api-2023.4.45/src/qbittorrent_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:12:19.000000 qbittorrent-api-2023.4.45/src/qbittorrent_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-11 19:12:20.000000 qbittorrent-api-2023.4.45/src/qbittorrent_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 19:12:20.000000 qbittorrent-api-2023.4.45/src/qbittorrent_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:12:20.181085 qbittorrent-api-2023.4.45/src/qbittorrentapi/
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16447 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/_attrdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/_attrdict.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/_types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/_version_support.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/_version_support.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/app.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6611 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/definitions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/log.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34702 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/request.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12490 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/rss.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13223 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/sync.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    87028 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)    32537 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/torrents.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/src/qbittorrentapi/transfer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:12:20.185085 qbittorrent-api-2023.4.45/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)    24503 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_rss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    17932 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_torrent.py
--rw-r--r--   0 runner    (1001) docker     (123)    46941 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_torrents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 19:12:10.000000 qbittorrent-api-2023.4.45/tests/test_zzz_last_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (116)     2016 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    35149 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      145 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    23199 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    17763 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    23199 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      696 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2020-04-23 04:02:29.000000 qbittorrent-api-6.0.0/qbittorrent_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/qbittorrentapi/
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3655 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/app.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2408 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10851 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7416 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2930 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1786 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26761 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1771 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/log.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11711 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/request.py
+-rw-r--r--   0 runner    (1001) docker     (116)    13759 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/responses.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5813 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/rss.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6711 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/search.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1801 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/sync.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30791 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/torrents.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4224 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/qbittorrentapi/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-04-23 04:02:29.175511 qbittorrent-api-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1525 2020-04-23 04:02:22.000000 qbittorrent-api-6.0.0/setup.py
```

### Comparing `qbittorrent-api-2023.4.45/src/qbittorrentapi/exceptions.py` & `qbittorrent-api-6.0.0/qbittorrentapi/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,142 +1,156 @@
-from requests.exceptions import HTTPError as RequestsHTTPError
 from requests.exceptions import RequestException
 
 
 class APIError(Exception):
-    """Base error for all exceptions from this Client."""
-
-
-class UnsupportedQbittorrentVersion(APIError):
-    """Connected qBittorrent is not fully supported by this Client."""
+    """
+    Base error for all exceptions from this Client.
+    """
+    pass
 
 
 class FileError(IOError, APIError):
-    """Base class for all exceptions for file handling."""
+    """
+    Base class for all exceptions for file handling.
+    """
+    pass
 
 
 class TorrentFileError(FileError):
-    """Base class for all exceptions for torrent files."""
+    """
+    Base class for all exceptions for torrent files.
+    """
+    pass
 
 
 class TorrentFileNotFoundError(TorrentFileError):
-    """Specified torrent file does not appear to exist."""
+    """
+    Specified torrent file does not appear to exist.
+    """
+    pass
 
 
 class TorrentFilePermissionError(TorrentFileError):
-    """Permission was denied to read the specified torrent file."""
+    """
+    Permission was denied to read the specified torrent file.
+    """
+    pass
 
 
 class APIConnectionError(RequestException, APIError):
-    """Base class for all communications errors including HTTP errors."""
+    """
+    Base class for all communications errors including HTTP errors.
+    """
+    pass
 
 
 class LoginFailed(APIConnectionError):
-    """This can technically be raised with any request since log in may be
-    attempted for any request and could fail."""
+    """
+    This can technically be raised with any request since log in may be attempted for any request and could fail.
+    """
+    pass
 
 
-class HTTPError(RequestsHTTPError, APIConnectionError):
+class HTTPError(APIConnectionError):
     """
-    Base error for all HTTP errors.
-
-    All errors following a successful connection to qBittorrent are
-    returned as HTTP statuses.
+    Base error for all HTTP errors. All errors following a successful connection to qBittorrent are returned as HTTP statuses.
     """
-
-    http_status_code = None
+    pass
 
 
 class HTTP4XXError(HTTPError):
-    """Base error for all HTTP 4XX statuses."""
+    """
+    Base error for all HTTP 4XX statuses.
+    """
+    pass
 
 
 class HTTP5XXError(HTTPError):
-    """Base error for all HTTP 5XX statuses."""
+    """
+    Base error for all HTTP 5XX statuses.
+    """
+    pass
 
 
 class HTTP400Error(HTTP4XXError):
-    """HTTP 400 Status."""
-
-    http_status_code = 400
+    pass
 
 
 class HTTP401Error(HTTP4XXError):
-    """HTTP 401 Status."""
-
-    http_status_code = 401
+    pass
 
 
 class HTTP403Error(HTTP4XXError):
-    """HTTP 403 Status."""
-
-    http_status_code = 403
+    pass
 
 
 class HTTP404Error(HTTP4XXError):
-    """HTTP 404 Status."""
-
-    http_status_code = 404
-
-
-class HTTP405Error(HTTP4XXError):
-    """HTTP 405 Status."""
-
-    http_status_code = 405
+    pass
 
 
 class HTTP409Error(HTTP4XXError):
-    """HTTP 409 Status."""
-
-    http_status_code = 409
+    pass
 
 
 class HTTP415Error(HTTP4XXError):
-    """HTTP 415 Status."""
-
-    http_status_code = 415
+    pass
 
 
 class HTTP500Error(HTTP5XXError):
-    """HTTP 500 Status."""
-
-    http_status_code = 500
+    pass
 
 
 class MissingRequiredParameters400Error(HTTP400Error):
-    """Endpoint call is missing one or more required parameters."""
+    """
+    Endpoint call is missing one or more required parameters.
+    """
+    pass
 
 
 class InvalidRequest400Error(HTTP400Error):
-    """One or more endpoint arguments are malformed."""
+    """
+    One or more endpoint arguments are malformed.
+    """
+    pass
 
 
 class Unauthorized401Error(HTTP401Error):
-    """Primarily reserved for XSS and host header issues."""
+    """
+    Primarily reserved for XSS and host header issues.
+    """
+    pass
 
 
 class Forbidden403Error(HTTP403Error):
-    """Not logged in, IP has been banned, or calling an API method that isn't
-    public."""
+    """
+    Not logged in, IP has been banned, or calling an API method that isn't public.
+    """
+    pass
 
 
 class NotFound404Error(HTTP404Error):
-    """This should mean qBittorrent couldn't find a torrent for the torrent
-    hash."""
-
-
-class MethodNotAllowed405Error(HTTP405Error):
-    """HTTP method is not supported for the API endpoint."""
+    """
+    This should mean qBittorrent couldn't find a torrent for the torrent hash.
+    It is also possible this means the endpoint doesn't exist in qBittorrent...but that also means this Client has a bug.
+    """
+    pass
 
 
 class Conflict409Error(HTTP409Error):
-    """Returned if arguments don't make sense specific to the endpoint."""
+    """
+    Returned if arguments don't make sense specific to the endpoint.
+    """
+    pass
 
 
 class UnsupportedMediaType415Error(HTTP415Error):
-    """``torrents/add`` endpoint will return this for invalid URL(s) or
-    files."""
+    """
+    torrents/add endpoint will return this for invalid URL(s) or files.
+    """
+    pass
 
 
 class InternalServerError500Error(HTTP500Error):
-    """Returned if qBittorrent errors internally while processing the
-    request."""
+    """
+    Returned if qBittorent craps on itself while processing the request...
+    """
+    pass
```

