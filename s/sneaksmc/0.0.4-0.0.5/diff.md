# Comparing `tmp/sneaksmc-0.0.4.tar.gz` & `tmp/sneaksmc-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneaksmc-0.0.4.tar", last modified: Tue Apr 11 13:55:18 2023, max compression
+gzip compressed data, was "sneaksmc-0.0.5.tar", last modified: Tue Apr 11 18:46:29 2023, max compression
```

## Comparing `sneaksmc-0.0.4.tar` & `sneaksmc-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       36 2023-03-01 09:47:59.000000 sneaksmc-0.0.4/README.rst
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/setup.cfg
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 13:55:08.000000 sneaksmc-0.0.4/setup.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/sneaksmc/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.4/sneaksmc/__init__.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     3461 2023-04-11 13:50:50.000000 sneaksmc-0.0.4/sneaksmc/client.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.4/sneaksmc/crypt.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)    25027 2023-04-11 13:52:14.000000 sneaksmc-0.0.4/sneaksmc/server.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 13:55:18.156509 sneaksmc-0.0.4/sneaksmc.egg-info/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 13:55:17.000000 sneaksmc-0.0.4/sneaksmc.egg-info/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 13:55:18.000000 sneaksmc-0.0.4/sneaksmc.egg-info/SOURCES.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 13:55:17.000000 sneaksmc-0.0.4/sneaksmc.egg-info/dependency_links.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 13:55:18.000000 sneaksmc-0.0.4/sneaksmc.egg-info/requires.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 13:55:18.000000 sneaksmc-0.0.4/sneaksmc.egg-info/top_level.txt
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       79 2023-04-11 13:58:02.000000 sneaksmc-0.0.5/README.rst
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/setup.cfg
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 18:45:03.000000 sneaksmc-0.0.5/setup.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/sneaksmc/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.5/sneaksmc/__init__.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     3461 2023-04-11 13:50:50.000000 sneaksmc-0.0.5/sneaksmc/client.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.5/sneaksmc/crypt.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)    25031 2023-04-11 18:44:11.000000 sneaksmc-0.0.5/sneaksmc/server.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 18:46:29.077136 sneaksmc-0.0.5/sneaksmc.egg-info/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 18:46:28.000000 sneaksmc-0.0.5/sneaksmc.egg-info/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 18:46:29.000000 sneaksmc-0.0.5/sneaksmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 18:46:28.000000 sneaksmc-0.0.5/sneaksmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 18:46:28.000000 sneaksmc-0.0.5/sneaksmc.egg-info/requires.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 18:46:28.000000 sneaksmc-0.0.5/sneaksmc.egg-info/top_level.txt
```

### Comparing `sneaksmc-0.0.4/sneaksmc/client.py` & `sneaksmc-0.0.5/sneaksmc/client.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.4/sneaksmc/crypt.py` & `sneaksmc-0.0.5/sneaksmc/crypt.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.4/sneaksmc/server.py` & `sneaksmc-0.0.5/sneaksmc/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import argparse
 import random
 from http.server import BaseHTTPRequestHandler,HTTPServer
 import http.client
 from os import getcwd
 
 # Since we run this server as its own script, we have to add it to path...
-import sys
+#import sys
 import os
-SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
-sys.path.append(os.path.dirname(SCRIPT_DIR))
+#SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
+#sys.path.append(os.path.dirname(SCRIPT_DIR))
 from .crypt import Crypt
 
 
 
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 # Certificate file is a file that is only used by the coordinator node.
 # It consists of all the other node's certificates (ip address + public key).
@@ -135,23 +135,24 @@
             print("[Host: %s] Server has shut down" % host_name)
 
         def shutdown_server_on_signal(signum, frame):
             print("Received shutdown signal %d.. shutting down" % signum)
             server.shutdown()
             exit(0) # TODO: need this?
 
-        # Start server on a new thread
-        thread = threading.Thread(target=server_main)
-        thread.daemon = True
-        thread.start()
 
         # Shut down on kill (SIGTERM) and Ctrl-C (SIGINT)
         signal.signal(signal.SIGTERM, shutdown_server_on_signal)
         signal.signal(signal.SIGINT, shutdown_server_on_signal)
 
+        # Start server on a new thread
+        thread = threading.Thread(target=server_main)
+        thread.daemon = True
+        thread.start()
+
         # Shutdown automatic after _server_auto_shutdown has elapsed
         thread.join(_server_auto_shutdown)
         if thread.is_alive():
             server.shutdown()
```

