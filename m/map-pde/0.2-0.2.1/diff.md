# Comparing `tmp/map_pde-0.2.tar.gz` & `tmp/map_pde-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_pde-0.2.tar", last modified: Tue Apr 11 12:05:42 2023, max compression
+gzip compressed data, was "map_pde-0.2.1.tar", last modified: Tue Apr 11 13:17:37 2023, max compression
```

## Comparing `map_pde-0.2.tar` & `map_pde-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 12:05:42.834775 map_pde-0.2/
--rw-rw-rw-   0        0        0      279 2023-04-11 12:05:42.833778 map_pde-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-04-11 11:31:56.000000 map_pde-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 12:05:42.815770 map_pde-0.2/map_pde/
--rw-rw-rw-   0        0        0        0 2023-03-23 06:21:32.000000 map_pde-0.2/map_pde/__init__.py
--rw-rw-rw-   0        0        0    35309 2023-04-11 12:05:30.000000 map_pde-0.2/map_pde/client.py
--rw-rw-rw-   0        0        0     5774 2023-04-09 02:53:59.000000 map_pde-0.2/map_pde/constant.py
--rw-rw-rw-   0        0        0    14085 2023-04-09 02:50:43.000000 map_pde-0.2/map_pde/util.py
-drwxrwxrwx   0        0        0        0 2023-04-11 12:05:42.832776 map_pde-0.2/map_pde.egg-info/
--rw-rw-rw-   0        0        0      279 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 12:05:42.834775 map_pde-0.2/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-04-11 12:05:30.000000 map_pde-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:17:37.231676 map_pde-0.2.1/
+-rw-rw-rw-   0        0        0     1083 2023-03-23 06:20:49.000000 map_pde-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      263 2023-04-11 13:17:37.231676 map_pde-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-04-11 11:31:56.000000 map_pde-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 13:17:37.218670 map_pde-0.2.1/map_pde/
+-rw-rw-rw-   0        0        0        0 2023-03-23 06:21:32.000000 map_pde-0.2.1/map_pde/__init__.py
+-rw-rw-rw-   0        0        0    35342 2023-04-11 13:14:13.000000 map_pde-0.2.1/map_pde/client.py
+-rw-rw-rw-   0        0        0     5774 2023-04-09 02:53:59.000000 map_pde-0.2.1/map_pde/constant.py
+-rw-rw-rw-   0        0        0    14086 2023-04-11 13:16:57.000000 map_pde-0.2.1/map_pde/util.py
+drwxrwxrwx   0        0        0        0 2023-04-11 13:17:37.230676 map_pde-0.2.1/map_pde.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-04-11 13:17:37.000000 map_pde-0.2.1/map_pde.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-11 13:17:37.000000 map_pde-0.2.1/map_pde.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 13:17:37.000000 map_pde-0.2.1/map_pde.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 13:17:37.000000 map_pde-0.2.1/map_pde.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 13:17:37.000000 map_pde-0.2.1/map_pde.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       89 2023-04-11 13:17:37.236187 map_pde-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      384 2023-04-11 12:53:32.000000 map_pde-0.2.1/setup.py
```

### Comparing `map_pde-0.2/map_pde/client.py` & `map_pde-0.2.1/map_pde/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from obspy.clients.fdsn.header import (DEFAULT_USER_AGENT, FDSNWS,
                                        URL_MAPPING_SUBPATHS,
                                        WADL_PARAMETERS_NOT_TO_BE_PARSED,
                                        FDSNRedirectException,
                                        FDSNNoServiceException)
 from obspy.clients.fdsn.wadl_parser import WADLParser
 from socket import timeout as socket_timeout
-from map_pde.constant import *
-from map_pde.util import *
+from .constant import *
+from .util import *
 
 
 class CustomRedirectHandler(urllib_request.HTTPRedirectHandler):
     """
     Custom redirection handler to also do it for POST requests which the
     standard library does not do by default.
     """
@@ -823,15 +823,15 @@
             os.mkdir(dir)
         file_path = dir + "\\token"
         with open(file_path, "w") as f:
             f.write(self.sa_token)
 
 
 if __name__ == '__main__':
-    client = Client()
+    client = Client(sa_token="d72b9ced-88b9-45d8-8019-1430483a0dcb")
 
 
     # 通过Client获取波形数据
     st = client.get_map_waveforms([1], [1], [1, 2], startTime=UTCDateTime("2023-03-07 12:00:01"), endTime=UTCDateTime("2023-03-07 12:01:00"))
     print(st)
 
     # 对数据进行绘图
```

### Comparing `map_pde-0.2/map_pde/constant.py` & `map_pde-0.2.1/map_pde/constant.py`

 * *Files identical despite different names*

### Comparing `map_pde-0.2/map_pde/util.py` & `map_pde-0.2.1/map_pde/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
                                      FDSNBadGatewayException,
                                      FDSNTooManyRequestsException,
                                      FDSNRequestTooLargeException,
                                      FDSNServiceUnavailableException,
                                      FDSNUnauthorizedException,
                                      FDSNForbiddenException,
                                      FDSNInvalidRequestException)
-from constant import PARAMETER_ALIASES, DEFAULT_PARAMETERS
+from .constant import PARAMETER_ALIASES, DEFAULT_PARAMETERS
 from urllib.parse import urlencode
 from http.client import HTTPException, IncompleteRead
 from lxml import etree
 
 
 def convert_to_string(value):
     """
```

