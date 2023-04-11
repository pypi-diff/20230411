# Comparing `tmp/map_pde-0.1.tar.gz` & `tmp/map_pde-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "map_pde-0.1.tar", last modified: Tue Apr 11 11:50:49 2023, max compression
+gzip compressed data, was "map_pde-0.2.tar", last modified: Tue Apr 11 12:05:42 2023, max compression
```

## Comparing `map_pde-0.1.tar` & `map_pde-0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 11:50:49.137370 map_pde-0.1/
--rw-rw-rw-   0        0        0      279 2023-04-11 11:50:49.136371 map_pde-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       41 2023-04-11 11:31:56.000000 map_pde-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 11:50:49.129371 map_pde-0.1/map_pde.egg-info/
--rw-rw-rw-   0        0        0      279 2023-04-11 11:50:49.000000 map_pde-0.1/map_pde.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-11 11:50:49.000000 map_pde-0.1/map_pde.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 11:50:49.000000 map_pde-0.1/map_pde.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-11 11:50:49.000000 map_pde-0.1/map_pde.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-11 11:50:49.000000 map_pde-0.1/map_pde.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 11:50:49.137370 map_pde-0.1/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-04-11 11:50:45.000000 map_pde-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:50:49.131370 map_pde-0.1/src/
--rw-rw-rw-   0        0        0        0 2023-04-11 11:35:55.000000 map_pde-0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:50:49.135371 map_pde-0.1/src/pde/
--rw-rw-rw-   0        0        0        0 2023-03-23 06:21:32.000000 map_pde-0.1/src/pde/__init__.py
--rw-rw-rw-   0        0        0    35301 2023-04-11 11:36:22.000000 map_pde-0.1/src/pde/client.py
--rw-rw-rw-   0        0        0     5774 2023-04-09 02:53:59.000000 map_pde-0.1/src/pde/constant.py
--rw-rw-rw-   0        0        0    14085 2023-04-09 02:50:43.000000 map_pde-0.1/src/pde/util.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:05:42.834775 map_pde-0.2/
+-rw-rw-rw-   0        0        0      279 2023-04-11 12:05:42.833778 map_pde-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2023-04-11 11:31:56.000000 map_pde-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-11 12:05:42.815770 map_pde-0.2/map_pde/
+-rw-rw-rw-   0        0        0        0 2023-03-23 06:21:32.000000 map_pde-0.2/map_pde/__init__.py
+-rw-rw-rw-   0        0        0    35309 2023-04-11 12:05:30.000000 map_pde-0.2/map_pde/client.py
+-rw-rw-rw-   0        0        0     5774 2023-04-09 02:53:59.000000 map_pde-0.2/map_pde/constant.py
+-rw-rw-rw-   0        0        0    14085 2023-04-09 02:50:43.000000 map_pde-0.2/map_pde/util.py
+drwxrwxrwx   0        0        0        0 2023-04-11 12:05:42.832776 map_pde-0.2/map_pde.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-11 12:05:42.000000 map_pde-0.2/map_pde.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-11 12:05:42.834775 map_pde-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      382 2023-04-11 12:05:30.000000 map_pde-0.2/setup.py
```

### Comparing `map_pde-0.1/src/pde/client.py` & `map_pde-0.2/map_pde/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from obspy.clients.fdsn.header import (DEFAULT_USER_AGENT, FDSNWS,
                                        URL_MAPPING_SUBPATHS,
                                        WADL_PARAMETERS_NOT_TO_BE_PARSED,
                                        FDSNRedirectException,
                                        FDSNNoServiceException)
 from obspy.clients.fdsn.wadl_parser import WADLParser
 from socket import timeout as socket_timeout
-from src.pde.constant import *
-from src.pde.util import *
+from map_pde.constant import *
+from map_pde.util import *
 
 
 class CustomRedirectHandler(urllib_request.HTTPRedirectHandler):
     """
     Custom redirection handler to also do it for POST requests which the
     standard library does not do by default.
     """
@@ -803,26 +803,26 @@
 
     def _get_token_local(self):
         """
         从本地获取token
         :return:
         """
         user_home = os.path.expanduser('~')
-        file_path = user_home + "\\pde\\token"
+        file_path = user_home + "\\map_pde\\token"
         if not os.path.exists(file_path):
             raise FDSNException("There is no token locally, if this is your first time using it, \n please go to "
                                 "'http://10.99.12.109:38090/login' to register an account to get the token, \n and "
                                 "initialize the token the first time you use it.")
         with open(file_path) as f:
             token = f.read()
         self.sa_token = token
 
     def _save_token_local(self):
         user_home = os.path.expanduser('~')
-        dir = user_home + "\\pde"
+        dir = user_home + "\\map_pde"
         if not os.path.exists(dir):
             os.mkdir(dir)
         file_path = dir + "\\token"
         with open(file_path, "w") as f:
             f.write(self.sa_token)
```

### Comparing `map_pde-0.1/src/pde/constant.py` & `map_pde-0.2/map_pde/constant.py`

 * *Files identical despite different names*

### Comparing `map_pde-0.1/src/pde/util.py` & `map_pde-0.2/map_pde/util.py`

 * *Files identical despite different names*

