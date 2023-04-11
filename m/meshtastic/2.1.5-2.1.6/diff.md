# Comparing `tmp/meshtastic-2.1.5.tar.gz` & `tmp/meshtastic-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.1.5.tar", last modified: Thu Apr  6 14:20:40 2023, max compression
+gzip compressed data, was "meshtastic-2.1.6.tar", last modified: Tue Apr 11 15:06:19 2023, max compression
```

## Comparing `meshtastic-2.1.5.tar` & `meshtastic-2.1.6.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:20:40.360386 meshtastic-2.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-06 14:20:27.000000 meshtastic-2.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-06 14:20:27.000000 meshtastic-2.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-06 14:20:40.360386 meshtastic-2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-06 14:20:27.000000 meshtastic-2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:20:40.360386 meshtastic-2.1.5/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48243 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/ble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/device_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    37473 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    18598 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30559 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-06 14:20:27.000000 meshtastic-2.1.5/meshtastic/xmodem_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:20:40.360386 meshtastic-2.1.5/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-06 14:20:40.000000 meshtastic-2.1.5/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-06 14:20:40.000000 meshtastic-2.1.5/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:20:40.000000 meshtastic-2.1.5/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-06 14:20:40.000000 meshtastic-2.1.5/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-06 14:20:40.000000 meshtastic-2.1.5/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 14:20:40.000000 meshtastic-2.1.5/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 14:20:40.360386 meshtastic-2.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-06 14:20:27.000000 meshtastic-2.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:19.637641 meshtastic-2.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-11 15:06:05.000000 meshtastic-2.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 15:06:05.000000 meshtastic-2.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-11 15:06:19.637641 meshtastic-2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-11 15:06:05.000000 meshtastic-2.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:19.637641 meshtastic-2.1.6/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48555 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/ble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/device_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37473 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18598 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12859 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30559 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-11 15:06:05.000000 meshtastic-2.1.6/meshtastic/xmodem_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 15:06:19.637641 meshtastic-2.1.6/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-11 15:06:19.000000 meshtastic-2.1.6/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 15:06:19.637641 meshtastic-2.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-11 15:06:05.000000 meshtastic-2.1.6/setup.py
```

### Comparing `meshtastic-2.1.5/LICENSE.txt` & `meshtastic-2.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/PKG-INFO` & `meshtastic-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.1.5/README.md` & `meshtastic-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/__init__.py` & `meshtastic-2.1.6/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/__main__.py` & `meshtastic-2.1.6/meshtastic/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,19 @@
             ch = interface.localNode.getChannelByChannelIndex(channelIndex)
             logging.debug(f"ch:{ch}")
             if ch and ch.role != channel_pb2.Channel.Role.DISABLED:
                 print(
                     f"Sending text message {args.sendtext} to {args.dest} on channelIndex:{channelIndex}"
                 )
                 interface.sendText(
-                    args.sendtext, args.dest, wantAck=True, channelIndex=channelIndex
+                    args.sendtext,
+                    args.dest,
+                    wantAck=True,
+                    channelIndex=channelIndex,
+                    onResponse=interface.getNode(args.dest, False).onAckNak,
                 )
             else:
                 meshtastic.util.our_exit(
                     f"Warning: {channelIndex} is not a valid channel. Channel must not be DISABLED."
                 )
 
         if args.sendping:
@@ -758,15 +762,15 @@
             # Even if others said we could close, stay open if the user asked for a tunnel
             closeNow = False
             if interface.noProto:
                 logging.warning(f"Not starting Tunnel - disabled by noProto")
             else:
                 tunnel.Tunnel(interface, subnet=args.tunnel_net)
 
-        if args.dest != BROADCAST_ADDR and waitForAckNak:
+        if args.ack or (args.dest != BROADCAST_ADDR and waitForAckNak):
             print(
                 f"Waiting for an acknowledgment from remote node (this could take a while)"
             )
             interface.getNode(args.dest, False).iface.waitForAckNak()
 
         # if the user didn't ask for serial debugging output, we might want to exit after we've done our operation
         if (not args.seriallog) and closeNow:
@@ -1180,14 +1184,20 @@
         help="Traceroute from connected node to a destination. "
         "You need pass the destination ID as argument, like "
         "this: '--traceroute !ba4bf9d0' "
         "Only nodes that have the encryption key can be traced.",
     )
 
     parser.add_argument(
+        "--ack",
+        help="Use in combination with --sendtext to wait for an acknowledgment.",
+        action="store_true",
+    )
+
+    parser.add_argument(
         "--reboot", help="Tell the destination node to reboot", action="store_true"
     )
 
     parser.add_argument(
         "--reboot-ota",
         help="Tell the destination node to reboot into factory firmware",
         action="store_true",
```

### Comparing `meshtastic-2.1.5/meshtastic/admin_pb2.py` & `meshtastic-2.1.6/meshtastic/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/apponly_pb2.py` & `meshtastic-2.1.6/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/ble_interface.py` & `meshtastic-2.1.6/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.1.6/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/channel_pb2.py` & `meshtastic-2.1.6/meshtastic/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/config_pb2.py` & `meshtastic-2.1.6/meshtastic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/connection_status_pb2.py` & `meshtastic-2.1.6/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/device_metadata_pb2.py` & `meshtastic-2.1.6/meshtastic/device_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/deviceonly_pb2.py` & `meshtastic-2.1.6/meshtastic/deviceonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/globals.py` & `meshtastic-2.1.6/meshtastic/globals.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/localonly_pb2.py` & `meshtastic-2.1.6/meshtastic/localonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/mesh_interface.py` & `meshtastic-2.1.6/meshtastic/mesh_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/mesh_pb2.py` & `meshtastic-2.1.6/meshtastic/mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/module_config_pb2.py` & `meshtastic-2.1.6/meshtastic/module_config_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\xaa\x17\n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x1a\x99\x01\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x1a\'\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1a\x9b\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"H\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x1a\xce\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\x86\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x42\x11\n\x0fpayload_variantBg\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\xb8\x17\n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x1a\xa7\x01\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x1a\'\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1a\x9b\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"H\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x1a\xce\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\x86\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x42\x11\n\x0fpayload_variantBg\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 
 
 _MODULECONFIG = DESCRIPTOR.message_types_by_name['ModuleConfig']
 _MODULECONFIG_MQTTCONFIG = _MODULECONFIG.nested_types_by_name['MQTTConfig']
 _MODULECONFIG_REMOTEHARDWARECONFIG = _MODULECONFIG.nested_types_by_name['RemoteHardwareConfig']
 _MODULECONFIG_AUDIOCONFIG = _MODULECONFIG.nested_types_by_name['AudioConfig']
@@ -112,35 +112,35 @@
 _sym_db.RegisterMessage(ModuleConfig.CannedMessageConfig)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\022ModuleConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _MODULECONFIG._serialized_start=35
-  _MODULECONFIG._serialized_end=3021
+  _MODULECONFIG._serialized_end=3035
   _MODULECONFIG_MQTTCONFIG._serialized_start=547
-  _MODULECONFIG_MQTTCONFIG._serialized_end=700
-  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_start=702
-  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=741
-  _MODULECONFIG_AUDIOCONFIG._serialized_start=744
-  _MODULECONFIG_AUDIOCONFIG._serialized_end=1089
-  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=922
-  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=1089
-  _MODULECONFIG_SERIALCONFIG._serialized_start=1092
-  _MODULECONFIG_SERIALCONFIG._serialized_end=1631
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=1291
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=1557
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=1559
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=1631
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=1634
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=1968
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=1971
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=2103
-  _MODULECONFIG_RANGETESTCONFIG._serialized_start=2105
-  _MODULECONFIG_RANGETESTCONFIG._serialized_end=2169
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=2172
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=2434
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=2437
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=3002
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=2903
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=3002
+  _MODULECONFIG_MQTTCONFIG._serialized_end=714
+  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_start=716
+  _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=755
+  _MODULECONFIG_AUDIOCONFIG._serialized_start=758
+  _MODULECONFIG_AUDIOCONFIG._serialized_end=1103
+  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=936
+  _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=1103
+  _MODULECONFIG_SERIALCONFIG._serialized_start=1106
+  _MODULECONFIG_SERIALCONFIG._serialized_end=1645
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=1305
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=1571
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=1573
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=1645
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=1648
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=1982
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=1985
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=2117
+  _MODULECONFIG_RANGETESTCONFIG._serialized_start=2119
+  _MODULECONFIG_RANGETESTCONFIG._serialized_end=2183
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=2186
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=2448
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=2451
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=3016
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=2917
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=3016
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.5/meshtastic/mqtt_pb2.py` & `meshtastic-2.1.6/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/node.py` & `meshtastic-2.1.6/meshtastic/node.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/portnums_pb2.py` & `meshtastic-2.1.6/meshtastic/portnums_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/remote_hardware.py` & `meshtastic-2.1.6/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.1.6/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/rtttl_pb2.py` & `meshtastic-2.1.6/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/serial_interface.py` & `meshtastic-2.1.6/meshtastic/serial_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/storeforward_pb2.py` & `meshtastic-2.1.6/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/stream_interface.py` & `meshtastic-2.1.6/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/supported_device.py` & `meshtastic-2.1.6/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/tcp_interface.py` & `meshtastic-2.1.6/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/telemetry_pb2.py` & `meshtastic-2.1.6/meshtastic/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/test.py` & `meshtastic-2.1.6/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/tunnel.py` & `meshtastic-2.1.6/meshtastic/tunnel.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/util.py` & `meshtastic-2.1.6/meshtastic/util.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic/xmodem_pb2.py` & `meshtastic-2.1.6/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.5/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.1.6/meshtastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.1.5
+Version: 2.1.6
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.1.5/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.1.6/meshtastic.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 meshtastic/__main__.py
 meshtastic/admin_pb2.py
 meshtastic/apponly_pb2.py
 meshtastic/ble.py
 meshtastic/ble_interface.py
 meshtastic/cannedmessages_pb2.py
 meshtastic/channel_pb2.py
+meshtastic/clientonly_pb2.py
 meshtastic/config_pb2.py
 meshtastic/connection_status_pb2.py
 meshtastic/device_metadata_pb2.py
 meshtastic/deviceonly_pb2.py
 meshtastic/globals.py
 meshtastic/localonly_pb2.py
 meshtastic/mesh_interface.py
```

### Comparing `meshtastic-2.1.5/setup.py` & `meshtastic-2.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.1.5",
+    version="2.1.6",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

