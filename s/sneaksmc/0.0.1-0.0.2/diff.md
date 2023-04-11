# Comparing `tmp/sneaksmc-0.0.1.tar.gz` & `tmp/sneaksmc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneaksmc-0.0.1.tar", last modified: Tue Apr 11 12:10:15 2023, max compression
+gzip compressed data, was "sneaksmc-0.0.2.tar", last modified: Tue Apr 11 12:41:47 2023, max compression
```

## Comparing `sneaksmc-0.0.1.tar` & `sneaksmc-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:10:15.556387 sneaksmc-0.0.1/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 12:10:15.556387 sneaksmc-0.0.1/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       36 2023-03-01 09:47:59.000000 sneaksmc-0.0.1/README.rst
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 12:10:15.556387 sneaksmc-0.0.1/setup.cfg
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 12:09:51.000000 sneaksmc-0.0.1/setup.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:10:15.552387 sneaksmc-0.0.1/sneaksmc/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       75 2023-04-11 09:09:09.000000 sneaksmc-0.0.1/sneaksmc/__init__.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     3123 2023-03-06 15:07:52.000000 sneaksmc-0.0.1/sneaksmc/client.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     6379 2023-03-02 10:22:52.000000 sneaksmc-0.0.1/sneaksmc/crypt.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)    25155 2023-04-11 08:42:06.000000 sneaksmc-0.0.1/sneaksmc/server.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:10:15.556387 sneaksmc-0.0.1/sneaksmc.egg-info/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 12:10:15.000000 sneaksmc-0.0.1/sneaksmc.egg-info/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 12:10:15.000000 sneaksmc-0.0.1/sneaksmc.egg-info/SOURCES.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 12:10:15.000000 sneaksmc-0.0.1/sneaksmc.egg-info/dependency_links.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 12:10:15.000000 sneaksmc-0.0.1/sneaksmc.egg-info/requires.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 12:10:15.000000 sneaksmc-0.0.1/sneaksmc.egg-info/top_level.txt
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       36 2023-03-01 09:47:59.000000 sneaksmc-0.0.2/README.rst
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/setup.cfg
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 12:40:54.000000 sneaksmc-0.0.2/setup.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/sneaksmc/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       75 2023-04-11 09:09:09.000000 sneaksmc-0.0.2/sneaksmc/__init__.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     3122 2023-04-11 12:37:44.000000 sneaksmc-0.0.2/sneaksmc/client.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     6379 2023-03-02 10:22:52.000000 sneaksmc-0.0.2/sneaksmc/crypt.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)    25182 2023-04-11 12:40:16.000000 sneaksmc-0.0.2/sneaksmc/server.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 12:41:47.096085 sneaksmc-0.0.2/sneaksmc.egg-info/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 12:41:46.000000 sneaksmc-0.0.2/sneaksmc.egg-info/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 12:41:47.000000 sneaksmc-0.0.2/sneaksmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 12:41:46.000000 sneaksmc-0.0.2/sneaksmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 12:41:47.000000 sneaksmc-0.0.2/sneaksmc.egg-info/requires.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 12:41:47.000000 sneaksmc-0.0.2/sneaksmc.egg-info/top_level.txt
```

### Comparing `sneaksmc-0.0.1/sneaksmc/client.py` & `sneaksmc-0.0.2/sneaksmc/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Clientk
 import http.client
 import time
-from .cryptk import Cryptk
+from .crypt import Cryptk
 
 
 class Clientk():
     def __init__(self) -> None:
         """ Initialize client to request and communicate with SMC coordinator """
         self.ck = Cryptk()
         self.coordinator_node = None
```

### Comparing `sneaksmc-0.0.1/sneaksmc/crypt.py` & `sneaksmc-0.0.2/sneaksmc/crypt.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.1/sneaksmc/server.py` & `sneaksmc-0.0.2/sneaksmc/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from os import getcwd
 
 # Since we run this server as its own script, we have to add it to path...
 import sys
 import os
 SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(os.path.dirname(SCRIPT_DIR))
-from smccryptk import Cryptk
+#from smccryptk import Cryptk
+from .crypt import Cryptk
 
 
 
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 # Certificate file is a file that is only used by the coordinator node.
 # It consists of all the other node's certificates (ip address + public key).
 certificate_file = __location__+"/.certificates.txt"
```

