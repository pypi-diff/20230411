# Comparing `tmp/opb-30.tar.gz` & `tmp/opb-31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opb-30.tar", last modified: Tue Apr 11 13:30:40 2023, max compression
+gzip compressed data, was "opb-31.tar", last modified: Tue Apr 11 13:55:29 2023, max compression
```

## Comparing `opb-30.tar` & `opb-31.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.877272 opb-30/
--rw-r--r--   0 bart      (1000) bart      (1001)     6848 2023-04-11 13:30:40.877272 opb-30/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     4582 2023-04-11 11:01:25.000000 opb-30/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.873272 opb-30/bin/
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1918 2023-04-11 13:07:29.000000 opb-30/bin/opb
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1003 2023-04-11 13:04:48.000000 opb-30/bin/opbc
--rwxr-xr-x   0 bart      (1000) bart      (1001)     1181 2023-04-11 13:05:14.000000 opb-30/bin/opbd
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.873272 opb-30/opb/
--rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-11 11:17:26.000000 opb-30/opb/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6007 2023-04-11 13:17:07.000000 opb-30/opb/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.873272 opb-30/opb/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      248 2023-04-11 11:17:10.000000 opb-30/opb/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      498 2023-04-11 11:25:09.000000 opb-30/opb/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1136 2023-04-11 11:23:17.000000 opb-30/opb/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18718 2023-04-11 12:43:17.000000 opb-30/opb/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-11 11:23:41.000000 opb-30/opb/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2931 2023-04-11 11:23:30.000000 opb-30/opb/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1001)    17740 2023-04-11 11:24:16.000000 opb-30/opb/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2366 2023-04-11 11:04:11.000000 opb-30/opb/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1001)     7736 2023-04-11 11:25:34.000000 opb-30/opb/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)      535 2023-04-11 11:19:26.000000 opb-30/opb/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1008 2023-04-11 11:19:48.000000 opb-30/opb/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1004 2023-04-11 11:20:05.000000 opb-30/opb/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2461 2023-04-11 13:16:47.000000 opb-30/opb/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1001)      315 2023-04-11 11:23:52.000000 opb-30/opb/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5693 2023-04-11 11:04:11.000000 opb-30/opb/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4895 2023-04-11 11:03:12.000000 opb-30/opb/objects.py
--rw-r--r--   0 bart      (1000) bart      (1001)     3309 2023-04-11 11:18:06.000000 opb-30/opb/persist.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1918 2023-04-11 13:21:17.000000 opb-30/opb/scanner.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-11 11:03:44.000000 opb-30/opb/threads.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.873272 opb-30/opb.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     6848 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)      648 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       16 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/namespace_packages.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        4 2023-04-11 13:30:40.000000 opb-30/opb.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-11 13:30:40.877272 opb-30/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)     1116 2023-04-11 13:23:08.000000 opb-30/setup.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:30:40.877272 opb-30/test/
--rw-r--r--   0 bart      (1000) bart      (1001)      653 2023-04-11 11:01:25.000000 opb-30/test/test_decoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      352 2023-04-11 11:01:25.000000 opb-30/test/test_encoder.py
--rw-r--r--   0 bart      (1000) bart      (1001)      899 2023-04-11 11:01:25.000000 opb-30/test/test_inherit.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4549 2023-04-11 11:01:25.000000 opb-30/test/test_objects.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.549208 opb-31/
+-rw-r--r--   0 bart      (1000) bart      (1001)     6732 2023-04-11 13:55:29.549208 opb-31/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     4466 2023-04-11 13:49:58.000000 opb-31/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.545208 opb-31/bin/
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1968 2023-04-11 13:53:03.000000 opb-31/bin/opb
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1003 2023-04-11 13:04:48.000000 opb-31/bin/opbc
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     1181 2023-04-11 13:05:14.000000 opb-31/bin/opbd
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.545208 opb-31/opb/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2143 2023-04-11 11:17:26.000000 opb-31/opb/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6007 2023-04-11 13:17:07.000000 opb-31/opb/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.545208 opb-31/opb/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      248 2023-04-11 11:17:10.000000 opb-31/opb/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      498 2023-04-11 11:25:09.000000 opb-31/opb/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1136 2023-04-11 11:23:17.000000 opb-31/opb/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18718 2023-04-11 12:43:17.000000 opb-31/opb/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      903 2023-04-11 11:23:41.000000 opb-31/opb/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2931 2023-04-11 11:23:30.000000 opb-31/opb/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    17740 2023-04-11 11:24:16.000000 opb-31/opb/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2366 2023-04-11 11:04:11.000000 opb-31/opb/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     7736 2023-04-11 11:25:34.000000 opb-31/opb/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      535 2023-04-11 11:19:26.000000 opb-31/opb/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1008 2023-04-11 11:19:48.000000 opb-31/opb/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1004 2023-04-11 11:20:05.000000 opb-31/opb/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2461 2023-04-11 13:16:47.000000 opb-31/opb/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      315 2023-04-11 11:23:52.000000 opb-31/opb/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5693 2023-04-11 11:04:11.000000 opb-31/opb/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4895 2023-04-11 11:03:12.000000 opb-31/opb/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     3309 2023-04-11 11:18:06.000000 opb-31/opb/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1918 2023-04-11 13:21:17.000000 opb-31/opb/scanner.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1867 2023-04-11 11:03:44.000000 opb-31/opb/threads.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.545208 opb-31/opb.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     6732 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)      648 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       16 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/namespace_packages.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        4 2023-04-11 13:55:29.000000 opb-31/opb.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2023-04-11 13:55:29.549208 opb-31/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)     1116 2023-04-11 13:50:48.000000 opb-31/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2023-04-11 13:55:29.549208 opb-31/test/
+-rw-r--r--   0 bart      (1000) bart      (1001)      653 2023-04-11 11:01:25.000000 opb-31/test/test_decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      352 2023-04-11 11:01:25.000000 opb-31/test/test_encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      899 2023-04-11 11:01:25.000000 opb-31/test/test_inherit.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4549 2023-04-11 11:01:25.000000 opb-31/test/test_objects.py
```

### Comparing `opb-30/PKG-INFO` & `opb-31/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opb
-Version: 30
+Version: 31
 Summary: object programming bot
 Home-page: http://github.com/operbot/opb
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -16,15 +16,15 @@
         ``OPB`` - object programming bot.
         
         
         **SYNOPSIS**
         
         ::
         
-         python3 -m opb [<cmd>|-c|-d] [key=value] [key==value]
+         opb [<cmd>|-c|-d] [key=value] [key==value]
         
         
         **DESCRIPTION**
         
         
         ``opb`` is a IRC bot, intended to be programmable, with a client program (opb),
         command line interface (opbc) and a daemon version (opbd), it provides object
@@ -61,49 +61,49 @@
         configuration is done by calling the ``cfg`` command:
         
         
         IRC
         
         ::
         
-         $ python3 -m opb cfg server=<server> channel=<channel> nick=<nick>
+         $ opb cfg server=<server> channel=<channel> nick=<nick>
         
          (*) default channel/server is #opb on localhost
         
         
         SASL
         
         ::
         
-         $ python3 -m opb pwd <nickservnick> <nickservpass>
-         $ python3 -m opb cfg password=<outputfrompwd>
+         $ opb pwd <nickservnick> <nickservpass>
+         $ opb cfg password=<outputfrompwd>
         
         
         USERS
         
         as default the user's userhost is not checked when a user types a command in a
         channel. To enable userhost checking enable users with the ``cfg`` command::
         
-         $ python3 -m opb cfg users=True
+         $ opb cfg users=True
         
         
         To add a user to the bot use the met command::
         
-         $ python3 -m opb  met <userhost>
+         $ opb  met <userhost>
         
         to delete a user use the del command with a substring of the userhost::
         
-         $ python3 -m opb del <substring>
+         $ opb del <substring>
         
         
         RSS
         
         ::
         
-         $ python3 -m opb rss <url>
+         $ opb rss <url>
         
         
         
         **RUNNING**
         
         
         this part shows how to run ``opb``.
@@ -112,39 +112,39 @@
         **cli**
         
         
         without any arguments ``opb`` doesn't respond, add arguments to have
         ``opb`` execute a command::
         
         
-         $ python3 -m opb
+         $ opb
          $
         
         
         the ``cmd`` command shows you a list of available commands::
         
         
-         $ python3 -m opb cmd
+         $ opb cmd
          cfg,cmd,dlt,dpl,flt,fnd,ftc,met,mre,nme,pwd,rem,rss,thr,upt
         
         
         **console**
         
         
         use the ``-c`` option to start the bot as a console::
         
-         $ python3 -m opb -c
+         $ opb -c
          OPB started at Fri Jan 6 01:49:58 2023
          > cmd
          cfg,cmd,dlt,dpl,flt,ftc,krn,log,met,mre,nme,pwd,rem,rss,thr,upt
          >
         
         running the bot in the background is done by using the ``-d`` option::
         
-         $ python3 -m opb -d
+         $ opb -d
          $
         
         
         **COMMANDS**
         
         
         here is a short description of the commands::
@@ -176,28 +176,28 @@
         attribute access and provides a save/load to/from json files on disk.
         Objects can be searched with database functions and uses read-only files
         to improve persistence and a type in filename for reconstruction. Methods are
         factored out into functions to have a clean namespace to read JSON data into.
         
         basic usage is this::
         
-         >>> from opb import Object
+         >>> from opb.objects import Object
          >>> o = Object()
          >>> o.key = "value"
          >>> o.key
          >>> 'value'
         
         Objects try to mimic a dictionary while trying to be an object with normal
         attribute access as well. hidden methods are provided, the methods are
         factored out into functions like get, items, keys, register, set, update
         and values.
         
         great for giving objects peristence by having their state stored in files::
         
-         >>> from opb import Object, write
+         >>> from opb.persist import Object, write
          >>> o = Object()
          >>> write(o)
          opb.objects.Object/89efa5fd7ad9497b96fdcb5f01477320/2022-11-21/17:20:12.221192
         
         
         **AUTHOR**
```

### Comparing `opb-30/README.rst` & `opb-31/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ``OPB`` - object programming bot.
 
 
 **SYNOPSIS**
 
 ::
 
- python3 -m opb [<cmd>|-c|-d] [key=value] [key==value]
+ opb [<cmd>|-c|-d] [key=value] [key==value]
 
 
 **DESCRIPTION**
 
 
 ``opb`` is a IRC bot, intended to be programmable, with a client program (opb),
 command line interface (opbc) and a daemon version (opbd), it provides object
@@ -53,49 +53,49 @@
 configuration is done by calling the ``cfg`` command:
 
 
 IRC
 
 ::
 
- $ python3 -m opb cfg server=<server> channel=<channel> nick=<nick>
+ $ opb cfg server=<server> channel=<channel> nick=<nick>
 
  (*) default channel/server is #opb on localhost
 
 
 SASL
 
 ::
 
- $ python3 -m opb pwd <nickservnick> <nickservpass>
- $ python3 -m opb cfg password=<outputfrompwd>
+ $ opb pwd <nickservnick> <nickservpass>
+ $ opb cfg password=<outputfrompwd>
 
 
 USERS
 
 as default the user's userhost is not checked when a user types a command in a
 channel. To enable userhost checking enable users with the ``cfg`` command::
 
- $ python3 -m opb cfg users=True
+ $ opb cfg users=True
 
 
 To add a user to the bot use the met command::
 
- $ python3 -m opb  met <userhost>
+ $ opb  met <userhost>
 
 to delete a user use the del command with a substring of the userhost::
 
- $ python3 -m opb del <substring>
+ $ opb del <substring>
 
 
 RSS
 
 ::
 
- $ python3 -m opb rss <url>
+ $ opb rss <url>
 
 
 
 **RUNNING**
 
 
 this part shows how to run ``opb``.
@@ -104,39 +104,39 @@
 **cli**
 
 
 without any arguments ``opb`` doesn't respond, add arguments to have
 ``opb`` execute a command::
 
 
- $ python3 -m opb
+ $ opb
  $
 
 
 the ``cmd`` command shows you a list of available commands::
 
 
- $ python3 -m opb cmd
+ $ opb cmd
  cfg,cmd,dlt,dpl,flt,fnd,ftc,met,mre,nme,pwd,rem,rss,thr,upt
 
 
 **console**
 
 
 use the ``-c`` option to start the bot as a console::
 
- $ python3 -m opb -c
+ $ opb -c
  OPB started at Fri Jan 6 01:49:58 2023
  > cmd
  cfg,cmd,dlt,dpl,flt,ftc,krn,log,met,mre,nme,pwd,rem,rss,thr,upt
  >
 
 running the bot in the background is done by using the ``-d`` option::
 
- $ python3 -m opb -d
+ $ opb -d
  $
 
 
 **COMMANDS**
 
 
 here is a short description of the commands::
@@ -168,28 +168,28 @@
 attribute access and provides a save/load to/from json files on disk.
 Objects can be searched with database functions and uses read-only files
 to improve persistence and a type in filename for reconstruction. Methods are
 factored out into functions to have a clean namespace to read JSON data into.
 
 basic usage is this::
 
- >>> from opb import Object
+ >>> from opb.objects import Object
  >>> o = Object()
  >>> o.key = "value"
  >>> o.key
  >>> 'value'
 
 Objects try to mimic a dictionary while trying to be an object with normal
 attribute access as well. hidden methods are provided, the methods are
 factored out into functions like get, items, keys, register, set, update
 and values.
 
 great for giving objects peristence by having their state stored in files::
 
- >>> from opb import Object, write
+ >>> from opb.persist import Object, write
  >>> o = Object()
  >>> write(o)
  opb.objects.Object/89efa5fd7ad9497b96fdcb5f01477320/2022-11-21/17:20:12.221192
 
 
 **AUTHOR**
```

### Comparing `opb-30/bin/opb` & `opb-31/bin/opb`

 * *Files 8% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     elif 'c' in cfg.opts:
         date = time.ctime(time.time()).replace('  ', ' ')
         print(f'OPB started {date}')
         csl = Console()
         launch(csl.loop)
         dowait = True
     if dowait:
+        scanpkg(opb.modules, starter, doall=True)
         scandir("modules", starter, doall=True)
         while 1:
             time.sleep(1.0)
             waiter()
 
 
 wrap(main)
```

### Comparing `opb-30/bin/opbc` & `opb-31/bin/opbc`

 * *Files identical despite different names*

### Comparing `opb-30/bin/opbd` & `opb-31/bin/opbd`

 * *Files identical despite different names*

### Comparing `opb-30/opb/clocked.py` & `opb-31/opb/clocked.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/handler.py` & `opb-31/opb/handler.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/fnd.py` & `opb-31/opb/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/irc.py` & `opb-31/opb/modules/irc.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/log.py` & `opb-31/opb/modules/log.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/mbx.py` & `opb-31/opb/modules/mbx.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/mdl.py` & `opb-31/opb/modules/mdl.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/req.py` & `opb-31/opb/modules/req.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/rss.py` & `opb-31/opb/modules/rss.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/sts.py` & `opb-31/opb/modules/sts.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/tdo.py` & `opb-31/opb/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/thr.py` & `opb-31/opb/modules/thr.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/udp.py` & `opb-31/opb/modules/udp.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/modules/wsd.py` & `opb-31/opb/modules/wsd.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/objects.py` & `opb-31/opb/objects.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/persist.py` & `opb-31/opb/persist.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/scanner.py` & `opb-31/opb/scanner.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb/threads.py` & `opb-31/opb/threads.py`

 * *Files identical despite different names*

### Comparing `opb-30/opb.egg-info/PKG-INFO` & `opb-31/opb.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opb
-Version: 30
+Version: 31
 Summary: object programming bot
 Home-page: http://github.com/operbot/opb
 Author: Bart Thate
 Author-email: operbot100@gmail.com
 License: Public Domain
 Description: README
         ######
@@ -16,15 +16,15 @@
         ``OPB`` - object programming bot.
         
         
         **SYNOPSIS**
         
         ::
         
-         python3 -m opb [<cmd>|-c|-d] [key=value] [key==value]
+         opb [<cmd>|-c|-d] [key=value] [key==value]
         
         
         **DESCRIPTION**
         
         
         ``opb`` is a IRC bot, intended to be programmable, with a client program (opb),
         command line interface (opbc) and a daemon version (opbd), it provides object
@@ -61,49 +61,49 @@
         configuration is done by calling the ``cfg`` command:
         
         
         IRC
         
         ::
         
-         $ python3 -m opb cfg server=<server> channel=<channel> nick=<nick>
+         $ opb cfg server=<server> channel=<channel> nick=<nick>
         
          (*) default channel/server is #opb on localhost
         
         
         SASL
         
         ::
         
-         $ python3 -m opb pwd <nickservnick> <nickservpass>
-         $ python3 -m opb cfg password=<outputfrompwd>
+         $ opb pwd <nickservnick> <nickservpass>
+         $ opb cfg password=<outputfrompwd>
         
         
         USERS
         
         as default the user's userhost is not checked when a user types a command in a
         channel. To enable userhost checking enable users with the ``cfg`` command::
         
-         $ python3 -m opb cfg users=True
+         $ opb cfg users=True
         
         
         To add a user to the bot use the met command::
         
-         $ python3 -m opb  met <userhost>
+         $ opb  met <userhost>
         
         to delete a user use the del command with a substring of the userhost::
         
-         $ python3 -m opb del <substring>
+         $ opb del <substring>
         
         
         RSS
         
         ::
         
-         $ python3 -m opb rss <url>
+         $ opb rss <url>
         
         
         
         **RUNNING**
         
         
         this part shows how to run ``opb``.
@@ -112,39 +112,39 @@
         **cli**
         
         
         without any arguments ``opb`` doesn't respond, add arguments to have
         ``opb`` execute a command::
         
         
-         $ python3 -m opb
+         $ opb
          $
         
         
         the ``cmd`` command shows you a list of available commands::
         
         
-         $ python3 -m opb cmd
+         $ opb cmd
          cfg,cmd,dlt,dpl,flt,fnd,ftc,met,mre,nme,pwd,rem,rss,thr,upt
         
         
         **console**
         
         
         use the ``-c`` option to start the bot as a console::
         
-         $ python3 -m opb -c
+         $ opb -c
          OPB started at Fri Jan 6 01:49:58 2023
          > cmd
          cfg,cmd,dlt,dpl,flt,ftc,krn,log,met,mre,nme,pwd,rem,rss,thr,upt
          >
         
         running the bot in the background is done by using the ``-d`` option::
         
-         $ python3 -m opb -d
+         $ opb -d
          $
         
         
         **COMMANDS**
         
         
         here is a short description of the commands::
@@ -176,28 +176,28 @@
         attribute access and provides a save/load to/from json files on disk.
         Objects can be searched with database functions and uses read-only files
         to improve persistence and a type in filename for reconstruction. Methods are
         factored out into functions to have a clean namespace to read JSON data into.
         
         basic usage is this::
         
-         >>> from opb import Object
+         >>> from opb.objects import Object
          >>> o = Object()
          >>> o.key = "value"
          >>> o.key
          >>> 'value'
         
         Objects try to mimic a dictionary while trying to be an object with normal
         attribute access as well. hidden methods are provided, the methods are
         factored out into functions like get, items, keys, register, set, update
         and values.
         
         great for giving objects peristence by having their state stored in files::
         
-         >>> from opb import Object, write
+         >>> from opb.persist import Object, write
          >>> o = Object()
          >>> write(o)
          opb.objects.Object/89efa5fd7ad9497b96fdcb5f01477320/2022-11-21/17:20:12.221192
         
         
         **AUTHOR**
```

### Comparing `opb-30/opb.egg-info/SOURCES.txt` & `opb-31/opb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opb-30/setup.py` & `opb-31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="opb",
-    version="30",
+    version="31",
     author="Bart Thate",
     author_email="operbot100@gmail.com",
     url="http://github.com/operbot/opb",
     description="object programming bot",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
```

### Comparing `opb-30/test/test_decoder.py` & `opb-31/test/test_decoder.py`

 * *Files identical despite different names*

### Comparing `opb-30/test/test_inherit.py` & `opb-31/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `opb-30/test/test_objects.py` & `opb-31/test/test_objects.py`

 * *Files identical despite different names*

