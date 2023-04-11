# Comparing `tmp/haicu-0.8.1.tar.gz` & `tmp/haicu-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.8.1.tar", last modified: Tue Apr 11 20:00:21 2023, max compression
+gzip compressed data, was "haicu-0.8.2.tar", last modified: Tue Apr 11 20:08:06 2023, max compression
```

## Comparing `haicu-0.8.1.tar` & `haicu-0.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:00:21.881911 haicu-0.8.1/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.8.1/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:00:21.881911 haicu-0.8.1/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     2042 2023-04-11 19:58:00.000000 haicu-0.8.1/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:00:21.881911 haicu-0.8.1/haicu/
--rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.8.1/haicu/__init__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    28538 2023-04-11 20:00:06.000000 haicu-0.8.1/haicu/__main__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:21:24.000000 haicu-0.8.1/haicu/format.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.8.1/haicu/ftdi.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:00:21.881911 haicu-0.8.1/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 20:00:21.000000 haicu-0.8.1/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      742 2023-04-11 20:00:16.000000 haicu-0.8.1/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 20:00:21.881911 haicu-0.8.1/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:08:06.498181 haicu-0.8.2/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.8.2/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:08:06.498181 haicu-0.8.2/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2042 2023-04-11 19:58:00.000000 haicu-0.8.2/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:08:06.498181 haicu-0.8.2/haicu/
+-rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.8.2/haicu/__init__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    28485 2023-04-11 20:07:56.000000 haicu-0.8.2/haicu/__main__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:21:24.000000 haicu-0.8.2/haicu/format.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.8.2/haicu/ftdi.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:08:06.498181 haicu-0.8.2/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 20:08:06.000000 haicu-0.8.2/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      742 2023-04-11 20:08:01.000000 haicu-0.8.2/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 20:08:06.498181 haicu-0.8.2/setup.cfg
```

### Comparing `haicu-0.8.1/LICENSE` & `haicu-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.8.1/PKG-INFO` & `haicu-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.8.1
+Version: 0.8.2
 Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

### Comparing `haicu-0.8.1/README.md` & `haicu-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `haicu-0.8.1/haicu/__main__.py` & `haicu-0.8.2/haicu/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     parser = argparse.ArgumentParser(prog=prog)
     parser.add_argument('--version', action='version', version='%(prog)s ' + VERSION)
     parser.add_argument('-v', '--verbose', action='count', default=0, help='Increase logging verbosity, can be repeated')
     parser.add_argument('-l', '--log', metavar='file', help='Log to output file')
     parser.add_argument('-s', '--serial', type=str, default='', help='MLD1200 serial of device to connect')
     parser.add_argument('-j', '--json', default=False, action='store_true', help='Send response as JSON object')
 
-    cmd_parser = parser.add_subparsers(dest="command", description="Valid subcommands", help=" ")
+    cmd_parser = parser.add_subparsers(metavar='{list,info,set,upload,program,convert,compare,monitor}', dest="command", description="Valid subcommands", help=" ")
 
     ftdi_list_parser = cmd_parser.add_parser("list", help="List available MLD1200 devices")
     ftdi_list_parser.set_defaults(func=arg_list)
 
     get_parser = cmd_parser.add_parser("info", help="Get status information")
     get_parser.set_defaults(func=arg_info)
 
@@ -121,48 +121,48 @@
     csv_parser = cmd_parser.add_parser("csv", help="Parse CSV file")
     csv_parser.add_argument("csvfile", type=str, help="CSV sum file")
     csv_parser.set_defaults(func=arg_csv)
 
     monitor_parser = cmd_parser.add_parser("monitor", help="Monitor MLD1200")
     monitor_parser.set_defaults(func=arg_monitor)
 
-    status_parser = cmd_parser.add_parser("status", aliases=['stat'], help=argparse.SUPPRESS)
+    status_parser = cmd_parser.add_parser("status", aliases=['stat'])
     status_parser.set_defaults(func=arg_status)
     status_parser.add_argument("addr", type=str, help="address to read")
 
-    reg_parser = cmd_parser.add_parser("control", aliases=['ctrl'], help=argparse.SUPPRESS)
+    reg_parser = cmd_parser.add_parser("control", aliases=['ctrl'])
     reg_parser.set_defaults(func=arg_reg)
     reg_parser.add_argument("addr", type=str, help="address to read/write")
     reg_parser.add_argument("data", nargs='?', type=str, help="32-bit value to write to register")
 
-    mem_parser = cmd_parser.add_parser("memory", aliases=['mem'], help=argparse.SUPPRESS)
+    mem_parser = cmd_parser.add_parser("memory", aliases=['mem'])
     mem_parser.set_defaults(func=arg_mem)
     mem_parser.add_argument("addr", type=str, help="24-bit address to read/write")
     mem_parser.add_argument("data", nargs='?', type=str, help="32-bit value to write to memory")
 
-    block_parser = cmd_parser.add_parser("bread", help=argparse.SUPPRESS)
+    block_parser = cmd_parser.add_parser("bread")
     block_parser.set_defaults(func=arg_block)
     block_parser.add_argument("addr", type=str, help="24-bit address to read")
     block_parser.add_argument("count", type=str, help="Number of words to read")
 
-    memtest_parser = cmd_parser.add_parser("memtest", help=argparse.SUPPRESS)
+    memtest_parser = cmd_parser.add_parser("memtest")
     memtest_parser.set_defaults(func=arg_memtest)
 
     args = parser.parse_args()
 
     try:
         ftdi_dev = haicu_ftdi.init(args.serial)
     except:
         print("Device '" + str(args.serial) + "' not found!")
         print()
         arg_list(args, None)
         sys.exit(-1)
 
     if(args.command == None):
-        parser.print_help()
+        parser.print_usage()
         sys.exit(0)
 
     args.func(args, ftdi_dev)
 
 def arg_list(args, ftdi_dev):
     print("Available devices:")
     result = haicu_ftdi.list_devices()
```

### Comparing `haicu-0.8.1/haicu/format.py` & `haicu-0.8.2/haicu/format.py`

 * *Files identical despite different names*

### Comparing `haicu-0.8.1/haicu/ftdi.py` & `haicu-0.8.2/haicu/ftdi.py`

 * *Files identical despite different names*

### Comparing `haicu-0.8.1/haicu.egg-info/PKG-INFO` & `haicu-0.8.2/haicu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.8.1
+Version: 0.8.2
 Summary: package for HAICU
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
```

