# Comparing `tmp/opb-20.tar.gz` & `tmp/opb-30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opb-20.tar", last modified: Sat Apr  8 01:43:29 2023, max compression
+gzip compressed data, was "opb-30.tar", last modified: Tue Apr 11 13:30:40 2023, max compression
```

## Comparing `opb-20.tar` & `opb-30.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-08 01:43:29.871067 opb-20/
--rw-r--r--   0 bart      (1000) bart      (1001)     6849 2023-04-08 01:43:29.871067 opb-20/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4582 2023-04-08 01:09:47.000000 opb-20/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-08 01:43:29.871067 opb-20/opb/
--rw-r--r--   0 bart      (1000) bart      (1001)      568 2023-04-08 00:31:48.000000 opb-20/opb/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      130 2023-04-07 21:53:44.000000 opb-20/opb/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1265 2023-04-07 21:51:57.000000 opb-20/opb/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5862 2023-04-07 21:51:57.000000 opb-20/opb/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-08 01:43:29.871067 opb-20/opb/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)       74 2023-04-08 00:33:46.000000 opb-20/opb/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      248 2023-04-07 21:51:57.000000 opb-20/opb/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      498 2023-04-07 21:51:57.000000 opb-20/opb/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18747 2023-04-07 23:18:11.000000 opb-20/opb/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7759 2023-04-07 23:18:42.000000 opb-20/opb/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3562 2023-04-07 23:17:36.000000 opb-20/opb/modules/shl.py
--rw-r--r--   0 bart      (1000) bart      (1001)      535 2023-04-07 21:51:57.000000 opb-20/opb/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1004 2023-04-07 21:51:57.000000 opb-20/opb/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)      315 2023-04-07 21:51:57.000000 opb-20/opb/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4991 2023-04-08 00:25:21.000000 opb-20/opb/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3067 2023-04-07 23:16:16.000000 opb-20/opb/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1938 2023-04-07 21:51:57.000000 opb-20/opb/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-07 21:51:57.000000 opb-20/opb/threads.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1455 2023-04-07 21:51:57.000000 opb-20/opb/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-08 01:43:29.871067 opb-20/opb.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     6849 2023-04-08 01:43:29.000000 opb-20/opb.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      524 2023-04-08 01:43:29.000000 opb-20/opb.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-08 01:43:29.000000 opb-20/opb.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        4 2023-04-08 01:43:29.000000 opb-20/opb.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-08 01:43:29.871067 opb-20/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)      947 2023-04-08 00:35:34.000000 opb-20/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-08 01:43:29.871067 opb-20/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      653 2023-04-07 21:51:57.000000 opb-20/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      352 2023-04-07 21:51:57.000000 opb-20/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      899 2023-04-07 21:51:57.000000 opb-20/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4549 2023-04-07 21:51:57.000000 opb-20/test/test_objects.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.877272 opb-30/
+-rw-r--r--   0 bart      (1000) bart      (1001)     6848 2023-04-11 13:30:40.877272 opb-30/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4582 2023-04-11 11:01:25.000000 opb-30/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.873272 opb-30/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1918 2023-04-11 13:07:29.000000 opb-30/bin/opb
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1003 2023-04-11 13:04:48.000000 opb-30/bin/opbc
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1181 2023-04-11 13:05:14.000000 opb-30/bin/opbd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.873272 opb-30/opb/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-11 11:17:26.000000 opb-30/opb/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6007 2023-04-11 13:17:07.000000 opb-30/opb/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.873272 opb-30/opb/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      248 2023-04-11 11:17:10.000000 opb-30/opb/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      498 2023-04-11 11:25:09.000000 opb-30/opb/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1136 2023-04-11 11:23:17.000000 opb-30/opb/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18718 2023-04-11 12:43:17.000000 opb-30/opb/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-11 11:23:41.000000 opb-30/opb/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2931 2023-04-11 11:23:30.000000 opb-30/opb/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17740 2023-04-11 11:24:16.000000 opb-30/opb/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2366 2023-04-11 11:04:11.000000 opb-30/opb/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7736 2023-04-11 11:25:34.000000 opb-30/opb/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      535 2023-04-11 11:19:26.000000 opb-30/opb/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1008 2023-04-11 11:19:48.000000 opb-30/opb/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1004 2023-04-11 11:20:05.000000 opb-30/opb/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2461 2023-04-11 13:16:47.000000 opb-30/opb/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      315 2023-04-11 11:23:52.000000 opb-30/opb/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5693 2023-04-11 11:04:11.000000 opb-30/opb/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4895 2023-04-11 11:03:12.000000 opb-30/opb/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3309 2023-04-11 11:18:06.000000 opb-30/opb/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1918 2023-04-11 13:21:17.000000 opb-30/opb/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-11 11:03:44.000000 opb-30/opb/threads.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.873272 opb-30/opb.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     6848 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      648 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       16 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/namespace_packages.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        4 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-11 13:30:40.877272 opb-30/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1116 2023-04-11 13:23:08.000000 opb-30/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.877272 opb-30/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      653 2023-04-11 11:01:25.000000 opb-30/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      352 2023-04-11 11:01:25.000000 opb-30/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      899 2023-04-11 11:01:25.000000 opb-30/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4549 2023-04-11 11:01:25.000000 opb-30/test/test_objects.py
```

### Comparing `opb-20/PKG-INFO` & `opb-30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: opb
-Version: 20
+Version: 30
 Summary: object programming bot
 Home-page: http://github.com/operbot/opb
-Author: Bart. Thate
+Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
         
         
         **NAME**
```

### Comparing `opb-20/README.rst` & `opb-30/README.rst`

 * *Files identical despite different names*

### Comparing `opb-20/opb/handler.py` & `opb-30/opb/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import inspect
 import queue
 import ssl
 import threading
 
 
-from opb.objects import Default, Object
-from opb.threads import launch
+from .objects import Default, Object
+from .threads import launch
 
 
 def __dir__():
     return (
             'Client',
             'Command',
             'Error',
@@ -156,18 +156,18 @@
         self.orig = None
         self.result = []
         self.sets = Default()
         self.skip = Default()
 
     def parse(self, txt):
         self.otxt = txt
-        spl = self.otxt.split()
+        splitted = self.otxt.split()
         args = []
         _nr = -1
-        for word in spl:
+        for word in splitted:
             if word.startswith('-'):
                 try:
                     self.index = int(word[1:])
                 except ValueError:
                     self.opts = self.opts + word[1:2]
                 continue
             try:
@@ -261,7 +261,15 @@
     return cfg
 
 
 def scan(mod):
     for _key, cmd in inspect.getmembers(mod, inspect.isfunction):
         if 'event' in cmd.__code__.co_varnames:
             Command.add(cmd.__name__, cmd)
+
+
+def spl(txt):
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
```

### Comparing `opb-20/opb/modules/irc.py` & `opb-30/opb/modules/irc.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 import ssl
 import time
 import textwrap
 import threading
 import _thread
 
 
+from opb.clocked import elapsed
 from opb.handler import Client, Command, Error, Event
 from opb.objects import Default, Object, keys, prt, update
 from opb.persist import find, fntime, last, write
 from opb.threads import launch
-from opb.utility import elapsed
 
 
 def __dir__():
     return (
             'Config',
             'IRC',
             'NoUser',
@@ -337,15 +337,14 @@
     def keep(self):
         while 1:
             self.connected.wait()
             self.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.command('PING', self.cfg.server)
-            time.sleep(10.0)
             if self.state.pongcheck:
                 self.state.pongcheck = False
                 self.keeprunning = False
                 self.reconnect()
 
 
     def logon(self, server, nck):
```

### Comparing `opb-20/opb/modules/rss.py` & `opb-30/opb/modules/rss.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,19 @@
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 from urllib.request import Request, urlopen
 
 
-from opb.clocked import Repeater
-from opb.handler import Listens
+from opb.clocked import Repeater, elapsed
+from opb.handler import Listens, spl
 from opb.objects import Object, prt, update
 from opb.persist import find, fntime, last, write
 from opb.threads import launch, threaded
-from opb.utility import elapsed, spl
 
 
 def __dir__():
     return (
         'Feed',
         'Fetcher',
         'Repeater',
```

### Comparing `opb-20/opb/modules/sts.py` & `opb-30/opb/modules/sts.py`

 * *Files identical despite different names*

### Comparing `opb-20/opb/modules/thr.py` & `opb-30/opb/modules/thr.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 "list running commands."
 
 
 import threading
 import time
 
 
+from opb.clocked import elapsed
 from opb.objects import Object, update
-from opb.utility import elapsed
 
 
 def __dir__():
     return (
             'thr',
            )
```

### Comparing `opb-20/opb/objects.py` & `opb-30/opb/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -213,15 +213,11 @@
         return JSONEncoder.encode(self, o)
 
     def iterencode(self, o, _one_shot=False) -> str:
         ""
         return JSONEncoder.iterencode(self, o, _one_shot)
 
 
-def dump(*args, **kw) -> None:
-    kw["cls"] = ObjectEncoder
-    return json.dump(*args, **kw)
-
 
 def dumps(*args, **kw) -> str:
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
```

### Comparing `opb-20/opb/persist.py` & `opb-30/opb/persist.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Tihs file is placed in the Public Domain.
 # pylint: disable=C0115,C0116,R0903,E0402
 
 
 "persistence"
 
 
+import json
 import os
 import pathlib
 import time
 import _thread
 
 
-from opb.objects import Object, dump, load, kind, search, update
+from .objects import Object, ObjectDecoder, ObjectEncoder
+from .objects import kind, search, update
 
 
 def __dir__():
     return (
             'Persist',
             'cdir',
             'last',
@@ -30,24 +32,29 @@
 
 
 disklock = _thread.allocate_lock()
 
 
 class Persist(Object):
 
-    workdir = os.path.expanduser("~/.opb")
+    workdir = os.path.expanduser("~/.opr")
 
 
 def cdir(pth) -> None:
     if not pth.endswith(os.sep):
         pth = os.path.dirname(pth)
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
 
 
+def dump(*args, **kw) -> None:
+    kw["cls"] = ObjectEncoder
+    return json.dump(*args, **kw)
+
+
 def files() -> []:
     return os.listdir(os.path.join(Persist.workdir, "store"))
 
 
 def fns(match) -> []:
     assert Persist.workdir
     dname = ''
@@ -67,14 +74,18 @@
 
 def hook(otp) -> Object:
     obj = Object()
     read(obj, otp)
     return obj
 
 
+def load(fpt, *args, **kw) -> Object:
+    return json.load(fpt, *args, cls=ObjectDecoder, **kw)
+
+
 def path(pth) -> str:
     return os.path.join(Persist.workdir, 'store', pth)
 
 
 def read(obj, pth) -> None:
     pth = path(pth)
     with disklock:
```

### Comparing `opb-20/opb/scanner.py` & `opb-30/opb/scanner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # This file is placed in the Public Domain.
-# pylint: disable=C0116,E0401
+# pylint: disable=C0116,E0401,E0402
 
 
 "introspection"
 
 
 import importlib
 import inspect
 import os
 
 
-from opb.handler import Command
-from opb.utility import spl
+from .handler import Command, spl
 
 
 def __dir__():
     return (
             'importer',
             'initer',
             'scan',
```

### Comparing `opb-20/opb/threads.py` & `opb-30/opb/threads.py`

 * *Files identical despite different names*

### Comparing `opb-20/opb.egg-info/PKG-INFO` & `opb-30/opb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: opb
-Version: 20
+Version: 30
 Summary: object programming bot
 Home-page: http://github.com/operbot/opb
-Author: Bart. Thate
+Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
         
         
         **NAME**
```

### Comparing `opb-20/opb.egg-info/SOURCES.txt` & `opb-30/opb.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 README.rst
 setup.py
-opb/__init__.py
-opb/__main__.py
+bin/opb
+bin/opbc
+bin/opbd
 opb/clocked.py
 opb/handler.py
 opb/objects.py
 opb/persist.py
 opb/scanner.py
 opb/threads.py
-opb/utility.py
 opb.egg-info/PKG-INFO
 opb.egg-info/SOURCES.txt
 opb.egg-info/dependency_links.txt
+opb.egg-info/namespace_packages.txt
 opb.egg-info/top_level.txt
-opb/modules/__init__.py
 opb/modules/cmd.py
 opb/modules/flt.py
+opb/modules/fnd.py
 opb/modules/irc.py
+opb/modules/log.py
+opb/modules/mbx.py
+opb/modules/mdl.py
+opb/modules/req.py
 opb/modules/rss.py
-opb/modules/shl.py
 opb/modules/sts.py
+opb/modules/tdo.py
 opb/modules/thr.py
+opb/modules/udp.py
 opb/modules/upt.py
+opb/modules/wsd.py
 test/test_decoder.py
 test/test_encoder.py
 test/test_inherit.py
 test/test_objects.py
```

### Comparing `opb-20/setup.py` & `opb-30/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,31 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="opb",
-    version="20",
-    author="Bart. Thate",
+    version="30",
+    author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/opb",
     description="object programming bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
     packages=[
               "opb",
               "opb.modules"
              ],
+    namespace_packages=[
+                        "opb",
+                        "opb.modules"
+                       ], 
+    scripts=["bin/opb", "bin/opbc", "bin/opbd"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: Public Domain",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
         "Intended Audience :: System Administrators",
         "Topic :: Communications :: Chat :: Internet Relay Chat",
```

### Comparing `opb-20/test/test_decoder.py` & `opb-30/test/test_decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         obj = Object()
         obj.test = "bla"
         oobj = loads(dumps(obj))
         self.assertEqual(oobj.test, "bla")
 
     def test_doctest(self):
         """
-            >>> from opq.objects import Object, dumps, loads
+            >>> from opb.objects import Object, dumps, loads
             >>> obj = Object()
             >>> obj.test = "bla"
             >>> oobj = loads(dumps(obj))
             >>> oobj.test
             'bla'
         """
         self.assertTrue(True)
```

### Comparing `opb-20/test/test_inherit.py` & `opb-30/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `opb-20/test/test_objects.py` & `opb-30/test/test_objects.py`

 * *Files identical despite different names*

