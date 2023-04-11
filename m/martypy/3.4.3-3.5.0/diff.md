# Comparing `tmp/martypy-3.4.3.tar.gz` & `tmp/martypy-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martypy-3.4.3.tar", last modified: Wed Jun 29 13:57:58 2022, max compression
+gzip compressed data, was "martypy-3.5.0.tar", last modified: Tue Apr 11 10:46:05 2023, max compression
```

## Comparing `martypy-3.4.3.tar` & `martypy-3.5.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2022-06-29 13:57:58.438987 martypy-3.4.3/
--rw-rw-rw-   0        0        0     2494 2022-06-29 13:56:20.000000 martypy-3.4.3/CHANGES.md
--rw-rw-rw-   0        0        0    11544 2022-06-28 13:52:45.000000 martypy-3.4.3/LICENSE.md
--rw-rw-rw-   0        0        0       91 2022-06-28 13:52:45.000000 martypy-3.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2152 2022-06-29 13:57:58.438987 martypy-3.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1291 2022-06-28 13:52:45.000000 martypy-3.4.3/README.md
-drwxrwxrwx   0        0        0        0 2022-06-29 13:57:58.414061 martypy-3.4.3/martypy/
--rw-rw-rw-   0        0        0    10411 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/ClientGeneric.py
--rw-rw-rw-   0        0        0    34852 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/ClientMV1.py
--rw-rw-rw-   0        0        0    35816 2022-06-29 13:53:07.000000 martypy-3.4.3/martypy/ClientMV2.py
--rw-rw-rw-   0        0        0      394 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/Exceptions.py
--rw-rw-rw-   0        0        0    10879 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/LikeHDLC.py
--rw-rw-rw-   0        0        0    54419 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/Marty.py
--rw-rw-rw-   0        0        0     3016 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/ProtocolOverAscii.py
--rw-rw-rw-   0        0        0     3163 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICCommsBase.py
--rw-rw-rw-   0        0        0      671 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICCommsParams.py
--rw-rw-rw-   0        0        0     9783 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICCommsSerial.py
--rw-rw-rw-   0        0        0     1235 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICCommsTest.py
--rw-rw-rw-   0        0        0     6541 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICCommsWiFi.py
--rw-rw-rw-   0        0        0     9266 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICHWElems.py
--rw-rw-rw-   0        0        0    32101 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICInterface.py
--rw-rw-rw-   0        0        0     6848 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICProtocols.py
--rw-rw-rw-   0        0        0     8792 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RICROSSerial.py
--rw-rw-rw-   0        0        0      759 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/RateAverager.py
--rw-rw-rw-   0        0        0      394 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/ValueAverager.py
--rw-rw-rw-   0        0        0     5877 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/WebSocket.py
--rw-rw-rw-   0        0        0     6048 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/WebSocketFrame.py
--rw-rw-rw-   0        0        0      232 2022-06-29 13:55:36.000000 martypy-3.4.3/martypy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-29 13:57:58.437991 martypy-3.4.3/martypy/tests/
--rw-rw-rw-   0        0        0        0 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/tests/__init__.py
--rw-rw-rw-   0        0        0      805 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/tests/testBaudRateSelection.py
--rw-rw-rw-   0        0        0     1632 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/tests/testColourSensor.py
--rw-rw-rw-   0        0        0     1442 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/tests/test_martypy.py
--rw-rw-rw-   0        0        0     4108 2022-06-28 13:52:45.000000 martypy-3.4.3/martypy/tests/testrob.py
-drwxrwxrwx   0        0        0        0 2022-06-29 13:57:58.429048 martypy-3.4.3/martypy.egg-info/
--rw-rw-rw-   0        0        0     2152 2022-06-29 13:57:57.000000 martypy-3.4.3/martypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      874 2022-06-29 13:57:58.000000 martypy-3.4.3/martypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-29 13:57:57.000000 martypy-3.4.3/martypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2022-06-29 13:57:58.000000 martypy-3.4.3/martypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-06-29 13:57:58.000000 martypy-3.4.3/martypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2022-06-29 11:49:09.000000 martypy-3.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       74 2022-06-29 13:57:58.440981 martypy-3.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1835 2022-06-29 13:56:31.000000 martypy-3.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:46:05.565529 martypy-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-11 10:45:55.000000 martypy-3.5.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-11 10:45:55.000000 martypy-3.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 10:45:55.000000 martypy-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-11 10:46:05.565529 martypy-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-11 10:45:55.000000 martypy-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:46:05.561529 martypy-3.5.0/martypy/
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/ClientGeneric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34847 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/ClientMV1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38446 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/ClientMV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10550 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/LikeHDLC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55547 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/Marty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/ProtocolOverAscii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICCommsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICCommsParams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICCommsSerial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICCommsTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICCommsWiFi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICHWElems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34125 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICProtocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8552 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICROSSerial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RICStreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/RateAverager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/ValueAverager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/WebSocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/WebSocketFrame.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:46:05.565529 martypy-3.5.0/martypy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/tests/testBaudRateSelection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/tests/testColourSensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/tests/testStreamMP3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/tests/test_martypy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-11 10:45:55.000000 martypy-3.5.0/martypy/tests/testrob.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:46:05.565529 martypy-3.5.0/martypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-11 10:46:05.000000 martypy-3.5.0/martypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-11 10:46:05.000000 martypy-3.5.0/martypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:46:05.000000 martypy-3.5.0/martypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-11 10:46:05.000000 martypy-3.5.0/martypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-11 10:46:05.000000 martypy-3.5.0/martypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-11 10:46:05.565529 martypy-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-11 10:45:55.000000 martypy-3.5.0/setup.py
```

### Comparing `martypy-3.4.3/CHANGES.md` & `martypy-3.5.0/CHANGES.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,65 @@
-Version 3.4.3 :
-- Resolved issue with missing dependency (package)
-- Resolved issue with ground and obstacle detection not being able to use sensor Name (rather than sensor side)
-
-Version 3.4.0 :
-- Support for ground and obstacle detection using the IR/Colour foot sensors
-- User callbacks on data received from the robot in the background
-- Automatically re-establish the WiFi connection if Marty reboots
-
-Version 3.3.1 :
-- Improved connection setup process (preparation for higher USB speeds)
-
-Version 3.3.0 :
-- New functions for controlling the disco add-on lights
-- New distance sensor function for Marty V2 that returns the distance in mm
-
-Version 3.2.1 :
-- Default `movetime` parameter for the `dance()` has been changed to 3000ms instead of 4500ms
-
-Version 3.2.0 :
-- New `Marty.add_on_query` method provides low-level access to Marty's addons
-- New `Marty.is_conn_ready` method for checking if Marty is connected
-- Small changes to the dictionary returned by `get_power_status()`
-- Stale power, servo and other information is no longer presented if updates from Marty cease
-- Various under-the-hood improvements, bugfixes and preparations for future features
-
-Version 3.1.0 :
-- Automatic Marty discovery when connecting over USB
-
-Version 3.0.3 :
-- Improved default parameters for `wiggle()` and `sidestep()`
-
-Version 3.0.0 :
-- **Blocking Mode**
-  - You can now select whether movement commands are blocking or non-blocking.
-  - The default behaviour changed from non-blocking to blocking.
-- New `stand_straight()` method matching the "Stand straight in <...>" Scratch block.
-- Marty V1 can `dance()` now!
-
-Version 2.2.0 :
-- Better defaults for movement commands
-- Various bugfixes including:
-  - The `walk()` command alternates steps by default
-  - You can use one `sidestep()` command to take multiple side-steps
-  - The `twist` argument to the `kick()` command now works
-  - We got a bit confused about which is left and which is right but Marty explained it to us!
-
-Version 2.1
-: Fixes a bug when connecting to Marty V1
-
-Version 2.0
-: Added Marty V2 support
-: Removed unnecessary imports
-: Dropped Python 2 support
-
-Version 1.2
-: Addresses security issues in `requests` and `urllib3` dependencies
-
-Version 1.1
-: Adds ROSClient and Distance Sensor support
-
-Version 1.0
-: SocketClient and TestClient provided
-
-Version 0.0.1 (Alpha)
-: Adds initial API implementation for Socket-based control. Adds client class structure
+Version 3.5.0 :
+- Add streaming sound support
+
+Version 3.4.0 :
+- Support for ground and obstacle detection using the IR/Colour foot sensors
+- User callbacks on data received from the robot in the background
+- Automatically re-establish the WiFi connection if Marty reboots
+
+Version 3.3.1 :
+- Improved connection setup process (preparation for higher USB speeds)
+
+Version 3.3.0 :
+- New functions for controlling the disco add-on lights
+- New distance sensor function for Marty V2 that returns the distance in mm
+
+Version 3.2.1 :
+- Default `movetime` parameter for the `dance()` has been changed to 3000ms instead of 4500ms
+
+Version 3.2.0 :
+- New `Marty.add_on_query` method provides low-level access to Marty's addons
+- New `Marty.is_conn_ready` method for checking if Marty is connected
+- Small changes to the dictionary returned by `get_power_status()`
+- Stale power, servo and other information is no longer presented if updates from Marty cease
+- Various under-the-hood improvements, bugfixes and preparations for future features
+
+Version 3.1.0 :
+- Automatic Marty discovery when connecting over USB
+
+Version 3.0.3 :
+- Improved default parameters for `wiggle()` and `sidestep()`
+
+Version 3.0.0 :
+- **Blocking Mode**
+  - You can now select whether movement commands are blocking or non-blocking.
+  - The default behaviour changed from non-blocking to blocking.
+- New `stand_straight()` method matching the "Stand straight in <...>" Scratch block.
+- Marty V1 can `dance()` now!
+
+Version 2.2.0 :
+- Better defaults for movement commands
+- Various bugfixes including:
+  - The `walk()` command alternates steps by default
+  - You can use one `sidestep()` command to take multiple side-steps
+  - The `twist` argument to the `kick()` command now works
+  - We got a bit confused about which is left and which is right but Marty explained it to us!
+
+Version 2.1
+: Fixes a bug when connecting to Marty V1
+
+Version 2.0
+: Added Marty V2 support
+: Removed unnecessary imports
+: Dropped Python 2 support
+
+Version 1.2
+: Addresses security issues in `requests` and `urllib3` dependencies
+
+Version 1.1
+: Adds ROSClient and Distance Sensor support
+
+Version 1.0
+: SocketClient and TestClient provided
+
+Version 0.0.1 (Alpha)
+: Adds initial API implementation for Socket-based control. Adds client class structure
```

### Comparing `martypy-3.4.3/LICENSE.md` & `martypy-3.5.0/LICENSE.md`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "{}"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2020 Robotical Ltd
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "{}"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2020 Robotical Ltd
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `martypy-3.4.3/PKG-INFO` & `martypy-3.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,63 @@
-Metadata-Version: 2.1
-Name: martypy
-Version: 3.4.3
-Summary: Python library for Marty the Robot V1 and V2
-Home-page: http://github.com/robotical/martypy
-Author: Robotical
-Author-email: hello@robotical.io
-Maintainer: Robotical
-Maintainer-email: hello@robotical.io
-License: Apache 2.0
-Keywords: ros,robot,marty,marty the robot,robotical
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE.md
-
-# martypy
-
-Python library to communicate with Marty the Robot V1 and V2 by Robotical
-
-[See the API Documentation](https://userguides.robotical.io/martyv2/documentation/python_function_reference)
-
-To regenerate documentation:
-- pip install -r dev-requirements.txt
-- pydoc-markdown --server --open
-
-## How to run example scripts
-
-If you cloned the repository or downloaded the source code to try the [example scripts](examples),
-you will need to make sure you have MartyPy installed before you can run the examples.
-
-The easiest way to install MartyPy is with the `pip install martypy` script as explained in
-[step 2 here](https://userguides.robotical.io/martyv2/userguides/python/setting_up_python_on_your_computer).
-
-If you would like to make modifications to the martypy library itself, it will be better to install
-it from source using the command `pip install --editable /path/to/martypy/repo` (replacing
-`/path/to/martypy/repo` as appropriate of course).
-
-If you do not want to "`pip install`" the MartyPy library, you can add the following 4 lines at the
-top (before any other code) of each script you want to run:
-
-```python
-import sys
-import pathlib
-cur_path = pathlib.Path(__file__).parent.resolve()
-sys.path.append(str(cur_path.parent.resolve()))
-```
+Metadata-Version: 2.1
+Name: martypy
+Version: 3.5.0
+Summary: Python library for Marty the Robot V1 and V2
+Home-page: http://github.com/robotical/martypy
+Author: Robotical
+Author-email: hello@robotical.io
+Maintainer: Robotical
+Maintainer-email: hello@robotical.io
+License: Apache 2.0
+Keywords: ros,robot,marty,marty the robot,robotical
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+License-File: LICENSE.md
+
+# martypy
+
+Python library to communicate with Marty the Robot V1 and V2 by Robotical
+
+[See the API Documentation](https://userguides.robotical.io/martyv2/documentation/python_function_reference)
+
+To regenerate documentation:
+- pip install -r dev-requirements.txt
+- pydoc-markdown --server --open
+
+## How to run example scripts
+
+If you cloned the repository or downloaded the source code to try the [example scripts](examples),
+you will need to make sure you have MartyPy installed before you can run the examples.
+
+The easiest way to install MartyPy is with the `pip install martypy` script as explained in
+[step 2 here](https://userguides.robotical.io/martyv2/userguides/python/setting_up_python_on_your_computer).
+
+Once martypy is installed you can run each example using python.
+The following (for the dance example) assumes you have connected your marty using the USB cable to a Windows computer
+
+python example_dance.py USB
+
+To run the sound example over WiFi when your Marty is connected on IP address 192.168.86.10, use:
+
+python example_sound.py WiFi 192.168.0.10
+
+If you would like to make modifications to the martypy library itself, it will be better to install
+it from source using the command `pip install --editable /path/to/martypy/repo` (replacing
+`/path/to/martypy/repo` as appropriate of course).
+
+If you do not want to "`pip install`" the MartyPy library, you can add the following 4 lines at the
+top (before any other code) of each script you want to run:
+
+```python
+import sys
+import pathlib
+cur_path = pathlib.Path(__file__).parent.resolve()
+sys.path.append(str(cur_path.parent.resolve()))
+```
```

### Comparing `martypy-3.4.3/README.md` & `martypy-3.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-# martypy
-
-Python library to communicate with Marty the Robot V1 and V2 by Robotical
-
-[See the API Documentation](https://userguides.robotical.io/martyv2/documentation/python_function_reference)
-
-To regenerate documentation:
-- pip install -r dev-requirements.txt
-- pydoc-markdown --server --open
-
-## How to run example scripts
-
-If you cloned the repository or downloaded the source code to try the [example scripts](examples),
-you will need to make sure you have MartyPy installed before you can run the examples.
-
-The easiest way to install MartyPy is with the `pip install martypy` script as explained in
-[step 2 here](https://userguides.robotical.io/martyv2/userguides/python/setting_up_python_on_your_computer).
-
-If you would like to make modifications to the martypy library itself, it will be better to install
-it from source using the command `pip install --editable /path/to/martypy/repo` (replacing
-`/path/to/martypy/repo` as appropriate of course).
-
-If you do not want to "`pip install`" the MartyPy library, you can add the following 4 lines at the
-top (before any other code) of each script you want to run:
-
-```python
-import sys
-import pathlib
-cur_path = pathlib.Path(__file__).parent.resolve()
-sys.path.append(str(cur_path.parent.resolve()))
-```
+# martypy
+
+Python library to communicate with Marty the Robot V1 and V2 by Robotical
+
+[See the API Documentation](https://userguides.robotical.io/martyv2/documentation/python_function_reference)
+
+To regenerate documentation:
+- pip install -r dev-requirements.txt
+- pydoc-markdown --server --open
+
+## How to run example scripts
+
+If you cloned the repository or downloaded the source code to try the [example scripts](examples),
+you will need to make sure you have MartyPy installed before you can run the examples.
+
+The easiest way to install MartyPy is with the `pip install martypy` script as explained in
+[step 2 here](https://userguides.robotical.io/martyv2/userguides/python/setting_up_python_on_your_computer).
+
+Once martypy is installed you can run each example using python.
+The following (for the dance example) assumes you have connected your marty using the USB cable to a Windows computer
+
+python example_dance.py USB
+
+To run the sound example over WiFi when your Marty is connected on IP address 192.168.86.10, use:
+
+python example_sound.py WiFi 192.168.0.10
+
+If you would like to make modifications to the martypy library itself, it will be better to install
+it from source using the command `pip install --editable /path/to/martypy/repo` (replacing
+`/path/to/martypy/repo` as appropriate of course).
+
+If you do not want to "`pip install`" the MartyPy library, you can add the following 4 lines at the
+top (before any other code) of each script you want to run:
+
+```python
+import sys
+import pathlib
+cur_path = pathlib.Path(__file__).parent.resolve()
+sys.path.append(str(cur_path.parent.resolve()))
+```
```

### Comparing `martypy-3.4.3/martypy/ClientMV2.py` & `martypy-3.5.0/martypy/ClientMV2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,780 +1,866 @@
-import logging
-import os
-import time
-import re
-from typing import Callable, Dict, List, Optional, Union, Tuple
-from packaging import version
-
-from .ClientGeneric import ClientGeneric
-from .RICCommsSerial import RICCommsSerial
-from .RICCommsWiFi import RICCommsWiFi
-from .RICCommsTest import RICCommsTest
-from .RICProtocols import DecodedMsg, RICProtocols
-from .RICROSSerial import RICROSSerial
-from .RICInterface import RICInterface
-from .RICHWElems import RICHWElems
-from .Exceptions import (MartyConnectException,
-                         MartyCommandException)
-
-logger = logging.getLogger(__name__)
-
-class ClientMV2(ClientGeneric):
-    '''
-    Lower level connector to Marty V2
-    '''
-    def __init__(self,
-                method: str,
-                locator: str,
-                serialBaud: int = None,
-                port = 80,
-                wsPath = "/ws",
-                subscribeRateHz = 10.0,
-                ricInterface: Optional[RICInterface] = None,
-                *args, **kwargs):
-        '''
-        Initialise connection to remote Marty
-        Args:
-            client_type: 'wifi' (for WiFi), 'usb' (for usb serial), 'exp' (for expansion serial),
-                'test' (output is available via get_test_output())
-            locator: str, ipAddress, hostname, serial-port, name of test file etc
-                    depending on method
-            serialBaud: serial baud rate
-            port: IP port for websockets
-            wsPath: path to use for websocket connection
-            subscribeRateHz: rate of fastest subscription to events
-        Raises:
-            MartyConnectException if the connection to the host failed
-        '''
-        # Call base constructor
-        super().__init__(*args, **kwargs)
-
-        # Initialise vars
-        self.subscribeRateHz = subscribeRateHz
-        self.lastRICSerialMsgTime = None
-        self.lastSubscrReqMsgTime = None
-        self.maxTimeBetweenPubs = 10
-        self.minTimeBetweenSubReqs = 10
-        self.max_blocking_wait_time = 120  # seconds
-        self.ricHardware = RICHWElems()
-        self.isClosing = False
-        self.ricSystemInfo = {}
-        self.ricHwElemsInfoByIDNo = {}
-        self.ricHwElemsList = []
-        self.loggingCallback = None
-        self.publishedMsgCallback = None
-        self.reportMsgCallback = None
-        self._initComplete = False
-        self.maxWaitForConnReadySecs = 10
-        self._minSysVersForSubscribeAPI = "1.0.0"
-        self._interfaceMethod = method
-        self._numHwStatusRetries = 10
-
-        # Check if we are given a RICInterface
-        if ricInterface is None:
-            # Handle the method of connection
-            if method == "usb" or method == "exp":
-                ifType = "overascii" if method == "usb" else "plain"
-                if serialBaud is None:
-                    serialBaud = 2000000 if method == "usb" else 921600
-                rifConfig = {
-                    "serialPort": locator,
-                    "serialBaud": serialBaud,
-                    "ifType": ifType,
-                }
-                self.ricIF = RICInterface(RICCommsSerial())
-            elif method == "test":
-                rifConfig = {
-                    "testFileName": locator
-                }
-                self.ricIF = RICInterface(RICCommsTest())
-            else:
-                rifConfig = {
-                    "ipAddrOrHostname": locator,
-                    "ipPort": port,
-                    "wsPath": wsPath,
-                    "ifType": "plain"
-                }
-                self.ricIF = RICInterface(RICCommsWiFi(self._onReconnect))
-        else:
-            rifConfig = {
-                "ipAddrOrHostname": locator,
-                "ifType": "plain"
-            }
-            self.ricIF = ricInterface
-
-        # Open comms
-        openOk = self.ricIF.open(rifConfig)
-        if not openOk:
-            raise MartyConnectException("Failed to open connection")
-
-        # Callbacks
-        self.ricIF.setDecodedMsgCB(self._rxDecodedMsg)
-        self.ricIF.setTimerCB(self._msgTimerCallback)
-        self.ricIF.setLogLineCB(self._logDebugMsg)
-
-    def start(self):
-        self._getRICVersion()
-        self._updateHwElemsInfo()
-        self._initComplete = True
-        # Wait for connection to be ready
-        waitStartTime = time.time()
-        while not self.is_conn_ready():
-            if time.time() - waitStartTime > self.maxWaitForConnReadySecs:
-                raise MartyConnectException("Connection to Marty not ready")
-            time.sleep(0.1)
-        # A flag is set on the first subscribed message - wait a little longer
-        # to ensure that one of each subscribed message type has been received
-        time.sleep(0.5)
-
-    def close(self):
-        if self.isClosing:
-            return
-        self.isClosing = True
-        # Stop any publishing messages
-        self._unsubscribeFromPubMessages()
-        # Close the RIC interface
-        self.ricIF.close()
-
-    def wait_if_required(self, expected_wait_ms: int, blocking_override: Union[bool, None]):
-        if not self.is_blocking(blocking_override):
-            return
-        if self.subscribeRateHz <= 0:
-            return
-
-        deadline = time.time() + expected_wait_ms/1000 + self.max_blocking_wait_time
-        time.sleep(2.5 * 1/self.subscribeRateHz)  # Give Marty time to report it is moving
-
-        # The is_moving flag may be cleared briefly between 2 queued trajectories
-        # Robot status may not be available for a while after Marty is turned on / connected to
-        while self.is_moving() or self.get_robot_status().get('workQCount', 1) > 0:
-            time.sleep(0.2 * 1/self.subscribeRateHz)
-            if time.time() > deadline:
-                raise TimeoutError("Marty wouldn't stop moving. Are you also controlling it via another method?"
-                                   f"{os.linesep}If you issued some very long-running non-blocking commands, "
-                                   "try increasing `marty.client.max_blocking_wait_time` (the current value "
-                                   f"is {self.max_blocking_wait_time} s)")
-
-    def hello(self) -> bool:
-        return self.ricIF.cmdRICRESTRslt("traj/getReady")
-
-    def get_ready(self) -> bool:
-        return self.ricIF.cmdRICRESTRslt("traj/getReady")
-
-    def stand_straight(self, move_time: int = 2000) -> bool:
-        return self.ricIF.cmdRICRESTRslt(f"traj/standStraight?moveTime={move_time}")
-
-    def discover(self) -> List[str]:
-        return []
-
-    def stop(self, stop_type: str, stopCode: int) -> bool:
-        robotRestCmd = "stop"
-        trajCmd = ""
-        if stopCode == 0: robotRestCmd = "stopAfterMove"
-        elif stopCode == 2: robotRestCmd = "panic"
-        elif stopCode == 3: trajCmd = "getReady"
-        elif stopCode == 4 or stopCode == 5: robotRestCmd = "pause"
-        isOk = self.ricIF.cmdRICRESTRslt("robot/" + robotRestCmd)
-        if len(trajCmd) > 0:
-            self.ricIF.cmdRICRESTRslt("traj/" + trajCmd)
-        return isOk
-
-    def resume(self) -> bool:
-        return self.ricIF.cmdRICRESTRslt("robot/resume")
-
-    def hold_position(self, hold_time: int) -> bool:
-        return self.ricIF.cmdRICRESTRslt(f"traj/hold?moveTime={hold_time}")
-
-    def move_joint(self, joint_id: int, position: int, move_time: int) -> bool:
-        return self.ricIF.cmdRICRESTRslt(f"traj/joint?jointID={joint_id}&angle={position}&moveTime={move_time}")
-
-    def get_joint_position(self, joint_id: Union[int, str]) -> float:
-        return self.ricHardware.getServoPos(joint_id, self.ricHwElemsInfoByIDNo)
-
-    def get_joint_current(self, joint_id: Union[int, str]) -> float:
-        return self.ricHardware.getServoCurrent(joint_id, self.ricHwElemsInfoByIDNo)
-
-    def get_joint_status(self, joint_id: Union[int, str]) -> int:
-        return self.ricHardware.getServoFlags(joint_id, self.ricHwElemsInfoByIDNo)
-
-    def lean(self, direction: str, amount: Optional[int], move_time: int) -> bool:
-        if amount is None:
-            amount = 29
-        try:
-            directionNum = ClientGeneric.SIDE_CODES[direction]
-        except KeyError:
-            self.preException(True)
-            raise MartyCommandException("Direction must be one of {}, not '{}'"
-                                        "".format(set(ClientGeneric.SIDE_CODES.keys()), direction))
-        return self.ricIF.cmdRICRESTRslt(f"traj/lean?side={directionNum}&leanAngle={amount}&moveTime={move_time}")
-
-    def walk(self, num_steps: int = 2, start_foot:str = 'auto', turn: int = 0,
-                step_length:int = 25, move_time: int = 1500) -> bool:
-        side_url_param = ''
-        if start_foot != 'auto':
-            try:
-                sideNum = ClientGeneric.SIDE_CODES[start_foot]
-            except KeyError:
-                raise MartyCommandException("Direction must be one of {}, not '{}'"
-                                            "".format(set(ClientGeneric.SIDE_CODES.keys()), start_foot))
-            side_url_param = f'&side={sideNum}'
-        return self.ricIF.cmdRICRESTRslt(f"traj/step/{num_steps}?stepLength={step_length}&turn={turn}"
-                                         f"&moveTime={move_time}" + side_url_param)
-
-    def eyes(self, joint_id: int, pose_or_angle: Union[str, int], move_time: int = 100) -> bool:
-        if type(pose_or_angle) is str:
-            try:
-                eyesTrajectory = ClientGeneric.EYE_POSES[pose_or_angle]
-            except KeyError:
-                raise MartyCommandException("pose must be one of {}, not '{}'"
-                                            "".format(set(ClientGeneric.EYE_POSES.keys()), pose_or_angle))
-            return self.ricIF.cmdRICRESTRslt(f"traj/{eyesTrajectory}")
-        return self.move_joint(joint_id, pose_or_angle, move_time)
-
-    def kick(self, side: str = 'right', twist: int = 0, move_time: int = 2500) -> bool:
-        if side != 'right' and side != 'left':
-            raise MartyCommandException("side must be one of 'right' or 'left', not '{}'"
-                                        "".format(side))
-        return self.ricIF.cmdRICRESTRslt(f"traj/kick?side={ClientGeneric.SIDE_CODES[side]}&moveTime={move_time}&turn={twist}")
-
-    def arms(self, left_angle: int, right_angle: int, move_time: int) -> bool:
-        self.move_joint(6, left_angle, move_time)
-        return self.move_joint(7, right_angle, move_time)
-
-    def celebrate(self, move_time: int = 4000) -> bool:
-
-        # TODO - add celebrate trajectory to Marty V2
-        return self.ricIF.cmdRICRESTRslt(f"traj/wiggle?moveTime={move_time}")
-
-    def circle_dance(self, side: str = 'right', move_time: int = 2500) -> bool:
-        if side != 'right' and side != 'left':
-            raise MartyCommandException("side must be one of 'right' or 'left', not '{}'"
-                                        "".format(side))
-        return self.ricIF.cmdRICRESTRslt(f"traj/circle?side={ClientGeneric.SIDE_CODES[side]}&moveTime={move_time}")
-
-    def dance(self, side: str = 'right', move_time: int = 3000) -> bool:
-        if side != 'right' and side != 'left':
-            raise MartyCommandException("side must be one of 'right' or 'left', not '{}'"
-                                        "".format(side))
-        return self.ricIF.cmdRICRESTRslt(f"traj/dance?side={ClientGeneric.SIDE_CODES[side]}&moveTime={move_time}")
-
-    def wiggle(self, move_time: int = 4000) -> bool:
-        return self.ricIF.cmdRICRESTRslt(f"traj/wiggle?moveTime={move_time}")
-
-    def sidestep(self, side: str, steps: int = 1, step_length: int = 35,
-            move_time: int = 1000) -> bool:
-        if side != 'right' and side != 'left':
-            raise MartyCommandException("side must be one of 'right' or 'left', not '{}'"
-                                        "".format(side))
-        return self.ricIF.cmdRICRESTRslt(f"traj/sidestep/{steps}?side={ClientGeneric.SIDE_CODES[side]}"
-                                         f"&stepLength={step_length}&moveTime={move_time}")
-
-    def play_sound(self, name_or_freq_start: Union[str,float],
-            freq_end: Optional[float] = None,
-            duration: Optional[int] = None) -> bool:
-        if not name_or_freq_start.lower().endswith(".raw"):
-                name_or_freq_start += ".raw"
-        return self.ricIF.cmdRICRESTRslt(f"filerun/{name_or_freq_start}")
-
-    def pinmode_gpio(self, gpio: int, mode: str) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def write_gpio(self, gpio: int, value: int) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def digitalread_gpio(self, gpio: int) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def i2c_write(self, *byte_array: int) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def i2c_write_to_ric(self, address: int, byte_array: bytes) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def get_battery_voltage(self) -> float:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def get_battery_remaining(self) -> float:
-        powerStatus = self.ricHardware.getPowerStatus()
-        return powerStatus.get("battRemainCapacityPercent", 0)
-
-    def get_distance_sensor(self) -> int:
-        for attached_add_on in self.get_add_ons_status().values():
-            if type(attached_add_on) == dict and attached_add_on['whoAmI'] == 'VCNL4200':
-                distance_bytes = attached_add_on['data'][1:3]
-                distance = int.from_bytes(distance_bytes, 'big')
-                return distance
-        return 0
-
-    def _index_data_color_ir(self, attached_add_on: str) -> Tuple[Tuple[int, int, int], str]:
-        '''
-        Parses data of passed-in color or IR sensor :two:
-        Args:
-            attached_add_on: Name of IR or color sensor add on
-        Returns:
-            A tuple with three integers of data (detection byte, obstacle value, ground value)
-            and a string of whether the sensor is a default 'left' or 'right' add on
-        '''
-        if attached_add_on['whoAmI'] == 'IRFoot':
-            detection_flags = attached_add_on['data'][1]
-            obstacle_data_raw = int.from_bytes(attached_add_on['data'][2:4], 'big')
-            ground_data_raw = int.from_bytes(attached_add_on['data'][4:6], 'big')
-            return (detection_flags, obstacle_data_raw, ground_data_raw), 'right'
-        if attached_add_on['whoAmI'] == 'coloursensor':
-            detection_flags = attached_add_on['data'][6]
-            obstacle_data_raw = int.from_bytes(attached_add_on['data'][8:10], 'big')
-            ground_data_raw = attached_add_on['data'][2]
-            return (detection_flags, obstacle_data_raw, ground_data_raw), 'left'
-
-    def _get_obstacle_and_ground_raw_data(self, add_on_or_side: str) -> list:
-        '''
-        Finds the wanted color or IR sensor and gets the parsed obstacle and ground data :two:
-        Args:
-            add_on_or_side: Takes in the name of a color sensor, name of an IR
-            sensor, `'left'` for the add on connected to the left foot,
-            or `'right'` for the add on connected to the right foot
-        Returns:
-            A tuple of the detection byte, obstacle reading, and ground reading of the add on
-        '''
-        sensor_whoamis = {'IRFoot', 'coloursensor'}
-        sensor_data = {'left': [], 'right': []}
-        sensor_possible_names = {
-            'left': ['LeftColorSensor', 'LeftIRFoot'],
-            'right': ['RightIRFoot', 'RightColorSensor']
-        }
-        addon_names = sensor_possible_names.get(add_on_or_side, [])
-
-        # There may be a situation just after connecting to RIC where publication messages from the addon
-        # have not yet been received so we need to wait for them to be received before we can parse them
-        for retryLoop in range(10):
-            addon_statuses = self.get_add_ons_status().values()
-            if len(addon_statuses) != 0:
-                break
-            time.sleep(0.1)
-
-        # Get the add-on values
-        for attached_add_on in addon_statuses:
-            if type(attached_add_on) == dict and attached_add_on.get('whoAmI','') in sensor_whoamis:
-                obstacle_and_ground_data, side = self._index_data_color_ir(attached_add_on)
-                if attached_add_on['name'] in addon_names:
-                    return obstacle_and_ground_data
-                else:
-                    sensor_data[side].append(obstacle_and_ground_data)
-        
-        sensor_possible_sides = sensor_possible_names.keys()
-        sensorSide = ""
-
-        for side in sensor_possible_sides:
-            if side in add_on_or_side.lower():
-                sensorSide = side
-
-        if len(sensorSide) > 0:
-            if len(sensor_data[sensorSide]) == 1:
-                return sensor_data[sensorSide][0]
-            elif add_on_or_side.lower() == 'left' or add_on_or_side.lower() == 'right':
-                raise MartyCommandException(
-                    f"Marty could not find a {add_on_or_side} sensor. "
-                    "Please make sure your add ons are plugged in and named correctly"
-                )
-            else:
-                raise MartyCommandException(
-                    f"The add on '{add_on_or_side}' is not a valid add on for obstacle and ground sensing."
-                    "Please make sure to pass in the name of an IR sensor or Color sensor."
-                )
-        else:
-            raise MartyCommandException(
-                f"The add on '{add_on_or_side}' is not a valid add on for obstacle and ground sensing."
-                "Please make sure to pass in the name of an IR sensor or Color sensor."
-            )
-
-    def foot_on_ground(self, add_on_or_side: str) -> bool:
-        raw_data = self._get_obstacle_and_ground_raw_data(add_on_or_side)
-        if len(raw_data) > 0:
-            return (raw_data[0] & 0b10) == 0b00
-        return False
-
-    def foot_obstacle_sensed(self, add_on_or_side: str) -> bool:
-        raw_data = self._get_obstacle_and_ground_raw_data(add_on_or_side)
-        if len(raw_data) > 0:
-            return (raw_data[0] & 0b1) == 0b1
-        return False
-
-    def get_obstacle_sensor_reading(self, add_on_or_side: str) -> int:
-        raw_data = self._get_obstacle_and_ground_raw_data(add_on_or_side)
-        if len(raw_data) > 1:
-            return raw_data[1]
-        return 0
-
-    def get_ground_sensor_reading(self, add_on_or_side: str) -> int:
-        raw_data = self._get_obstacle_and_ground_raw_data(add_on_or_side)
-        if len(raw_data) > 2:
-            return raw_data[2]
-        return 0
-
-    def get_accelerometer(self, axis: Optional[str] = None, axisCode: int = 0) -> float:
-        if axis is None:
-            return self.ricHardware.getIMUAll()
-        return self.ricHardware.getIMUAxisValue(axisCode)
-
-    def enable_motors(self, enable: bool = True, clear_queue: bool = True) -> bool:
-        return True
-
-    def enable_safeties(self, enable: bool = True) -> bool:
-        return True
-
-    def fall_protection(self, enable: bool = True) -> bool:
-        return True
-
-    def motor_protection(self, enable: bool = True) -> bool:
-        return True
-
-    def battery_protection(self, enable: bool = True) -> bool:
-        return True
-
-    def buzz_prevention(self, enable: bool = True) -> bool:
-        return True
-
-    def lifelike_behaviour(self, enable: bool = True) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def set_parameter(self, *byte_array: int) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def save_calibration(self) -> bool:
-        return self.ricIF.cmdRICRESTRslt(f"calibrate/set")
-
-    def clear_calibration(self) -> bool:
-        return self.ricIF.cmdRICRESTRslt(f"calibrate/setFlag/0")
-
-    def is_calibrated(self) -> bool:
-        result = self.ricIF.cmdRICRESTURLSync("calibrate")
-        if result.get("rslt", "") == "ok":
-            return result.get("calDone", 0) != 0
-        return False
-
-    def ros_command(self, *byte_array: int) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def keyframe (self, time: float, num_of_msgs: int, msgs) -> List[bytes]:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def get_chatter(self) -> bytes:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def get_firmware_version(self) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def _mute_serial(self) -> bool:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def ros_serial_formatter(self, topicID: int, send: bool = False, *message: int) -> List[int]:
-        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
-
-    def is_moving(self) -> bool:
-        return self.ricHardware.getIsMoving()
-
-    def is_paused(self) -> bool:
-        return self.ricHardware.getIsPaused()
-
-    def get_robot_status(self) -> Dict:
-        return self.ricHardware.getRobotStatus()
-
-    def get_joints(self) -> Dict:
-        return self.ricHardware.getServos(self.ricHwElemsInfoByIDNo)
-
-    def get_power_status(self) -> Dict:
-        return self.ricHardware.getPowerStatus()
-
-    def get_add_ons_status(self) -> Dict:
-        return self.ricHardware.getAddOns(self.ricHwElemsInfoByIDNo)
-
-    def get_add_on_status(self, add_on_name_or_id: Union[int, str]) -> Dict:
-        return self.ricHardware.getAddOn(add_on_name_or_id, self.ricHwElemsInfoByIDNo)
-
-    def add_on_query(self, add_on_name: str, data_to_write: bytes, num_bytes_to_read: int) -> Dict:
-        return self.ricIF.addOnQueryRaw(add_on_name, data_to_write, num_bytes_to_read)
-
-    def get_system_info(self) -> Dict:
-        return self.ricSystemInfo
-
-    def set_marty_name(self, name: str) -> bool:
-        escapedName = name.replace('"', '').replace('\n','')
-        return self.ricIF.cmdRICRESTRslt(f"friendlyname/{escapedName}")
-
-    def get_marty_name(self) -> str:
-        result = self.ricIF.cmdRICRESTURLSync("friendlyname")
-        if result.get("rslt", "") == "ok":
-            return result.get("friendlyName", "Marty")
-        return "Marty"
-
-    def is_marty_name_set(self) -> bool:
-        result = self.ricIF.cmdRICRESTURLSync("friendlyname")
-        if result.get("rslt", "") == "ok":
-            return result.get("friendlyNameIsSet", 0) != 0
-        return False
-
-    def get_hw_elems_list(self) -> List:
-        self._updateHwElemsInfo()
-        return self.ricHwElemsList
-
-    def send_ric_rest_cmd(self, ricRestCmd: str) -> None:
-        self.ricIF.sendRICRESTURL(ricRestCmd)
-
-    def send_ric_rest_cmd_sync(self, ricRestCmd: str) -> Dict:
-        return self.ricIF.cmdRICRESTURLSync(ricRestCmd)
-
-    def is_conn_ready(self) -> bool:
-        if not self.ricIF.isOpen():
-            return False
-        return self._initComplete and (self.lastRICSerialMsgTime is not None)
-
-    def _is_valid_disco_addon(self, add_on: str) -> bool:
-        disco_whoamis = {"LEDfoot", "LEDarm", "LEDeye"}
-        for attached_add_on in self.get_add_ons_status().values():
-            if type(attached_add_on) == dict and attached_add_on['name'] == add_on:
-                if attached_add_on['whoAmI'] in disco_whoamis:
-                    return True
-                else:
-                    raise MartyCommandException(f"The add on name: '{add_on}' is not a valid disco add on. "
-                                                "Please check the add on name in the scratch app -> configure -> add ons")
-        raise MartyCommandException(f"The add on name '{add_on}' is not a valid add on. Please check the add on "
-                                    "name in the scratch app -> configure -> add ons")
-
-    def disco_off(self, add_on: str) -> bool:
-        if self._is_valid_disco_addon(add_on):
-            response = self.add_on_query(add_on, bytes.fromhex('01'), 0)
-            return response.get("rslt", "") == "ok"
-
-    def disco_pattern(self, pattern: int, add_on: str) -> bool:
-        if pattern == 1:
-            pattern = '10'
-        elif pattern == 2:
-            pattern = '11'
-        else:
-            raise Exception("Pattern must be 1 or 2")
-        if self._is_valid_disco_addon(add_on):
-            response = self.add_on_query(add_on, bytes.fromhex(pattern), 0)
-            return response.get("rslt", "") == "ok"
-
-    def _region_to_bytes(self, region: Union[str, int]) -> bytes:
-        if region == 'all':
-            region = (2,)
-        else:
-            region = (4, region)
-        return bytes(region)
-
-    def _downscale_color(self, color: Union[tuple, bytes]):
-        return bytes(c//25 for c in color)
-
-    def _is_valid_color_hex(self, color_hex: str) -> bool:
-        hex_pattern = re.compile("^([A-Fa-f0-9]{6})$")
-        return bool(hex_pattern.match(color_hex))
-
-    def _parse_color_hex(self, color_hex: str, region: Union[str, int]) -> bytes:
-        input_color = color_hex
-        color_hex = color_hex.lstrip('#')
-        if self._is_valid_color_hex(color_hex):
-            color_bytes = bytes.fromhex(color_hex)
-        else:
-            raise MartyCommandException(f"The string '{input_color}' is not a valid hex color code or default color")
-        return color_bytes
-
-    def disco_color(self, color: Union[str, Tuple[int, int, int]], add_on: str, region: Union[int, str]) -> bool:
-        default_colors = {
-            'white'  : 'FFFFFF',
-            'red'    : 'FF0000',
-            'blue'   : '0000FF',
-            'yellow' : 'FFFF00',
-            'green'  : '008000',
-            'teal'   : '008080',
-            'pink'   : 'eb1362',
-            'purple' : '7800c8',
-            'orange' : '961900'
-        }
-        if type(color) is str:
-            color = default_colors.get(color.lower(), color)
-            color = self._parse_color_hex(color, region)
-        elif type(color) is tuple:
-            if len(color) != 3:
-                raise MartyCommandException(f'RGB tuple must be 3 numbers, instead of: {color}. Please enter a valid color.')
-        else:
-            raise MartyCommandException(f"Color must be of string or tuple form, not {type(color)}")
-        color = self._downscale_color(color)
-        region = self._region_to_bytes(region)
-        command = region + color
-        if self._is_valid_disco_addon(add_on):
-            response = self.add_on_query(add_on, command, 0)
-            return response.get("rslt", "") == "ok"
-
-    def disco_group_operation(self, disco_operation: Callable, whoamis: set, operation_kwargs: dict) -> bool:
-        '''
-        Calls disco operations in groups for multiple add ons :two:
-        Args:
-            disco_operation: function for disco add on
-            whoami_type_codes: the add ons that the function applies to
-            operation_kwargs: additional arguments that need to be passed into the operation
-        Returns:
-            True if Marty accepted all requests
-        '''
-        result = True
-        for attached_add_on in self.get_add_ons_status().values():
-            if type(attached_add_on) == dict and attached_add_on['whoAmI'] in whoamis:
-                addon_name = attached_add_on['name']
-                result = result and disco_operation(add_on=addon_name, **operation_kwargs)
-        return result
-
-    def register_logging_callback(self, loggingCallback: Callable[[str],None]) -> None:
-        '''
-        Register a callback function to be called on every log message from RIC.
-        Log messages are used mainly for debugging and error reporting.
-        Args:
-            messageCallback: a callback function (with one string argument - the log message)
-        Returns:
-            None
-        '''
-        self.loggingCallback = loggingCallback
-
-    def register_publish_callback(self, messageCallback: Callable[[int],None]) -> None:
-        '''
-        Register a callback function to be called on every message published by RIC.
-        RIC publishes information like the accelerometer and joint positions constantly.
-        If registered, the callback is called after the message is fully decoded, so a common
-        use-case is to check the topic (the int passed to the callback) to see if the information
-        is of interest (for example topic == Marty.PUBLISH_TOPIC_ACCELEROMETER if new accelerometer
-        data is available). Then get the changed information using the regular get_accelerometer method
-        (or get_joints, etc for other data).
-        Args:
-            messageCallback: a callback function (with one argument - the topic code of the published
-                    message) that will be called on every message published by RIC.
-        Returns:
-            None
-        '''
-        self.publishedMsgCallback = messageCallback
-
-    def register_report_callback(self, messageCallback: Callable[[str],None]) -> None:
-        '''
-        Register a callback function to be called on every report message recieved from RIC.
-        Report messages are used for alert conditions such as Falling, Over Current, etc.
-        The report message (passed in the callback function str) is a JSON string.
-        The elements of the JSON string include:
-            msgType: the type of report message (this will be "warn" for all alerts)
-            msgBody: the message text (this is "freeFallDet" or "overCurrentDet")
-            IDNo: the IDNo of the element that generated the report (the codes for these
-                are in the Marty.HW_ELEM_IDS dictionary but additional ones may appear if
-                add-ons create warnings - the IDNos of add-ons are not fixed numbers but you
-                can see the IDNo of add-ons by using the get_add_ons_status() method)
-        Args:
-            messageCallback: a callback function (with one string argument)
-                    that will be called on every message published by RIC.
-        Returns:
-            None
-        '''
-        self.reportMsgCallback = messageCallback
-
-    def get_interface_stats(self) -> Dict:
-        ricIFStats = self.ricIF.getStats()
-        publishInfo = self.ricHardware.getPublishStats()
-        ricIFStats.update(publishInfo)
-        return ricIFStats
-
-    def preException(self, isFatal: bool) -> None:
-        if isFatal:
-            self.ricIF.close()
-        logger.debug(f"Pre-exception isFatal {isFatal}")
-
-    def _rxDecodedMsg(self, decodedMsg: DecodedMsg, interface: RICInterface):
-        if decodedMsg.protocolID == RICProtocols.PROTOCOL_ROSSERIAL:
-            # logger.debug(f"ROSSERIAL message received {len(decodedMsg.payload)}")
-            self.lastRICSerialMsgTime = time.time()
-            if decodedMsg.payload:
-                RICROSSerial.decode(decodedMsg.payload, 0, self._rxPublishedMsg)
-        elif decodedMsg.protocolID == RICProtocols.PROTOCOL_RICREST:
-            # logger.debug(f"RIC REST message received {decodedMsg.payload}")
-            # Callback for REPORT messages
-            if (self.reportMsgCallback is not None) and (decodedMsg.msgTypeCode == RICProtocols.MSG_TYPE_REPORT):
-                try:
-                    self.reportMsgCallback(decodedMsg.payload)
-                except:
-                    logger.exception("Report callback failed:")
-        else:
-            logger.debug(f"RIC UNKNOWN message received {decodedMsg.payload}")
-            pass
-
-    def _rxPublishedMsg(self, topicID: int, payload: bytes):
-        # Decode the message
-        self.ricHardware.updateWithROSSerialMsg(topicID, payload)
-        # Callback on published messages
-        if self.publishedMsgCallback is not None:
-            try:
-                self.publishedMsgCallback(topicID)
-            except:
-                logger.exception("Publish callback failed:")
-
-    def _logDebugMsg(self, logMsg: str) -> None:
-        if self.loggingCallback:
-            try:
-                self.loggingCallback(logMsg)
-            except:
-                logger.exception("Logging callback failed:")
-
-    def _msgTimerCallback(self) -> None:
-        if self.isClosing:
-            return
-        self._subscribeToPubMessages(False)
-
-    def _getRICVersion(self) -> bool:
-        # Retries here to allow for baud-rate changes, etc
-        for retries in range(self._numHwStatusRetries):
-            # logger.debug(f"_getRICVersion attempt {retries+1}")
-            self.ricSystemInfo = self.ricIF.cmdRICRESTURLSync("v")
-            if self.ricSystemInfo.get("rslt", "") == "ok":
-                break
-        logger.debug(f"_getRICVersion rslt {self.ricSystemInfo.get('rslt', '')}")
-        return self.ricSystemInfo.get("rslt", "") == "ok"
-
-    def _updateHwElemsInfo(self):
-        hwElemsInfo = self.ricIF.cmdRICRESTURLSync("hwstatus")
-        if hwElemsInfo.get("rslt", "") == "ok":
-            self.ricHwElemsList = hwElemsInfo.get("hw", [])
-            self.ricHwElemsInfoByIDNo = {}
-            for el in self.ricHwElemsList:
-                if "IDNo" in el:
-                    self.ricHwElemsInfoByIDNo[el["IDNo"]] = el
-
-    def get_test_output(self) -> dict:
-        return self.ricIF.getTestOutput()
-
-    def _systemVersionGtEq(self, compareToVersion):
-        if self.ricSystemInfo is None:
-            return False
-        versInfo = self.ricSystemInfo.get("SystemVersion","0.0.0")
-        return version.parse(versInfo) >= version.parse(compareToVersion)
-
-    def _subscribeToPubMessages(self, forceResubscribe: bool):
-        versOk = self._systemVersionGtEq(self._minSysVersForSubscribeAPI)
-        timeForSubscr = self.lastRICSerialMsgTime is None or time.time() > self.lastRICSerialMsgTime + self.maxTimeBetweenPubs
-        resubscrReqd = self.lastSubscrReqMsgTime is None or time.time() > self.lastSubscrReqMsgTime + self.minTimeBetweenSubReqs
-        if versOk and self._initComplete and self.subscribeRateHz != 0 and (forceResubscribe or (timeForSubscr and resubscrReqd)):
-            # Subscribe for publication messages
-            logger.debug(f"Subscribe to published messages")
-            self.ricIF.sendRICRESTCmdFrame('{"cmdName":"subscription","action":"update",' + \
-                            '"pubRecs":[' + \
-                                '{' + f'"name":"MultiStatus","rateHz":{self.subscribeRateHz},' + '}' + \
-                                '{"name":"PowerStatus","rateHz":1.0},' + \
-                                '{' + f'"name":"AddOnStatus","rateHz":{self.subscribeRateHz}' + '}' + \
-                            ']}')
-            self.lastSubscrReqMsgTime = time.time()
-
-    def _unsubscribeFromPubMessages(self):
-        if self._systemVersionGtEq(self._minSysVersForSubscribeAPI):
-            # Send unsubscribe request
-            self.ricIF.sendRICRESTCmdFrame('{"cmdName":"subscription","action":"update",' + \
-                '"pubRecs":[' + \
-                    '{"name":"MultiStatus","rateHz":0},' + \
-                    '{"name":"PowerStatus","rateHz":0},' + \
-                    '{"name":"AddOnStatus","rateHz":0}' + \
-                ']}')
-            # Allow message to be sent
-            time.sleep(0.5)
-
-    def _onReconnect(self):
-        self._subscribeToPubMessages(True)
+import logging
+import os
+import time
+import re
+from typing import Callable, Dict, List, Optional, Union, Tuple
+from packaging import version
+
+from .ClientGeneric import ClientGeneric
+from .RICCommsSerial import RICCommsSerial
+from .RICCommsWiFi import RICCommsWiFi
+from .RICCommsTest import RICCommsTest
+from .RICProtocols import DecodedMsg, RICProtocols
+from .RICROSSerial import RICROSSerial
+from .RICInterface import RICInterface
+from .RICHWElems import RICHWElems
+from .Exceptions import (MartyConnectException,
+                         MartyCommandException)
+
+logger = logging.getLogger(__name__)
+
+class ClientMV2(ClientGeneric):
+    '''
+    Lower level connector to Marty V2
+    '''
+    def __init__(self,
+                method: str,
+                locator: str,
+                serialBaud: int = None,
+                port = 80,
+                wsPath = "/ws",
+                subscribeRateHz = 10.0,
+                ricInterface: Optional[RICInterface] = None,
+                *args, **kwargs):
+        '''
+        Initialise connection to remote Marty
+        Args:
+            client_type: 'wifi' (for WiFi), 'usb' (for usb serial), 'exp' (for expansion serial),
+                'test' (output is available via get_test_output())
+            locator: str, ipAddress, hostname, serial-port, name of test file etc
+                    depending on method
+            serialBaud: serial baud rate
+            port: IP port for websockets
+            wsPath: path to use for websocket connection
+            subscribeRateHz: rate of fastest subscription to events
+        Raises:
+            MartyConnectException if the connection to the host failed
+        '''
+        # Call base constructor
+        super().__init__(*args, **kwargs)
+
+        # Initialise vars
+        self.subscribeRateHz = subscribeRateHz
+        self.lastRICSerialMsgTime = None
+        self.lastSubscrReqMsgTime = None
+        self.maxTimeBetweenPubs = 10
+        self.minTimeBetweenSubReqs = 10
+        self.max_blocking_wait_time = 120  # seconds
+        self.ricHardware = RICHWElems()
+        self.isClosing = False
+        self.ricSystemInfo = {}
+        self.ricHwElemsInfoByIDNo = {}
+        self.ricHwElemsList = []
+        self.loggingCallback = None
+        self.publishedMsgCallback = None
+        self.reportMsgCallback = None
+        self._initComplete = False
+        self.maxWaitForConnReadySecs = 10
+        self._minSysVersForSubscribeAPI = "1.0.0"
+        self._interfaceMethod = method
+        self._numHwStatusRetries = 10
+        self._sendFileProgressCB = None
+        self._playMP3ProgressCB = None
+        # Debug
+        self.DEBUG_RECEIVE_PUBLISHED_MSG = False
+        self.DEBUG_RECEIVE_RICREST_MSGS = False
+        self.DEBUG_GET_RIC_VERSION = False
+        self.DEBUG_GET_HW_ELEMS_INFO = False
+        self.DEBUG_SUBSCRIBE_TO_PUB_MSGS = False
+        self.DEBUG_CONNECTION_PROCESS = False
+
+        # Check if we are given a RICInterface
+        if ricInterface is None:
+            # Handle the method of connection
+            if method == "usb" or method == "exp":
+                ifType = "overascii" if method == "usb" else "plain"
+                if serialBaud is None:
+                    serialBaud = 115200 if method == "usb" else 921600
+                rifConfig = {
+                    "serialPort": locator,
+                    "serialBaud": serialBaud,
+                    "ifType": ifType,
+                }
+                self.ricIF = RICInterface(RICCommsSerial())
+            elif method == "test":
+                rifConfig = {
+                    "testFileName": locator
+                }
+                self.ricIF = RICInterface(RICCommsTest())
+            else:
+                rifConfig = {
+                    "ipAddrOrHostname": locator,
+                    "ipPort": port,
+                    "wsPath": wsPath,
+                    "ifType": "plain"
+                }
+                self.ricIF = RICInterface(RICCommsWiFi(self._onReconnect))
+        else:
+            rifConfig = {
+                "ipAddrOrHostname": locator,
+                "ifType": "plain"
+            }
+            self.ricIF = ricInterface
+
+        # Debug
+        ricConnStartTime = time.time()
+        if self.DEBUG_CONNECTION_PROCESS:
+            logger.debug("Starting to connect to RIC")
+
+        # Open comms
+        openOk = self.ricIF.open(rifConfig)
+        if not openOk:
+            raise MartyConnectException("Failed to open connection")
+
+        # Debug
+        if self.DEBUG_CONNECTION_PROCESS:
+            logger.debug(f"RIC interface connection took {time.time() - ricConnStartTime} seconds")
+
+        # Callbacks
+        self.ricIF.setDecodedMsgCB(self._rxDecodedMsg)
+        self.ricIF.setTimerCB(self._msgTimerCallback)
+        self.ricIF.setLogLineCB(self._logDebugMsg)
+
+    def start(self):
+        # Debug
+        debugRICOverallStart = time.time()
+        debugStartTime = time.time()
+        if self.DEBUG_CONNECTION_PROCESS:
+            logger.debug("Starting to communicate with RIC")
+
+        # Get the version of RIC
+        self._getRICVersion()
+
+        # Debug
+        if self.DEBUG_CONNECTION_PROCESS:
+            logger.debug(f"Got RIC version in {time.time() - debugStartTime} seconds")
+        debugStartTime = time.time()
+
+        # Get HWElems
+        self._updateHwElemsInfo()
+
+        # Debug
+        if self.DEBUG_CONNECTION_PROCESS:
+            logger.debug(f"Got HWElems in {time.time() - debugStartTime} seconds")
+
+        # Now completed init
+        self._initComplete = True
+
+        # Debug
+        # self._updateHwElemsInfo()
+
+        # Wait for connection to be ready
+        waitStartTime = time.time()
+        while not self.is_conn_ready():
+            if time.time() - waitStartTime > self.maxWaitForConnReadySecs:
+                raise MartyConnectException("Connection to Marty not ready")
+            time.sleep(0.1)
+
+        # Debug
+        if self.DEBUG_CONNECTION_PROCESS:
+            logger.debug(f"Marty wait for ready time {time.time() - debugStartTime} seconds")
+
+        # A flag is set on the first subscribed message - wait a little longer
+        # to ensure that one of each subscribed message type has been received
+        time.sleep(0.5)
+
+        # Debug
+        if self.DEBUG_CONNECTION_PROCESS:
+            logger.debug(f"Marty overall start time {time.time() - debugRICOverallStart} seconds")
+
+    def close(self):
+        if self.isClosing:
+            return
+        self.isClosing = True
+        # Send unsubscribe request
+        self._unsubscribeFromPubMessages()
+        # Close the RIC interface
+        self.ricIF.close()
+
+    def wait_if_required(self, expected_wait_ms: int, blocking_override: Union[bool, None]):
+        if not self.is_blocking(blocking_override):
+            return
+        if self.subscribeRateHz <= 0:
+            return
+
+        deadline = time.time() + expected_wait_ms/1000 + self.max_blocking_wait_time
+        time.sleep(2.5 * 1/self.subscribeRateHz)  # Give Marty time to report it is moving
+
+        # The is_moving flag may be cleared briefly between 2 queued trajectories
+        # Robot status may not be available for a while after Marty is turned on / connected to
+        while self.is_moving() or self.get_robot_status().get('workQCount', 1) > 0:
+            time.sleep(0.2 * 1/self.subscribeRateHz)
+            if time.time() > deadline:
+                raise TimeoutError("Marty wouldn't stop moving. Are you also controlling it via another method?"
+                                   f"{os.linesep}If you issued some very long-running non-blocking commands, "
+                                   "try increasing `marty.client.max_blocking_wait_time` (the current value "
+                                   f"is {self.max_blocking_wait_time} s)")
+
+    def hello(self) -> bool:
+        return self.ricIF.cmdRICRESTRslt("traj/getReady")
+
+    def get_ready(self) -> bool:
+        return self.ricIF.cmdRICRESTRslt("traj/getReady")
+
+    def stand_straight(self, move_time: int = 2000) -> bool:
+        return self.ricIF.cmdRICRESTRslt(f"traj/standStraight?moveTime={move_time}")
+
+    def discover(self) -> List[str]:
+        return []
+
+    def stop(self, stop_type: str, stopCode: int) -> bool:
+        robotRestCmd = "stop"
+        trajCmd = ""
+        if stopCode == 0: robotRestCmd = "stopAfterMove"
+        elif stopCode == 2: robotRestCmd = "panic"
+        elif stopCode == 3: trajCmd = "getReady"
+        elif stopCode == 4 or stopCode == 5: robotRestCmd = "pause"
+        isOk = self.ricIF.cmdRICRESTRslt("robot/" + robotRestCmd)
+        if len(trajCmd) > 0:
+            self.ricIF.cmdRICRESTRslt("traj/" + trajCmd)
+        return isOk
+
+    def resume(self) -> bool:
+        return self.ricIF.cmdRICRESTRslt("robot/resume")
+
+    def hold_position(self, hold_time: int) -> bool:
+        return self.ricIF.cmdRICRESTRslt(f"traj/hold?moveTime={hold_time}")
+
+    def move_joint(self, joint_id: int, position: int, move_time: int) -> bool:
+        return self.ricIF.cmdRICRESTRslt(f"traj/joint?jointID={joint_id}&angle={position}&moveTime={move_time}")
+
+    def get_joint_position(self, joint_id: Union[int, str]) -> float:
+        return self.ricHardware.getServoPos(joint_id, self.ricHwElemsInfoByIDNo)
+
+    def get_joint_current(self, joint_id: Union[int, str]) -> float:
+        return self.ricHardware.getServoCurrent(joint_id, self.ricHwElemsInfoByIDNo)
+
+    def get_joint_status(self, joint_id: Union[int, str]) -> int:
+        return self.ricHardware.getServoFlags(joint_id, self.ricHwElemsInfoByIDNo)
+
+    def lean(self, direction: str, amount: Optional[int], move_time: int) -> bool:
+        if amount is None:
+            amount = 29
+        try:
+            directionNum = ClientGeneric.SIDE_CODES[direction]
+        except KeyError:
+            self.preException(True)
+            raise MartyCommandException("Direction must be one of {}, not '{}'"
+                                        "".format(set(ClientGeneric.SIDE_CODES.keys()), direction))
+        return self.ricIF.cmdRICRESTRslt(f"traj/lean?side={directionNum}&leanAngle={amount}&moveTime={move_time}")
+
+    def walk(self, num_steps: int = 2, start_foot:str = 'auto', turn: int = 0,
+                step_length:int = 25, move_time: int = 1500) -> bool:
+        side_url_param = ''
+        if start_foot != 'auto':
+            try:
+                sideNum = ClientGeneric.SIDE_CODES[start_foot]
+            except KeyError:
+                raise MartyCommandException("Direction must be one of {}, not '{}'"
+                                            "".format(set(ClientGeneric.SIDE_CODES.keys()), start_foot))
+            side_url_param = f'&side={sideNum}'
+        return self.ricIF.cmdRICRESTRslt(f"traj/step/{num_steps}?stepLength={step_length}&turn={turn}"
+                                         f"&moveTime={move_time}" + side_url_param)
+
+    def eyes(self, joint_id: int, pose_or_angle: Union[str, int], move_time: int = 100) -> bool:
+        if type(pose_or_angle) is str:
+            try:
+                eyesTrajectory = ClientGeneric.EYE_POSES[pose_or_angle]
+            except KeyError:
+                raise MartyCommandException("pose must be one of {}, not '{}'"
+                                            "".format(set(ClientGeneric.EYE_POSES.keys()), pose_or_angle))
+            return self.ricIF.cmdRICRESTRslt(f"traj/{eyesTrajectory}")
+        return self.move_joint(joint_id, pose_or_angle, move_time)
+
+    def kick(self, side: str = 'right', twist: int = 0, move_time: int = 2500) -> bool:
+        if side != 'right' and side != 'left':
+            raise MartyCommandException("side must be one of 'right' or 'left', not '{}'"
+                                        "".format(side))
+        return self.ricIF.cmdRICRESTRslt(f"traj/kick?side={ClientGeneric.SIDE_CODES[side]}&moveTime={move_time}&turn={twist}")
+
+    def arms(self, left_angle: int, right_angle: int, move_time: int) -> bool:
+        self.move_joint(6, left_angle, move_time)
+        return self.move_joint(7, right_angle, move_time)
+
+    def celebrate(self, move_time: int = 4000) -> bool:
+
+        # TODO - add celebrate trajectory to Marty V2
+        return self.ricIF.cmdRICRESTRslt(f"traj/wiggle?moveTime={move_time}")
+
+    def circle_dance(self, side: str = 'right', move_time: int = 2500) -> bool:
+        if side != 'right' and side != 'left':
+            raise MartyCommandException("side must be one of 'right' or 'left', not '{}'"
+                                        "".format(side))
+        return self.ricIF.cmdRICRESTRslt(f"traj/circle?side={ClientGeneric.SIDE_CODES[side]}&moveTime={move_time}")
+
+    def dance(self, side: str = 'right', move_time: int = 3000) -> bool:
+        if side != 'right' and side != 'left':
+            raise MartyCommandException("side must be one of 'right' or 'left', not '{}'"
+                                        "".format(side))
+        return self.ricIF.cmdRICRESTRslt(f"traj/dance?side={ClientGeneric.SIDE_CODES[side]}&moveTime={move_time}")
+
+    def wiggle(self, move_time: int = 4000) -> bool:
+        return self.ricIF.cmdRICRESTRslt(f"traj/wiggle?moveTime={move_time}")
+
+    def sidestep(self, side: str, steps: int = 1, step_length: int = 35,
+            move_time: int = 1000) -> bool:
+        if side != 'right' and side != 'left':
+            raise MartyCommandException("side must be one of 'right' or 'left', not '{}'"
+                                        "".format(side))
+        return self.ricIF.cmdRICRESTRslt(f"traj/sidestep/{steps}?side={ClientGeneric.SIDE_CODES[side]}"
+                                         f"&stepLength={step_length}&moveTime={move_time}")
+
+    def set_volume(self, volume: int) -> bool:
+        return self.ricIF.cmdRICRESTRslt(f"audio/vol/{volume}")
+
+    def get_volume(self) -> int:
+        result = self.ricIF.cmdRICRESTURLSync("audio/vol")
+        if result.get("rslt", "") == "ok":
+            return result.get("volPC", 0)
+        return 0
+
+    def play_sound(self, name_or_freq_start: Union[str,float],
+            freq_end: Optional[float] = None,
+            duration: Optional[int] = None) -> bool:
+        if name_or_freq_start.lower().endswith(".mp3"):
+            return self.ricIF.play_mp3(name_or_freq_start)
+        if not name_or_freq_start.lower().endswith(".raw"):
+            name_or_freq_start += ".raw"
+        return self.ricIF.cmdRICRESTRslt(f"filerun/{name_or_freq_start}")
+
+    def pinmode_gpio(self, gpio: int, mode: str) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def write_gpio(self, gpio: int, value: int) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def digitalread_gpio(self, gpio: int) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def i2c_write(self, *byte_array: int) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def i2c_write_to_ric(self, address: int, byte_array: bytes) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def get_battery_voltage(self) -> float:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def get_battery_remaining(self) -> float:
+        powerStatus = self.ricHardware.getPowerStatus()
+        return powerStatus.get("battRemainCapacityPercent", 0)
+
+    def get_distance_sensor(self) -> int:
+        for attached_add_on in self.get_add_ons_status().values():
+            if type(attached_add_on) == dict and attached_add_on['whoAmI'] == 'VCNL4200':
+                distance_bytes = attached_add_on['data'][1:3]
+                distance = int.from_bytes(distance_bytes, 'big')
+                return distance
+        return 0
+
+    def _index_data_color_ir(self, attached_add_on: str) -> Tuple[Tuple[int, int, int], str]:
+        '''
+        Parses data of passed-in color or IR sensor :two:
+        Args:
+            attached_add_on: Name of IR or color sensor add on
+        Returns:
+            A tuple with three integers of data (detection byte, obstacle value, ground value)
+            and a string of whether the sensor is a default 'left' or 'right' add on
+        '''
+        if attached_add_on['whoAmI'] == 'IRFoot':
+            detection_flags = attached_add_on['data'][1]
+            obstacle_data_raw = int.from_bytes(attached_add_on['data'][2:4], 'big')
+            ground_data_raw = int.from_bytes(attached_add_on['data'][4:6], 'big')
+            return (detection_flags, obstacle_data_raw, ground_data_raw), 'right'
+        if attached_add_on['whoAmI'] == 'coloursensor':
+            detection_flags = attached_add_on['data'][6]
+            obstacle_data_raw = int.from_bytes(attached_add_on['data'][8:10], 'big')
+            ground_data_raw = attached_add_on['data'][2]
+            return (detection_flags, obstacle_data_raw, ground_data_raw), 'left'
+
+    def _get_obstacle_and_ground_raw_data(self, add_on_or_side: str) -> list:
+        '''
+        Finds the wanted color or IR sensor and gets the parsed obstacle and ground data :two:
+        Args:
+            add_on_or_side: Takes in the name of a color sensor, name of an IR
+            sensor, `'left'` for the add on connected to the left foot,
+            or `'right'` for the add on connected to the right foot
+        Returns:
+            A tuple of the detection byte, obstacle reading, and ground reading of the add on
+        '''
+        sensor_whoamis = {'IRFoot', 'coloursensor'}
+        sensor_data = {'left': [], 'right': []}
+        sensor_possible_names = {
+            'left': ['LeftColorSensor', 'LeftIRFoot'],
+            'right': ['RightIRFoot', 'RightColorSensor']
+        }
+        addon_names = sensor_possible_names.get(add_on_or_side, [])
+
+        # There may be a situation just after connecting to RIC where publication messages from the addon
+        # have not yet been received so we need to wait for them to be received before we can parse them
+        for retryLoop in range(10):
+            addon_statuses = self.get_add_ons_status().values()
+            if len(addon_statuses) != 0:
+                break
+            time.sleep(0.1)
+
+        # Get the add-on values
+        for attached_add_on in addon_statuses:
+            if type(attached_add_on) == dict and attached_add_on.get('whoAmI','') in sensor_whoamis:
+                obstacle_and_ground_data, side = self._index_data_color_ir(attached_add_on)
+                if attached_add_on['name'] in addon_names:
+                    return obstacle_and_ground_data
+                else:
+                    sensor_data[side].append(obstacle_and_ground_data)
+        if len(sensor_data[add_on_or_side.lower()]) == 1:
+            return sensor_data[add_on_or_side.lower()][0]
+        elif add_on_or_side.lower() == 'left' or add_on_or_side.lower() == 'right':
+            raise MartyCommandException(
+                f"Marty could not find a {add_on_or_side} sensor. "
+                "Please make sure your add ons are plugged in and named correctly"
+            )
+        else:
+            raise MartyCommandException(
+                f"The add on '{add_on_or_side}' is not a valid add on for obstacle and ground sensing."
+                "Please make sure to pass in the name of an IR sensor or Color sensor."
+            )
+
+    def foot_on_ground(self, add_on_or_side: str) -> bool:
+        raw_data = self._get_obstacle_and_ground_raw_data(add_on_or_side)
+        if len(raw_data) > 0:
+            return (raw_data[0] & 0b10) == 0b00
+        return False
+
+    def foot_obstacle_sensed(self, add_on_or_side: str) -> bool:
+        raw_data = self._get_obstacle_and_ground_raw_data(add_on_or_side)
+        if len(raw_data) > 0:
+            return (raw_data[0] & 0b1) == 0b1
+        return False
+
+    def get_obstacle_sensor_reading(self, add_on_or_side: str) -> int:
+        raw_data = self._get_obstacle_and_ground_raw_data(add_on_or_side)
+        if len(raw_data) > 1:
+            return raw_data[1]
+        return 0
+
+    def get_ground_sensor_reading(self, add_on_or_side: str) -> int:
+        raw_data = self._get_obstacle_and_ground_raw_data(add_on_or_side)
+        if len(raw_data) > 2:
+            return raw_data[2]
+        return 0
+
+    def get_accelerometer(self, axis: Optional[str] = None, axisCode: int = 0) -> float:
+        if axis is None:
+            return self.ricHardware.getIMUAll()
+        return self.ricHardware.getIMUAxisValue(axisCode)
+
+    def enable_motors(self, enable: bool = True, clear_queue: bool = True) -> bool:
+        return True
+
+    def enable_safeties(self, enable: bool = True) -> bool:
+        return True
+
+    def fall_protection(self, enable: bool = True) -> bool:
+        return True
+
+    def motor_protection(self, enable: bool = True) -> bool:
+        return True
+
+    def battery_protection(self, enable: bool = True) -> bool:
+        return True
+
+    def buzz_prevention(self, enable: bool = True) -> bool:
+        return True
+
+    def lifelike_behaviour(self, enable: bool = True) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def set_parameter(self, *byte_array: int) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def save_calibration(self) -> bool:
+        return self.ricIF.cmdRICRESTRslt(f"calibrate/set")
+
+    def clear_calibration(self) -> bool:
+        return self.ricIF.cmdRICRESTRslt(f"calibrate/setFlag/0")
+
+    def is_calibrated(self) -> bool:
+        result = self.ricIF.cmdRICRESTURLSync("calibrate")
+        if result.get("rslt", "") == "ok":
+            return result.get("calDone", 0) != 0
+        return False
+
+    def ros_command(self, *byte_array: int) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def keyframe (self, time: float, num_of_msgs: int, msgs) -> List[bytes]:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def get_chatter(self) -> bytes:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def get_firmware_version(self) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def _mute_serial(self) -> bool:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def ros_serial_formatter(self, topicID: int, send: bool = False, *message: int) -> List[int]:
+        raise MartyCommandException(ClientGeneric.NOT_IMPLEMENTED)
+
+    def is_moving(self) -> bool:
+        return self.ricHardware.getIsMoving()
+
+    def is_paused(self) -> bool:
+        return self.ricHardware.getIsPaused()
+
+    def get_robot_status(self) -> Dict:
+        return self.ricHardware.getRobotStatus()
+
+    def get_joints(self) -> Dict:
+        return self.ricHardware.getServos(self.ricHwElemsInfoByIDNo)
+
+    def get_power_status(self) -> Dict:
+        return self.ricHardware.getPowerStatus()
+
+    def get_add_ons_status(self) -> Dict:
+        return self.ricHardware.getAddOns(self.ricHwElemsInfoByIDNo)
+
+    def get_add_on_status(self, add_on_name_or_id: Union[int, str]) -> Dict:
+        return self.ricHardware.getAddOn(add_on_name_or_id, self.ricHwElemsInfoByIDNo)
+
+    def add_on_query(self, add_on_name: str, data_to_write: bytes, num_bytes_to_read: int) -> Dict:
+        return self.ricIF.addOnQueryRaw(add_on_name, data_to_write, num_bytes_to_read)
+
+    def get_system_info(self) -> Dict:
+        return self.ricSystemInfo
+
+    def set_marty_name(self, name: str) -> bool:
+        escapedName = name.replace('"', '').replace('\n','')
+        return self.ricIF.cmdRICRESTRslt(f"friendlyname/{escapedName}")
+
+    def get_marty_name(self) -> str:
+        result = self.ricIF.cmdRICRESTURLSync("friendlyname")
+        if result.get("rslt", "") == "ok":
+            return result.get("friendlyName", "Marty")
+        return "Marty"
+
+    def is_marty_name_set(self) -> bool:
+        result = self.ricIF.cmdRICRESTURLSync("friendlyname")
+        if result.get("rslt", "") == "ok":
+            return result.get("friendlyNameIsSet", 0) != 0
+        return False
+
+    def get_hw_elems_list(self) -> List:
+        self._updateHwElemsInfo()
+        return self.ricHwElemsList
+
+    def send_ric_rest_cmd(self, ricRestCmd: str) -> None:
+        self.ricIF.sendRICRESTURL(ricRestCmd)
+
+    def send_ric_rest_cmd_sync(self, ricRestCmd: str) -> Dict:
+        return self.ricIF.cmdRICRESTURLSync(ricRestCmd)
+
+    def is_conn_ready(self) -> bool:
+        if not self.ricIF.isOpen():
+            return False
+        return self._initComplete and ((self.lastRICSerialMsgTime is not None) or (self.subscribeRateHz == 0) or (len(self.ricHwElemsList) < 10))
+
+    def _is_valid_disco_addon(self, add_on: str) -> bool:
+        disco_whoamis = {"LEDfoot", "LEDarm", "LEDeye"}
+        for attached_add_on in self.get_add_ons_status().values():
+            if type(attached_add_on) == dict and attached_add_on['name'] == add_on:
+                if attached_add_on['whoAmI'] in disco_whoamis:
+                    return True
+                else:
+                    raise MartyCommandException(f"The add on name: '{add_on}' is not a valid disco add on. "
+                                                "Please check the add on name in the scratch app -> configure -> add ons")
+        raise MartyCommandException(f"The add on name '{add_on}' is not a valid add on. Please check the add on "
+                                    "name in the scratch app -> configure -> add ons")
+
+    def disco_off(self, add_on: str) -> bool:
+        if self._is_valid_disco_addon(add_on):
+            response = self.add_on_query(add_on, bytes.fromhex('01'), 0)
+            return response.get("rslt", "") == "ok"
+
+    def disco_pattern(self, pattern: int, add_on: str) -> bool:
+        if pattern == 1:
+            pattern = '10'
+        elif pattern == 2:
+            pattern = '11'
+        else:
+            raise Exception("Pattern must be 1 or 2")
+        if self._is_valid_disco_addon(add_on):
+            response = self.add_on_query(add_on, bytes.fromhex(pattern), 0)
+            return response.get("rslt", "") == "ok"
+
+    def _region_to_bytes(self, region: Union[str, int]) -> bytes:
+        if region == 'all':
+            region = (2,)
+        else:
+            region = (4, region)
+        return bytes(region)
+
+    def _downscale_color(self, color: Union[tuple, bytes]):
+        return bytes(c//25 for c in color)
+
+    def _is_valid_color_hex(self, color_hex: str) -> bool:
+        hex_pattern = re.compile("^([A-Fa-f0-9]{6})$")
+        return bool(hex_pattern.match(color_hex))
+
+    def _parse_color_hex(self, color_hex: str, region: Union[str, int]) -> bytes:
+        input_color = color_hex
+        color_hex = color_hex.lstrip('#')
+        if self._is_valid_color_hex(color_hex):
+            color_bytes = bytes.fromhex(color_hex)
+        else:
+            raise MartyCommandException(f"The string '{input_color}' is not a valid hex color code or default color")
+        return color_bytes
+
+    def disco_color(self, color: Union[str, Tuple[int, int, int]], add_on: str, region: Union[int, str]) -> bool:
+        default_colors = {
+            'white'  : 'FFFFFF',
+            'red'    : 'FF0000',
+            'blue'   : '0000FF',
+            'yellow' : 'FFFF00',
+            'green'  : '008000',
+            'teal'   : '008080',
+            'pink'   : 'eb1362',
+            'purple' : '7800c8',
+            'orange' : '961900'
+        }
+        if type(color) is str:
+            color = default_colors.get(color.lower(), color)
+            color = self._parse_color_hex(color, region)
+        elif type(color) is tuple:
+            if len(color) != 3:
+                raise MartyCommandException(f'RGB tuple must be 3 numbers, instead of: {color}. Please enter a valid color.')
+        else:
+            raise MartyCommandException(f"Color must be of string or tuple form, not {type(color)}")
+        color = self._downscale_color(color)
+        region = self._region_to_bytes(region)
+        command = region + color
+        if self._is_valid_disco_addon(add_on):
+            response = self.add_on_query(add_on, command, 0)
+            return response.get("rslt", "") == "ok"
+
+    def disco_group_operation(self, disco_operation: Callable, whoamis: set, operation_kwargs: dict) -> bool:
+        '''
+        Calls disco operations in groups for multiple add ons :two:
+        Args:
+            disco_operation: function for disco add on
+            whoami_type_codes: the add ons that the function applies to
+            operation_kwargs: additional arguments that need to be passed into the operation
+        Returns:
+            True if Marty accepted all requests
+        '''
+        result = True
+        for attached_add_on in self.get_add_ons_status().values():
+            if type(attached_add_on) == dict and attached_add_on['whoAmI'] in whoamis:
+                addon_name = attached_add_on['name']
+                result = result and disco_operation(add_on=addon_name, **operation_kwargs)
+        return result
+
+    def register_logging_callback(self, loggingCallback: Callable[[str],None]) -> None:
+        '''
+        Register a callback function to be called on every log message from RIC.
+        Log messages are used mainly for debugging and error reporting.
+        Args:
+            messageCallback: a callback function (with one string argument - the log message)
+        Returns:
+            None
+        '''
+        self.loggingCallback = loggingCallback
+
+    def register_publish_callback(self, messageCallback: Callable[[int],None]) -> None:
+        '''
+        Register a callback function to be called on every message published by RIC.
+        RIC publishes information like the accelerometer and joint positions constantly.
+        If registered, the callback is called after the message is fully decoded, so a common
+        use-case is to check the topic (the int passed to the callback) to see if the information
+        is of interest (for example topic == Marty.PUBLISH_TOPIC_ACCELEROMETER if new accelerometer
+        data is available). Then get the changed information using the regular get_accelerometer method
+        (or get_joints, etc for other data).
+        Args:
+            messageCallback: a callback function (with one argument - the topic code of the published
+                    message) that will be called on every message published by RIC.
+        Returns:
+            None
+        '''
+        self.publishedMsgCallback = messageCallback
+
+    def register_report_callback(self, messageCallback: Callable[[str],None]) -> None:
+        '''
+        Register a callback function to be called on every report message recieved from RIC.
+        Report messages are used for alert conditions such as Falling, Over Current, etc.
+        The report message (passed in the callback function str) is a JSON string.
+        The elements of the JSON string include:
+            msgType: the type of report message (this will be "warn" for all alerts)
+            msgBody: the message text (this is "freeFallDet" or "overCurrentDet")
+            IDNo: the IDNo of the element that generated the report (the codes for these
+                are in the Marty.HW_ELEM_IDS dictionary but additional ones may appear if
+                add-ons create warnings - the IDNos of add-ons are not fixed numbers but you
+                can see the IDNo of add-ons by using the get_add_ons_status() method)
+        Args:
+            messageCallback: a callback function (with one string argument)
+                    that will be called on every message published by RIC.
+        Returns:
+            None
+        '''
+        self.reportMsgCallback = messageCallback
+
+    def get_interface_stats(self) -> Dict:
+        ricIFStats = self.ricIF.getStats()
+        publishInfo = self.ricHardware.getPublishStats()
+        ricIFStats.update(publishInfo)
+        return ricIFStats
+
+    def preException(self, isFatal: bool) -> None:
+        if isFatal:
+            self.ricIF.close()
+        logger.warning(f"Pre-exception isFatal {isFatal}")
+
+    def _rxDecodedMsg(self, decodedMsg: DecodedMsg, interface: RICInterface):
+        if decodedMsg.protocolID == RICProtocols.PROTOCOL_ROSSERIAL:
+            if self.DEBUG_RECEIVE_PUBLISHED_MSG:
+                logger.debug(f"ROSSERIAL message received {len(decodedMsg.payload)}")
+            self.lastRICSerialMsgTime = time.time()
+            if decodedMsg.payload:
+                RICROSSerial.decode(decodedMsg.payload, 0, self._rxPublishedMsg)
+        elif decodedMsg.protocolID == RICProtocols.PROTOCOL_RICREST:
+            if self.DEBUG_RECEIVE_RICREST_MSGS:
+                logger.debug(f"RICREST message received {decodedMsg.payload}")
+            # Callback for REPORT messages
+            if (self.reportMsgCallback is not None) and (decodedMsg.msgTypeCode == RICProtocols.MSG_TYPE_REPORT):
+                try:
+                    self.reportMsgCallback(decodedMsg.payload)
+                except:
+                    logger.exception("Report callback failed:")
+        else:
+            logger.info(f"RIC UNKNOWN message received {decodedMsg.payload}")
+            pass
+
+    def _rxPublishedMsg(self, topicID: int, payload: bytes):
+        # Decode the message
+        self.ricHardware.updateWithROSSerialMsg(topicID, payload)
+        # Callback on published messages
+        if self.publishedMsgCallback is not None:
+            try:
+                self.publishedMsgCallback(topicID)
+            except:
+                logger.exception("Publish callback failed:")
+
+    def _logDebugMsg(self, logMsg: str) -> None:
+        if self.loggingCallback:
+            try:
+                self.loggingCallback(logMsg)
+            except:
+                logger.exception("Logging callback failed:")
+
+    def _msgTimerCallback(self) -> None:
+        if self.isClosing:
+            return
+        self._subscribeToPubMessages(False)
+
+    def _getRICVersion(self) -> bool:
+        # Retries here to allow for baud-rate changes, etc
+        for retries in range(self._numHwStatusRetries):
+            # logger.debug(f"_getRICVersion attempt {retries+1}")
+            self.ricSystemInfo = self.ricIF.cmdRICRESTURLSync("v")
+            if self.ricSystemInfo.get("rslt", "") == "ok":
+                break
+        if self.DEBUG_GET_RIC_VERSION:
+            logger.debug(f"_getRICVersion rslt {self.ricSystemInfo.get('rslt', '')} self.ricSystemInfo {self.ricSystemInfo}")
+        return self.ricSystemInfo.get("rslt", "") == "ok"
+
+    def _updateHwElemsInfo(self):
+        hwElemsInfo = self.ricIF.cmdRICRESTURLSync("hwstatus")
+        if hwElemsInfo.get("rslt", "") == "ok":
+            self.ricHwElemsList = hwElemsInfo.get("hw", [])
+            self.ricHwElemsInfoByIDNo = {}
+            for el in self.ricHwElemsList:
+                if "IDNo" in el:
+                    self.ricHwElemsInfoByIDNo[el["IDNo"]] = el
+            if self.DEBUG_GET_HW_ELEMS_INFO:
+                logger.debug(f"_updateHwElemsInfo found {len(self.ricHwElemsList)} elems")
+
+    def get_test_output(self) -> dict:
+        return self.ricIF.getTestOutput()
+
+    def _systemVersionGtEq(self, compareToVersion):
+        if self.ricSystemInfo is None:
+            return False
+        versInfo = self.ricSystemInfo.get("SystemVersion","0.0.0")
+        return version.parse(versInfo) >= version.parse(compareToVersion)
+
+    def _subscribeToPubMessages(self, forceResubscribe: bool):
+        versOk = self._systemVersionGtEq(self._minSysVersForSubscribeAPI)
+        timeForSubscr = self.lastRICSerialMsgTime is None or time.time() > self.lastRICSerialMsgTime + self.maxTimeBetweenPubs
+        resubscrReqd = self.lastSubscrReqMsgTime is None or time.time() > self.lastSubscrReqMsgTime + self.minTimeBetweenSubReqs
+        if versOk and self._initComplete and self.subscribeRateHz != 0 and (forceResubscribe or (timeForSubscr and resubscrReqd)):
+            # Subscribe for publication messages
+            if self.DEBUG_SUBSCRIBE_TO_PUB_MSGS:
+                logger.debug(f"Subscribe to published messages")
+            self.ricIF.sendRICRESTCmdFrame('{"cmdName":"subscription","action":"update",' + \
+                            '"pubRecs":[' + \
+                                '{' + f'"name":"MultiStatus","rateHz":{self.subscribeRateHz},' + '}' + \
+                                '{"name":"PowerStatus","rateHz":1.0},' + \
+                                '{' + f'"name":"AddOnStatus","rateHz":{self.subscribeRateHz}' + '}' + \
+                            ']}')
+            self.lastSubscrReqMsgTime = time.time()
+
+    def _unsubscribeFromPubMessages(self):
+        # Send unsubscribe request
+        self.ricIF.sendRICRESTCmdFrame('{"cmdName":"subscription","action":"update",' + \
+            '"pubRecs":[' + \
+                '{"name":"MultiStatus","rateHz":0},' + \
+                '{"name":"PowerStatus","rateHz":0},' + \
+                '{"name":"AddOnStatus","rateHz":0}' + \
+            ']}')
+        # Allow message to be sent
+        time.sleep(0.5)
+
+    def _onReconnect(self):
+        self._subscribeToPubMessages(True)
+
+    def _sendFileProgressAdapter(self, fileSize: int, bytesSent: int,
+                progress_callback: Callable[[int, int, 'RICInterface'], bool] = None):
+        if self._sendFileProgressCB:
+            return self._sendFileProgressCB(fileSize, bytesSent)
+        return True
+
+    def send_file(self, filename: str,  
+                progress_callback: Callable[[int, int], bool] = None,
+                file_dest:str = "fs") -> bool:
+        self._sendFileProgressCB = progress_callback
+        return self.ricIF.sendFile(filename, self._sendFileProgressAdapter, file_dest)
+
+    def _playMP3ProgressAdapter(self, fileSize: int, bytesSent: int,
+                progress_callback: Callable[[int, int, 'RICInterface'], bool] = None):
+        if self._playMP3ProgressCB:
+            return self._playMP3ProgressCB(fileSize, bytesSent)
+        return True
+
+    def play_mp3(self, filename: str, 
+                progress_callback: Callable[[int, int], bool] = None) -> bool:
+        self._playMP3ProgressCB = progress_callback
+        return self.ricIF.streamSoundFile(filename, "streamaudio", self._playMP3ProgressAdapter)
+
+    def get_file_list(self) -> List[str]:
+        result = self.ricIF.cmdRICRESTURLSync("filelist", timeOutSecs=5)
+        if result.get("rslt", "") == "ok":
+            return result.get("files", [])
+        return []
+
+    def delete_file(self, filename: str) -> bool:
+        result = self.ricIF.cmdRICRESTURLSync(f"filedelete/local/{filename}", timeOutSecs=5)
+        return result.get("rslt", "") == "ok"
```

### Comparing `martypy-3.4.3/martypy/LikeHDLC.py` & `martypy-3.5.0/martypy/LikeHDLC.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,329 +1,329 @@
-'''
-HDLC-like communications
-'''
-
-__version__ = '0.7.0'
-
-import logging
-import struct
-import time
-from enum import Enum
-from typing import Callable, Union
-
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-class HDLCStats:
-    '''
-    HDLCStats - statistics on HDLC-like communication
-    '''
-    crcErrors = 0
-    framesRxOk = 0
-
-class HDLCState(Enum):
-    STATE_READ = 1
-    STATE_ESCAPE = 2
-
-# Frame
-class Frame(object):
-    '''
-    Frame - represents an encoded HDLC-like frame
-    '''
-    CRC16_LUT = [
-        0x0000, 0x1021, 0x2042, 0x3063, 0x4084, 0x50a5, 0x60c6, 0x70e7,
-        0x8108, 0x9129, 0xa14a, 0xb16b, 0xc18c, 0xd1ad, 0xe1ce, 0xf1ef,
-        0x1231, 0x0210, 0x3273, 0x2252, 0x52b5, 0x4294, 0x72f7, 0x62d6,
-        0x9339, 0x8318, 0xb37b, 0xa35a, 0xd3bd, 0xc39c, 0xf3ff, 0xe3de,
-        0x2462, 0x3443, 0x0420, 0x1401, 0x64e6, 0x74c7, 0x44a4, 0x5485,
-        0xa56a, 0xb54b, 0x8528, 0x9509, 0xe5ee, 0xf5cf, 0xc5ac, 0xd58d,
-        0x3653, 0x2672, 0x1611, 0x0630, 0x76d7, 0x66f6, 0x5695, 0x46b4,
-        0xb75b, 0xa77a, 0x9719, 0x8738, 0xf7df, 0xe7fe, 0xd79d, 0xc7bc,
-        0x48c4, 0x58e5, 0x6886, 0x78a7, 0x0840, 0x1861, 0x2802, 0x3823,
-        0xc9cc, 0xd9ed, 0xe98e, 0xf9af, 0x8948, 0x9969, 0xa90a, 0xb92b,
-        0x5af5, 0x4ad4, 0x7ab7, 0x6a96, 0x1a71, 0x0a50, 0x3a33, 0x2a12,
-        0xdbfd, 0xcbdc, 0xfbbf, 0xeb9e, 0x9b79, 0x8b58, 0xbb3b, 0xab1a,
-        0x6ca6, 0x7c87, 0x4ce4, 0x5cc5, 0x2c22, 0x3c03, 0x0c60, 0x1c41,
-        0xedae, 0xfd8f, 0xcdec, 0xddcd, 0xad2a, 0xbd0b, 0x8d68, 0x9d49,
-        0x7e97, 0x6eb6, 0x5ed5, 0x4ef4, 0x3e13, 0x2e32, 0x1e51, 0x0e70,
-        0xff9f, 0xefbe, 0xdfdd, 0xcffc, 0xbf1b, 0xaf3a, 0x9f59, 0x8f78,
-        0x9188, 0x81a9, 0xb1ca, 0xa1eb, 0xd10c, 0xc12d, 0xf14e, 0xe16f,
-        0x1080, 0x00a1, 0x30c2, 0x20e3, 0x5004, 0x4025, 0x7046, 0x6067,
-        0x83b9, 0x9398, 0xa3fb, 0xb3da, 0xc33d, 0xd31c, 0xe37f, 0xf35e,
-        0x02b1, 0x1290, 0x22f3, 0x32d2, 0x4235, 0x5214, 0x6277, 0x7256,
-        0xb5ea, 0xa5cb, 0x95a8, 0x8589, 0xf56e, 0xe54f, 0xd52c, 0xc50d,
-        0x34e2, 0x24c3, 0x14a0, 0x0481, 0x7466, 0x6447, 0x5424, 0x4405,
-        0xa7db, 0xb7fa, 0x8799, 0x97b8, 0xe75f, 0xf77e, 0xc71d, 0xd73c,
-        0x26d3, 0x36f2, 0x0691, 0x16b0, 0x6657, 0x7676, 0x4615, 0x5634,
-        0xd94c, 0xc96d, 0xf90e, 0xe92f, 0x99c8, 0x89e9, 0xb98a, 0xa9ab,
-        0x5844, 0x4865, 0x7806, 0x6827, 0x18c0, 0x08e1, 0x3882, 0x28a3,
-        0xcb7d, 0xdb5c, 0xeb3f, 0xfb1e, 0x8bf9, 0x9bd8, 0xabbb, 0xbb9a,
-        0x4a75, 0x5a54, 0x6a37, 0x7a16, 0x0af1, 0x1ad0, 0x2ab3, 0x3a92,
-        0xfd2e, 0xed0f, 0xdd6c, 0xcd4d, 0xbdaa, 0xad8b, 0x9de8, 0x8dc9,
-        0x7c26, 0x6c07, 0x5c64, 0x4c45, 0x3ca2, 0x2c83, 0x1ce0, 0x0cc1,
-        0xef1f, 0xff3e, 0xcf5d, 0xdf7c, 0xaf9b, 0xbfba, 0x8fd9, 0x9ff8,
-        0x6e17, 0x7e36, 0x4e55, 0x5e74, 0x2e93, 0x3eb2, 0x0ed1, 0x1ef0,
-        ]
-
-    DELIMITER_CODE_NON_ASCII = 0xE7
-    ESCAPE_CODE_NON_ASCII = 0xD7
-    DELIMITER_CODE_ASCII = 0x7E
-    ESCAPE_CODE_ASCII = 0x7D
-
-    def __init__(self, delimiterCode: int, escapeCode: int) -> None:
-        '''
-        Initialise Frame
-
-        Args:
-            delimiterCode (for HDLC frame start/end)
-            escapeCode (for HDLC escapes)
-
-        Returns:
-            None
-        '''
-        self.finished = False
-        self.error = False
-        self.state = HDLCState.STATE_READ
-        self.data = bytearray()
-        self.crc = bytearray()
-        self.reader = None
-        self.delimiterCode = delimiterCode
-        self.escapeCode = escapeCode
-
-    def __len__(self) -> int:
-        return len(self.data)
-
-    def addByte(self, b: int) -> None:
-        '''
-        Add byte to frame
-
-        Args:
-            b: byte to add
-
-        Returns:
-            None
-        '''
-        if b == self.escapeCode:
-            self.state = HDLCState.STATE_ESCAPE
-        elif self.state == HDLCState.STATE_ESCAPE:
-            self.state = HDLCState.STATE_READ
-            b = b ^ 0x20
-            self.data.append(b)
-        else:
-            self.data.append(b)
-
-    def finish(self) -> None:
-        '''
-        Complete frame creation - updates crc and data variables
-
-        Args:
-            none
-
-        Returns:
-            None
-        '''
-        self.crc = self.data[-2:]
-        self.data = self.data[:-2]
-        self.finished = True
-
-    def checkCRC(self) -> bool:
-        '''
-        Check the CRC received matches expected
-
-        Args:
-            none
-
-        Returns:
-            bool - False indicates CRC check failure
-        '''
-        res = bool(self.crc == LikeHDLC.calcCRC(self.data))
-        if not res:
-            logger.debug(f"invalid crc {self.crc} != {LikeHDLC.calcCRC(self.data)}")
-            self.error = True
-        return res
-        
-    def toString(self) -> str:
-        return self.data.decode('utf-8').rstrip('\0')
-
-# LikeHDLC
-class LikeHDLC:
-    '''
-    HDLC-like with encode and decode capabilities
-    To decode, construct LikeHDLC and supply onFrame callback -
-        then send data to decodeData() and onFrame
-        callback will be called for each frame decoded
-    To encode use class method encode()
-    The communications protocol is based on HDLC but with some simplifications:
-    - byte-wise only, escape codes can be modified from standard
-    - encoding and decoding only
-    '''
-    def __init__(self, 
-            onFrame: Callable[[Union[bytes, str]], None],
-            onError: Callable[[], None],
-            asciiEscapes: bool = False,
-            payloadsAreStrings: bool = False) -> None:
-        '''
-        Initialise LikeHDLC
-        Args:
-            onFrame: callback function (takes 1 parameter which is a received frame)
-            onError: callback function (0 parameters) when an error occurs
-            asciiEscapes: bool - use the standard HDLC escape codes (which are ASCII values)
-            payloadsAreStrings: bool - received frames are returned as strings (as opposed to bytes)
-        Returns:
-            None
-        '''
-        self.payloadsAreStrings = payloadsAreStrings
-        self.onFrame = onFrame
-        self.onError = onError
-        self.asciiEscapes = asciiEscapes
-        self.setAsciiEscapes(asciiEscapes)
-        self.clear()
-        self.clearStats()
-
-    def setAsciiEscapes(self, asciiEscapes: bool = False) -> None:
-        '''
-        Set HDLC delimiter and escape codes
-
-        Args:
-            asciiEscapes: use standard ASCII values
-
-        Returns:
-            None
-        '''
-        self.delimiterCode = Frame.DELIMITER_CODE_ASCII if asciiEscapes \
-                        else Frame.DELIMITER_CODE_NON_ASCII
-        self.escapeCode = Frame.ESCAPE_CODE_ASCII if asciiEscapes \
-                        else Frame.ESCAPE_CODE_NON_ASCII
-
-    def clear(self) -> None:
-        '''
-        Clear the frame buffer
-        Args:
-            none
-        Returns:
-            None
-        '''
-        self.currentFrame = None
-
-    def clearStats(self) -> None:
-        '''
-        Clear statistics on HDLC operation
-        Args:
-            none
-        Returns:
-            None
-        '''
-        self.stats = HDLCStats()
-
-    def decodeData(self, b: int) -> None:
-        '''
-        Add a byte to be decoded
-        Args:
-            b byte to add
-        Returns:
-            None
-        '''
-        if b < 0 or b > 255:
-            return
-        if b == self.delimiterCode:
-            # Start or End
-            if (self.currentFrame is None) or len(self.currentFrame) < 1:
-                # Start
-                self.currentFrame = Frame(self.delimiterCode, self.escapeCode)
-                # logger.debug(f"START time {time.time()}")
-            else:
-                # End
-                self.currentFrame.finish()
-                self.currentFrame.checkCRC()
-                # logger.debug(f"END time {time.time()}")
-        else:
-            if self.currentFrame is not None:
-                if not self.currentFrame.finished:
-                    # Add to current frame
-                    self.currentFrame.addByte(b)
-
-        # Validate and callback if finished
-        if (self.currentFrame is not None) and self.currentFrame.finished:
-            rxFrame = self.currentFrame
-            self.currentFrame = None
-            if not rxFrame.error:
-                # Success
-                if self.payloadsAreStrings:
-                    self.onFrame(rxFrame.toString())
-                else:
-                    self.onFrame(rxFrame.data)
-                self.stats.framesRxOk += 1
-            elif rxFrame.finished:
-                # Error
-                self.stats.crcErrors += 1
-                self.onError()
-
-    def getStats(self) -> HDLCStats:
-        '''
-        Get statistics on HDLC conversion
-
-        Args:
-            none
-
-        Returns:
-            HDLCStats object containing statistics
-        '''
-        return self.stats
-
-    @classmethod
-    def encode(cls, data: bytes, asciiEscapes: bool = False) -> bytes:
-        '''
-        Encode data into an HDLC-like frame
-
-        Args:
-            data: bytes representing the data
-
-        Returns:
-            bytes representing the frame
-        '''
-        delimiterCode = Frame.DELIMITER_CODE_ASCII if asciiEscapes \
-                    else Frame.DELIMITER_CODE_NON_ASCII
-        escapeCode = Frame.ESCAPE_CODE_ASCII if asciiEscapes \
-                    else Frame.ESCAPE_CODE_NON_ASCII
-        frame = bytearray()
-        frame.append(delimiterCode)
-        crc = cls.calcCRC(data)
-        data = data + crc
-        for byte in data:
-            if byte == delimiterCode or byte == escapeCode:
-                frame.append(escapeCode)
-                frame.append(byte ^ 0x20)
-            else:
-                frame.append(byte)
-        frame.append(delimiterCode)
-        return bytes(frame)
-
-    @classmethod
-    def calcCRC(cls, data: bytes) -> bytes:
-        '''
-        Calculate CRC-CCITT 16Bit check code
-        https://en.wikipedia.org/wiki/High-Level_Data_Link_Control
-
-        Args:
-            data: bytes representing the data
-
-        Returns:
-            bytes representing the checksum (2 bytes big-endian)
-        '''
-
-        crc = 0xffff
-        for c in data:
-            crc = ((crc<<8)&0xff00) ^ Frame.CRC16_LUT[((crc>>8)&0xff)^c]
-        return bytearray(struct.pack(">H", crc))
-
-    @classmethod
-    def toBytes(cls, data):
-        '''
-        Convert iterable data (list, etc) into bytes
-
-        Args:
-            data: the data to turn into bytes (1 byte is added per value)
-
-        Returns:
-            None
-        '''
-        return bytearray(data)
+'''
+HDLC-like communications
+'''
+
+__version__ = '0.7.0'
+
+import logging
+import struct
+import time
+from enum import Enum
+from typing import Callable, Union
+
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+class HDLCStats:
+    '''
+    HDLCStats - statistics on HDLC-like communication
+    '''
+    crcErrors = 0
+    framesRxOk = 0
+
+class HDLCState(Enum):
+    STATE_READ = 1
+    STATE_ESCAPE = 2
+
+# Frame
+class Frame(object):
+    '''
+    Frame - represents an encoded HDLC-like frame
+    '''
+    CRC16_LUT = [
+        0x0000, 0x1021, 0x2042, 0x3063, 0x4084, 0x50a5, 0x60c6, 0x70e7,
+        0x8108, 0x9129, 0xa14a, 0xb16b, 0xc18c, 0xd1ad, 0xe1ce, 0xf1ef,
+        0x1231, 0x0210, 0x3273, 0x2252, 0x52b5, 0x4294, 0x72f7, 0x62d6,
+        0x9339, 0x8318, 0xb37b, 0xa35a, 0xd3bd, 0xc39c, 0xf3ff, 0xe3de,
+        0x2462, 0x3443, 0x0420, 0x1401, 0x64e6, 0x74c7, 0x44a4, 0x5485,
+        0xa56a, 0xb54b, 0x8528, 0x9509, 0xe5ee, 0xf5cf, 0xc5ac, 0xd58d,
+        0x3653, 0x2672, 0x1611, 0x0630, 0x76d7, 0x66f6, 0x5695, 0x46b4,
+        0xb75b, 0xa77a, 0x9719, 0x8738, 0xf7df, 0xe7fe, 0xd79d, 0xc7bc,
+        0x48c4, 0x58e5, 0x6886, 0x78a7, 0x0840, 0x1861, 0x2802, 0x3823,
+        0xc9cc, 0xd9ed, 0xe98e, 0xf9af, 0x8948, 0x9969, 0xa90a, 0xb92b,
+        0x5af5, 0x4ad4, 0x7ab7, 0x6a96, 0x1a71, 0x0a50, 0x3a33, 0x2a12,
+        0xdbfd, 0xcbdc, 0xfbbf, 0xeb9e, 0x9b79, 0x8b58, 0xbb3b, 0xab1a,
+        0x6ca6, 0x7c87, 0x4ce4, 0x5cc5, 0x2c22, 0x3c03, 0x0c60, 0x1c41,
+        0xedae, 0xfd8f, 0xcdec, 0xddcd, 0xad2a, 0xbd0b, 0x8d68, 0x9d49,
+        0x7e97, 0x6eb6, 0x5ed5, 0x4ef4, 0x3e13, 0x2e32, 0x1e51, 0x0e70,
+        0xff9f, 0xefbe, 0xdfdd, 0xcffc, 0xbf1b, 0xaf3a, 0x9f59, 0x8f78,
+        0x9188, 0x81a9, 0xb1ca, 0xa1eb, 0xd10c, 0xc12d, 0xf14e, 0xe16f,
+        0x1080, 0x00a1, 0x30c2, 0x20e3, 0x5004, 0x4025, 0x7046, 0x6067,
+        0x83b9, 0x9398, 0xa3fb, 0xb3da, 0xc33d, 0xd31c, 0xe37f, 0xf35e,
+        0x02b1, 0x1290, 0x22f3, 0x32d2, 0x4235, 0x5214, 0x6277, 0x7256,
+        0xb5ea, 0xa5cb, 0x95a8, 0x8589, 0xf56e, 0xe54f, 0xd52c, 0xc50d,
+        0x34e2, 0x24c3, 0x14a0, 0x0481, 0x7466, 0x6447, 0x5424, 0x4405,
+        0xa7db, 0xb7fa, 0x8799, 0x97b8, 0xe75f, 0xf77e, 0xc71d, 0xd73c,
+        0x26d3, 0x36f2, 0x0691, 0x16b0, 0x6657, 0x7676, 0x4615, 0x5634,
+        0xd94c, 0xc96d, 0xf90e, 0xe92f, 0x99c8, 0x89e9, 0xb98a, 0xa9ab,
+        0x5844, 0x4865, 0x7806, 0x6827, 0x18c0, 0x08e1, 0x3882, 0x28a3,
+        0xcb7d, 0xdb5c, 0xeb3f, 0xfb1e, 0x8bf9, 0x9bd8, 0xabbb, 0xbb9a,
+        0x4a75, 0x5a54, 0x6a37, 0x7a16, 0x0af1, 0x1ad0, 0x2ab3, 0x3a92,
+        0xfd2e, 0xed0f, 0xdd6c, 0xcd4d, 0xbdaa, 0xad8b, 0x9de8, 0x8dc9,
+        0x7c26, 0x6c07, 0x5c64, 0x4c45, 0x3ca2, 0x2c83, 0x1ce0, 0x0cc1,
+        0xef1f, 0xff3e, 0xcf5d, 0xdf7c, 0xaf9b, 0xbfba, 0x8fd9, 0x9ff8,
+        0x6e17, 0x7e36, 0x4e55, 0x5e74, 0x2e93, 0x3eb2, 0x0ed1, 0x1ef0,
+        ]
+
+    DELIMITER_CODE_NON_ASCII = 0xE7
+    ESCAPE_CODE_NON_ASCII = 0xD7
+    DELIMITER_CODE_ASCII = 0x7E
+    ESCAPE_CODE_ASCII = 0x7D
+
+    def __init__(self, delimiterCode: int, escapeCode: int) -> None:
+        '''
+        Initialise Frame
+
+        Args:
+            delimiterCode (for HDLC frame start/end)
+            escapeCode (for HDLC escapes)
+
+        Returns:
+            None
+        '''
+        self.finished = False
+        self.error = False
+        self.state = HDLCState.STATE_READ
+        self.data = bytearray()
+        self.crc = bytearray()
+        self.reader = None
+        self.delimiterCode = delimiterCode
+        self.escapeCode = escapeCode
+
+    def __len__(self) -> int:
+        return len(self.data)
+
+    def addByte(self, b: int) -> None:
+        '''
+        Add byte to frame
+
+        Args:
+            b: byte to add
+
+        Returns:
+            None
+        '''
+        if b == self.escapeCode:
+            self.state = HDLCState.STATE_ESCAPE
+        elif self.state == HDLCState.STATE_ESCAPE:
+            self.state = HDLCState.STATE_READ
+            b = b ^ 0x20
+            self.data.append(b)
+        else:
+            self.data.append(b)
+
+    def finish(self) -> None:
+        '''
+        Complete frame creation - updates crc and data variables
+
+        Args:
+            none
+
+        Returns:
+            None
+        '''
+        self.crc = self.data[-2:]
+        self.data = self.data[:-2]
+        self.finished = True
+
+    def checkCRC(self) -> bool:
+        '''
+        Check the CRC received matches expected
+
+        Args:
+            none
+
+        Returns:
+            bool - False indicates CRC check failure
+        '''
+        res = bool(self.crc == LikeHDLC.calcCRC(self.data))
+        if not res:
+            logger.debug(f"invalid crc {self.crc} != {LikeHDLC.calcCRC(self.data)}")
+            self.error = True
+        return res
+        
+    def toString(self) -> str:
+        return self.data.decode('utf-8').rstrip('\0')
+
+# LikeHDLC
+class LikeHDLC:
+    '''
+    HDLC-like with encode and decode capabilities
+    To decode, construct LikeHDLC and supply onFrame callback -
+        then send data to decodeData() and onFrame
+        callback will be called for each frame decoded
+    To encode use class method encode()
+    The communications protocol is based on HDLC but with some simplifications:
+    - byte-wise only, escape codes can be modified from standard
+    - encoding and decoding only
+    '''
+    def __init__(self, 
+            onFrame: Callable[[Union[bytes, str]], None],
+            onError: Callable[[], None],
+            asciiEscapes: bool = False,
+            payloadsAreStrings: bool = False) -> None:
+        '''
+        Initialise LikeHDLC
+        Args:
+            onFrame: callback function (takes 1 parameter which is a received frame)
+            onError: callback function (0 parameters) when an error occurs
+            asciiEscapes: bool - use the standard HDLC escape codes (which are ASCII values)
+            payloadsAreStrings: bool - received frames are returned as strings (as opposed to bytes)
+        Returns:
+            None
+        '''
+        self.payloadsAreStrings = payloadsAreStrings
+        self.onFrame = onFrame
+        self.onError = onError
+        self.asciiEscapes = asciiEscapes
+        self.setAsciiEscapes(asciiEscapes)
+        self.clear()
+        self.clearStats()
+
+    def setAsciiEscapes(self, asciiEscapes: bool = False) -> None:
+        '''
+        Set HDLC delimiter and escape codes
+
+        Args:
+            asciiEscapes: use standard ASCII values
+
+        Returns:
+            None
+        '''
+        self.delimiterCode = Frame.DELIMITER_CODE_ASCII if asciiEscapes \
+                        else Frame.DELIMITER_CODE_NON_ASCII
+        self.escapeCode = Frame.ESCAPE_CODE_ASCII if asciiEscapes \
+                        else Frame.ESCAPE_CODE_NON_ASCII
+
+    def clear(self) -> None:
+        '''
+        Clear the frame buffer
+        Args:
+            none
+        Returns:
+            None
+        '''
+        self.currentFrame = None
+
+    def clearStats(self) -> None:
+        '''
+        Clear statistics on HDLC operation
+        Args:
+            none
+        Returns:
+            None
+        '''
+        self.stats = HDLCStats()
+
+    def decodeData(self, b: int) -> None:
+        '''
+        Add a byte to be decoded
+        Args:
+            b byte to add
+        Returns:
+            None
+        '''
+        if b < 0 or b > 255:
+            return
+        if b == self.delimiterCode:
+            # Start or End
+            if (self.currentFrame is None) or len(self.currentFrame) < 1:
+                # Start
+                self.currentFrame = Frame(self.delimiterCode, self.escapeCode)
+                # logger.debug(f"START time {time.time()}")
+            else:
+                # End
+                self.currentFrame.finish()
+                self.currentFrame.checkCRC()
+                # logger.debug(f"END time {time.time()}")
+        else:
+            if self.currentFrame is not None:
+                if not self.currentFrame.finished:
+                    # Add to current frame
+                    self.currentFrame.addByte(b)
+
+        # Validate and callback if finished
+        if (self.currentFrame is not None) and self.currentFrame.finished:
+            rxFrame = self.currentFrame
+            self.currentFrame = None
+            if not rxFrame.error:
+                # Success
+                if self.payloadsAreStrings:
+                    self.onFrame(rxFrame.toString())
+                else:
+                    self.onFrame(rxFrame.data)
+                self.stats.framesRxOk += 1
+            elif rxFrame.finished:
+                # Error
+                self.stats.crcErrors += 1
+                self.onError()
+
+    def getStats(self) -> HDLCStats:
+        '''
+        Get statistics on HDLC conversion
+
+        Args:
+            none
+
+        Returns:
+            HDLCStats object containing statistics
+        '''
+        return self.stats
+
+    @classmethod
+    def encode(cls, data: bytes, asciiEscapes: bool = False) -> bytes:
+        '''
+        Encode data into an HDLC-like frame
+
+        Args:
+            data: bytes representing the data
+
+        Returns:
+            bytes representing the frame
+        '''
+        delimiterCode = Frame.DELIMITER_CODE_ASCII if asciiEscapes \
+                    else Frame.DELIMITER_CODE_NON_ASCII
+        escapeCode = Frame.ESCAPE_CODE_ASCII if asciiEscapes \
+                    else Frame.ESCAPE_CODE_NON_ASCII
+        frame = bytearray()
+        frame.append(delimiterCode)
+        crc = cls.calcCRC(data)
+        data = data + crc
+        for byte in data:
+            if byte == delimiterCode or byte == escapeCode:
+                frame.append(escapeCode)
+                frame.append(byte ^ 0x20)
+            else:
+                frame.append(byte)
+        frame.append(delimiterCode)
+        return bytes(frame)
+
+    @classmethod
+    def calcCRC(cls, data: bytes) -> bytes:
+        '''
+        Calculate CRC-CCITT 16Bit check code
+        https://en.wikipedia.org/wiki/High-Level_Data_Link_Control
+
+        Args:
+            data: bytes representing the data
+
+        Returns:
+            bytes representing the checksum (2 bytes big-endian)
+        '''
+
+        crc = 0xffff
+        for c in data:
+            crc = ((crc<<8)&0xff00) ^ Frame.CRC16_LUT[((crc>>8)&0xff)^c]
+        return bytearray(struct.pack(">H", crc))
+
+    @classmethod
+    def toBytes(cls, data):
+        '''
+        Convert iterable data (list, etc) into bytes
+
+        Args:
+            data: the data to turn into bytes (1 byte is added per value)
+
+        Returns:
+            None
+        '''
+        return bytearray(data)
```

### Comparing `martypy-3.4.3/martypy/ProtocolOverAscii.py` & `martypy-3.5.0/martypy/ProtocolOverAscii.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-'''
-Implements a frame protocol on top of a standard ASCII interface
-'''
-class ProtocolOverAscii():
-    '''
-    ProtocolOverAscii
-    The main serial port on RIC (USB C connector) is used for plain-text logging AND control
-    This protocol makes that possible by assuming bit-7 of any plain-text would be 0 and then
-    condensing all control communications into the remaining (bit-7 == 1) values of each byte
-    '''
-    OVERASCII_ESCAPE_1 = 0x85
-    OVERASCII_ESCAPE_2 = 0x8E
-    OVERASCII_ESCAPE_3 = 0x8F
-    OVERASCII_MOD_CODE = 0x20
-
-    def __init__(self):
-        self.escapeSeqCode = 0
-
-    def decodeByte(self, ch: int) -> int:
-        '''
-        Function to handle char for decoding
-        Returns -1 if char was an escape code - remainder will be returned later
-        Args:
-            ch: byte to decode
-        Returns:
-            decoded byte or -1 if the byte was an escape code (see above)
-        '''
-        # Check if in escape sequence
-        if self.escapeSeqCode != 0:
-            prevEscCode = self.escapeSeqCode
-            self.escapeSeqCode = 0
-            if prevEscCode == 1:
-                return (ch ^ self.OVERASCII_MOD_CODE) & 0x7f
-            elif prevEscCode == 2:
-                return ch ^ self.OVERASCII_MOD_CODE
-            return ch
-        elif ch == self.OVERASCII_ESCAPE_1:
-            self.escapeSeqCode = 1
-            return -1
-        elif ch == self.OVERASCII_ESCAPE_2:
-            self.escapeSeqCode = 2
-            return -1
-        elif ch == self.OVERASCII_ESCAPE_3:
-            self.escapeSeqCode = 3
-            return -1
-        else:
-            return ch & 0x7f
-
-    @classmethod
-    def encode(cls, inData: bytes) -> bytes:
-        '''
-        Encode frame
-        Values 0x00-0x0F map to ESCAPE_CODE_1, VALUE_XOR_20H_AND_MSB_SET
-        Values 0x10-0x7f map to VALUE_WITH_MSB_SET
-        Values 0x80-0x8F map to ESCAPE_CODE_2, VALUE_XOR_20H
-        Values 0x90-0xff map to ESCAPE_CODE_3, VALUE
-        Value ESCAPE_CODE_1 maps to ESCAPE_CODE_1 + VALUE
-        Args:
-            inData: data to encode (bytes)
-        Returns:
-            encoded frame (bytes)
-        '''
-        # Iterate over frame
-        encodedFrame = bytearray()
-        for toEnc in inData:
-            # Handle escape chars
-            if toEnc <= 0x0f:
-                encodedFrame.append(ProtocolOverAscii.OVERASCII_ESCAPE_1)
-                encodedFrame.append((toEnc ^ ProtocolOverAscii.OVERASCII_MOD_CODE) | 0x80)
-            elif (toEnc >= 0x10) and (toEnc <= 0x7f):
-                encodedFrame.append(toEnc | 0x80)
-            elif (toEnc >= 0x80) and (toEnc <= 0x8f):
-                encodedFrame.append(ProtocolOverAscii.OVERASCII_ESCAPE_2)
-                encodedFrame.append(toEnc ^ ProtocolOverAscii.OVERASCII_MOD_CODE)
-            else:
-                encodedFrame.append(ProtocolOverAscii.OVERASCII_ESCAPE_3)
-                encodedFrame.append(toEnc)
-        return encodedFrame
+'''
+Implements a frame protocol on top of a standard ASCII interface
+'''
+class ProtocolOverAscii():
+    '''
+    ProtocolOverAscii
+    The main serial port on RIC (USB C connector) is used for plain-text logging AND control
+    This protocol makes that possible by assuming bit-7 of any plain-text would be 0 and then
+    condensing all control communications into the remaining (bit-7 == 1) values of each byte
+    '''
+    OVERASCII_ESCAPE_1 = 0x85
+    OVERASCII_ESCAPE_2 = 0x8E
+    OVERASCII_ESCAPE_3 = 0x8F
+    OVERASCII_MOD_CODE = 0x20
+
+    def __init__(self):
+        self.escapeSeqCode = 0
+
+    def decodeByte(self, ch: int) -> int:
+        '''
+        Function to handle char for decoding
+        Returns -1 if char was an escape code - remainder will be returned later
+        Args:
+            ch: byte to decode
+        Returns:
+            decoded byte or -1 if the byte was an escape code (see above)
+        '''
+        # Check if in escape sequence
+        if self.escapeSeqCode != 0:
+            prevEscCode = self.escapeSeqCode
+            self.escapeSeqCode = 0
+            if prevEscCode == 1:
+                return (ch ^ self.OVERASCII_MOD_CODE) & 0x7f
+            elif prevEscCode == 2:
+                return ch ^ self.OVERASCII_MOD_CODE
+            return ch
+        elif ch == self.OVERASCII_ESCAPE_1:
+            self.escapeSeqCode = 1
+            return -1
+        elif ch == self.OVERASCII_ESCAPE_2:
+            self.escapeSeqCode = 2
+            return -1
+        elif ch == self.OVERASCII_ESCAPE_3:
+            self.escapeSeqCode = 3
+            return -1
+        else:
+            return ch & 0x7f
+
+    @classmethod
+    def encode(cls, inData: bytes) -> bytes:
+        '''
+        Encode frame
+        Values 0x00-0x0F map to ESCAPE_CODE_1, VALUE_XOR_20H_AND_MSB_SET
+        Values 0x10-0x7f map to VALUE_WITH_MSB_SET
+        Values 0x80-0x8F map to ESCAPE_CODE_2, VALUE_XOR_20H
+        Values 0x90-0xff map to ESCAPE_CODE_3, VALUE
+        Value ESCAPE_CODE_1 maps to ESCAPE_CODE_1 + VALUE
+        Args:
+            inData: data to encode (bytes)
+        Returns:
+            encoded frame (bytes)
+        '''
+        # Iterate over frame
+        encodedFrame = bytearray()
+        for toEnc in inData:
+            # Handle escape chars
+            if toEnc <= 0x0f:
+                encodedFrame.append(ProtocolOverAscii.OVERASCII_ESCAPE_1)
+                encodedFrame.append((toEnc ^ ProtocolOverAscii.OVERASCII_MOD_CODE) | 0x80)
+            elif (toEnc >= 0x10) and (toEnc <= 0x7f):
+                encodedFrame.append(toEnc | 0x80)
+            elif (toEnc >= 0x80) and (toEnc <= 0x8f):
+                encodedFrame.append(ProtocolOverAscii.OVERASCII_ESCAPE_2)
+                encodedFrame.append(toEnc ^ ProtocolOverAscii.OVERASCII_MOD_CODE)
+            else:
+                encodedFrame.append(ProtocolOverAscii.OVERASCII_ESCAPE_3)
+                encodedFrame.append(toEnc)
+        return encodedFrame
```

### Comparing `martypy-3.4.3/martypy/RICCommsParams.py` & `martypy-3.5.0/martypy/RICCommsParams.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-'''
-Parameters used for communication
-'''
-class RICCommsParams:
-
-    def __init__(self, connParams: dict = {}, fileTransferParams: dict = {}) -> None:
-        self.connParams = connParams
-        self.fileTransferParams = fileTransferParams
-
-    @property
-    def conn(self) -> dict:
-        return self.connParams
-
-    @conn.setter
-    def conn(self, connParams: dict) -> None:
-        self.connParams = connParams
-
-    @property
-    def fileTransfer(self) -> dict:
-        return self.fileTransferParams
-
-    @fileTransfer.setter
-    def fileTransfer(self, fileTransferParams: dict) -> None:
-        self.fileTransferParams = fileTransferParams
+'''
+Parameters used for communication
+'''
+class RICCommsParams:
+
+    def __init__(self, connParams: dict = {}, fileTransferParams: dict = {}) -> None:
+        self.connParams = connParams
+        self.fileTransferParams = fileTransferParams
+
+    @property
+    def conn(self) -> dict:
+        return self.connParams
+
+    @conn.setter
+    def conn(self, connParams: dict) -> None:
+        self.connParams = connParams
+
+    @property
+    def fileTransfer(self) -> dict:
+        return self.fileTransferParams
+
+    @fileTransfer.setter
+    def fileTransfer(self, fileTransferParams: dict) -> None:
+        self.fileTransferParams = fileTransferParams
```

### Comparing `martypy-3.4.3/martypy/RICCommsSerial.py` & `martypy-3.5.0/martypy/RICCommsSerial.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,262 +1,270 @@
-'''
-Serial communications with a Robotical RIC
-'''
-import logging
-import serial
-from serial.serialutil import SerialException
-import serial.tools.list_ports
-from threading import Thread
-import time
-from typing import Dict, List
-from warnings import warn
-
-from .RICCommsBase import RICCommsBase
-from .LikeHDLC import LikeHDLC
-from .ProtocolOverAscii import ProtocolOverAscii
-from .Exceptions import MartyConnectException
-
-logger = logging.getLogger(__name__)
-
-
-class RICCommsSerial(RICCommsBase):
-    '''
-    RICCommsSerial
-    Provides a serial interface for RIC communications
-    '''
-    def __init__(self) -> None:
-        '''
-        Initialise RICCommsSerial
-        '''
-        super().__init__()
-        self._isOpen = False
-        self.serialReaderThread: Thread = None
-        self.serialDevice: serial.Serial = None
-        self.serialThreadEnabled = False
-        self._hdlc = LikeHDLC(self._onHDLCFrame, self._onHDLCError)
-        self.overAscii = False
-        self.serialLogLine = ""
-        self.serialPortErrors = 0
-        self.baudRateAlternates = [2000000, 115200]
-        self.curBaudRate = 0
-        self.baudRateCheckedOk = False
-        self.msgRespTimeoutSecs = 1.5
-        self.numMsgsTimedOutSinceRateChange = 0
-        self.numMsgsTimedOutBeforeRateChange = 1
-
-    def __del__(self) -> None:
-        '''
-        Destructor
-        '''
-        try:
-            self.close()
-        except:
-            pass
-
-    @classmethod
-    def detect_rics(cls) -> List[str]:
-        serial_ports = serial.tools.list_ports.comports()
-        possible_rics = [port.device for port in serial_ports
-                         if "CP210" in port.description]
-        return possible_rics
-
-    def isOpen(self) -> bool:
-        '''
-        Check if comms open
-        Returns:
-            True if comms open
-        '''
-        return self._isOpen
-
-    def open(self, openParams: Dict) -> bool:
-        '''
-        Open connection
-        Protocol can be plain (if the port is not used for any other purpose) or
-                 overascii (if the port is also used for logging information)
-        Args:
-            openParams: dict containing params used to open the connection, may include
-                        "serialPort" (will be auto-detected if missing/empty),
-                        "serialBaud",
-                        "ifType" == "plain" or "overascii",
-                        "asciiEscapes"
-        Returns:
-            True if open succeeded or already open
-        Throws:
-            MartyConnectException: if connection cannot be opened
-        '''
-        # Check not already open
-        if self._isOpen:
-            return True
-
-        # Get params
-        self.commsParams.conn = openParams
-        self.commsParams.fileTransfer = {"fileBlockMax": 5000, "fileXferSync": False}
-        serialPort = openParams.get("serialPort", "")
-        serialBaud = openParams.get("serialBaud", 2000000)
-        self.overAscii = openParams.get("ifType", "plain") != "plain"
-        if self.overAscii:
-            self.protocolOverAscii = ProtocolOverAscii()
-        hdlcAsciiEscapes = openParams.get("asciiEscapes", False)
-
-        # Detect serial port with correct chip code
-        rics = self.detect_rics()
-        if not serialPort:
-            if len(rics) == 0:
-                raise MartyConnectException(
-                    "No serial (COM) port provided and no Martys detected."
-                )
-            if len(rics) > 1:
-                warn(f"Multiple Martys detected ({rics}). Connecting to {rics[0]}.",
-                     stacklevel=0)
-            serialPort = rics[0]
-
-        # Try to open serial port
-        try:
-            self.baudRateCheckedOk = False
-            self.curBaudRate = serialBaud
-            self.serialDevice = serial.Serial(port=None, baudrate=serialBaud)
-            self.serialDevice.port = serialPort
-            self.serialDevice.rts = 0
-            self.serialDevice.dtr = 0
-            self.serialDevice.dsrdtr = False
-            self.serialDevice.open()
-        except Exception as excp:
-            error_message = f"Serial port problem on {self.serialDevice.port}. Try "\
-                            f"connecting to one of the following ports instead: {rics}"
-            raise MartyConnectException(error_message) from excp
-
-        # Configure HDLC
-        self._hdlc.setAsciiEscapes(hdlcAsciiEscapes)
-        
-        # Start receive loop
-        self.serialThreadEnabled = True
-        self.serialReaderThread = Thread(target=self._serialRxLoop)
-        self.serialReaderThread.daemon = True
-        self.serialReaderThread.start()
-        self._isOpen = True
-        return True
-
-    def close(self) -> None:
-        '''
-        Close serial port
-        '''
-        if not self._isOpen:
-            return
-        # Stop thread function
-        if self.serialReaderThread is not None:
-            self.serialThreadEnabled = False
-            time.sleep(0.01)
-            self.serialReaderThread.join()
-            self.serialReaderThread = None
-        # Close port
-        if self.serialDevice is not None:
-            self.serialDevice.close()
-            self.serialDevice = None
-        self._isOpen = False
-
-    def send(self, data: bytes) -> None:
-        '''
-        Send data to serial port
-        Args:
-            data: bytes to send on serial port
-        Returns:
-            none
-        Throws:
-            MartyConnectException: if the connection has an error
-        '''
-        # logger.debug(f"Sending to IF len {len(bytesToSend)} {str(bytesToSend)}")
-        hdlcEncoded = self._hdlc.encode(data)
-        try:
-            if self.overAscii:
-                encodedFrame = ProtocolOverAscii.encode(hdlcEncoded)
-                self._sendBytesToIF(encodedFrame)
-                # logger.debug(f"send {encodedFrame.hex()}")
-            else:
-                self._sendBytesToIF(hdlcEncoded)
-        except Exception as excp:
-            raise MartyConnectException("Serial send problem") from excp
-
-    def _serialRxLoop(self) -> None:
-        '''
-        Thread function used to process serial port data
-        '''
-        while self.serialThreadEnabled:
-            i = self.serialDevice.in_waiting
-            if i < 1:
-                time.sleep(0.001)
-                continue
-            byt = self.serialDevice.read(i)
-            for b in byt:
-                if self.overAscii:
-                    if b >= 128:
-                        decodedVal = self.protocolOverAscii.decodeByte(b)
-                        if decodedVal >= 0:
-                            # logger.debug(f"{decodedVal:02x}")
-                            self._hdlc.decodeData(decodedVal)
-                    else:
-                        if b == 0x0a:
-                            if self.logLineCB:
-                                self.logLineCB(self.serialLogLine)
-                            self.serialLogLine = ""
-                        else:
-                            self.serialLogLine += chr(b)
-                else:
-                    self._hdlc.decodeData(b)
-            # logger.debug(f"CommsSerial rx {byt.hex()}")
-        # logger.debug("Exiting serialRxLoop")
-
-    def _onHDLCFrame(self, frame: bytes) -> None:
-        if self.rxFrameCB is not None:
-            self.rxFrameCB(frame)
-
-    def _onHDLCError(self) -> None:
-        pass
-
-    def _sendBytesToIF(self, bytesToSend: bytes) -> None:
-        # logger.debug(f"Sending to IF len {len(bytesToSend)} {str(bytesToSend)}")
-        if not self._isOpen:
-            return
-        # logger.debug(f"CommsSerial sendBytesToIF {''.join('{:02x}'.format(x) for x in bytesToSend)}")
-        if self.serialDevice is not None:
-            try:
-                self.serialDevice.write(bytesToSend)
-            except SerialException as excp:
-                # The port has connected but now failing to send characters
-                # This may sort itself out or require user intervention
-                self.serialPortErrors += 1
-                pass
-
-    def getTestOutput(self) -> dict:
-        return {}
-
-    def getMsgRespTimeoutSecs(self, defaultValue):
-        '''
-        Get the timeout for a message response
-        '''
-        return self.msgRespTimeoutSecs
-
-    def hintMsgTimeout(self, numTimedOut):
-        '''
-        Hint that messages are timing out from upper layers
-        '''
-        # Check if we've already found the right baud rate
-        if not self.baudRateCheckedOk:
-            # Count failed messages since last rate change
-            self.numMsgsTimedOutSinceRateChange += numTimedOut
-            if self.numMsgsTimedOutSinceRateChange >= self.numMsgsTimedOutBeforeRateChange:
-                # Enough messages timed out since last rate change, so try next rate
-                self._skipToNextBaudRate()
-                self.numMsgsTimedOutSinceRateChange = 0
-                # Back off the next rate change by a factor of 2
-                self.numMsgsTimedOutBeforeRateChange *= 2
-
-    def _skipToNextBaudRate(self):
-        '''
-        Skip to the next baud rate in the list
-        '''
-        if self.curBaudRate in self.baudRateAlternates:
-            curBaudIdx = self.baudRateAlternates.index(self.curBaudRate)
-            self.curBaudRate = self.baudRateAlternates[(curBaudIdx + 1) % len(self.baudRateAlternates)]
-        else:
-            self.curBaudRate = self.baudRateAlternates[0]
-        self.serialDevice.baudrate = self.curBaudRate
-        logger.debug(f"_skipToNextBaudRate comms failing - changing baud-rate to {self.curBaudRate}")
+'''
+Serial communications with a Robotical RIC
+'''
+import logging
+import serial
+from serial.serialutil import SerialException
+import serial.tools.list_ports
+from threading import Thread
+import time
+from typing import Dict, List
+from warnings import warn
+
+from .RICCommsBase import RICCommsBase
+from .LikeHDLC import LikeHDLC
+from .ProtocolOverAscii import ProtocolOverAscii
+from .Exceptions import MartyConnectException
+
+logger = logging.getLogger(__name__)
+
+
+class RICCommsSerial(RICCommsBase):
+    '''
+    RICCommsSerial
+    Provides a serial interface for RIC communications
+    '''
+    def __init__(self) -> None:
+        '''
+        Initialise RICCommsSerial
+        '''
+        super().__init__()
+        self._isOpen = False
+        self.serialReaderThread: Thread = None
+        self.serialDevice: serial.Serial = None
+        self.serialThreadEnabled = False
+        self._hdlc = LikeHDLC(self._onHDLCFrame, self._onHDLCError)
+        self.overAscii = False
+        self.serialLogLine = ""
+        self.serialPortErrors = 0
+        self.baudRateAlternates = [115200, 2000000]
+        self.curBaudRate = 0
+        self.baudRateCheckedOk = False
+        self.msgRespTimeoutSecs = 1.5
+        self.numMsgsTimedOutSinceRateChange = 0
+        self.numMsgsTimedOutBeforeRateChange = 1
+        self.DEBUG_HDLC_RX = False
+        self.DEBUG_HDLC_TX = False
+
+    def __del__(self) -> None:
+        '''
+        Destructor
+        '''
+        try:
+            self.close()
+        except:
+            pass
+
+    @classmethod
+    def detect_rics(cls) -> List[str]:
+        serial_ports = serial.tools.list_ports.comports()
+        possible_rics = [port.device for port in serial_ports
+                         if "CP210" in port.description]
+        return possible_rics
+
+    def isOpen(self) -> bool:
+        '''
+        Check if comms open
+        Returns:
+            True if comms open
+        '''
+        return self._isOpen
+
+    def open(self, openParams: Dict) -> bool:
+        '''
+        Open connection
+        Protocol can be plain (if the port is not used for any other purpose) or
+                 overascii (if the port is also used for logging information)
+        Args:
+            openParams: dict containing params used to open the connection, may include
+                        "serialPort" (will be auto-detected if missing/empty),
+                        "serialBaud",
+                        "ifType" == "plain" or "overascii",
+                        "asciiEscapes"
+        Returns:
+            True if open succeeded or already open
+        Throws:
+            MartyConnectException: if connection cannot be opened
+        '''
+        # Check not already open
+        if self._isOpen:
+            return True
+
+        # Get params
+        self.commsParams.conn = openParams
+        self.commsParams.fileTransfer = {"fileBlockMax": 5000, "fileXferSync": False, "fileBatchAck": 1}
+        serialPort = openParams.get("serialPort", "")
+        serialBaud = openParams.get("serialBaud", 115200)
+        self.overAscii = openParams.get("ifType", "plain") != "plain"
+        if self.overAscii:
+            self.protocolOverAscii = ProtocolOverAscii()
+        hdlcAsciiEscapes = openParams.get("asciiEscapes", False)
+
+        # Detect serial port with correct chip code
+        rics = self.detect_rics()
+        if not serialPort:
+            if len(rics) == 0:
+                raise MartyConnectException(
+                    "No serial (COM) port provided and no Martys detected."
+                )
+            if len(rics) > 1:
+                warn(f"Multiple Martys detected ({rics}). Connecting to {rics[0]}.",
+                     stacklevel=0)
+            serialPort = rics[0]
+
+        # Try to open serial port
+        try:
+            self.baudRateCheckedOk = False
+            self.curBaudRate = serialBaud
+            self.serialDevice = serial.Serial(port=None, baudrate=serialBaud)
+            self.serialDevice.port = serialPort
+            self.serialDevice.rts = 0
+            self.serialDevice.dtr = 0
+            self.serialDevice.dsrdtr = False
+            self.serialDevice.open()
+        except Exception as excp:
+            error_message = f"Serial port problem on {self.serialDevice.port}. Try "\
+                            f"connecting to one of the following ports instead: {rics}"
+            raise MartyConnectException(error_message) from excp
+
+        # Configure HDLC
+        self._hdlc.setAsciiEscapes(hdlcAsciiEscapes)
+        
+        # Start receive loop
+        self.serialThreadEnabled = True
+        self.serialReaderThread = Thread(target=self._serialRxLoop)
+        self.serialReaderThread.daemon = True
+        self.serialReaderThread.start()
+        self._isOpen = True
+        return True
+
+    def close(self) -> None:
+        '''
+        Close serial port
+        '''
+        if not self._isOpen:
+            return
+        # Stop thread function
+        if self.serialReaderThread is not None:
+            self.serialThreadEnabled = False
+            time.sleep(0.01)
+            self.serialReaderThread.join()
+            self.serialReaderThread = None
+        # Close port
+        if self.serialDevice is not None:
+            self.serialDevice.close()
+            self.serialDevice = None
+        self._isOpen = False
+
+    def send(self, data: bytes) -> None:
+        '''
+        Send data to serial port
+        Args:
+            data: bytes to send on serial port
+        Returns:
+            none
+        Throws:
+            MartyConnectException: if the connection has an error
+        '''
+        if self.DEBUG_HDLC_TX:
+            logger.debug(f"Sending to IF len {len(bytes)} {bytes.hex()}")
+        hdlcEncoded = self._hdlc.encode(data)
+        try:
+            if self.overAscii:
+                encodedFrame = ProtocolOverAscii.encode(hdlcEncoded)
+                if self.DEBUG_HDLC_TX:
+                    logger.info(f"RICCommsSerial send encoded length {len(encodedFrame)} unencoded {data.hex() if len(data) < 20 else data.hex()[:20] + '...'}")
+                self._sendBytesToIF(encodedFrame)
+            else:
+                if self.DEBUG_HDLC_TX:
+                    logger.debug(f"RICCommsSerial sendRaw {encodedFrame.hex()}")
+                self._sendBytesToIF(hdlcEncoded)
+        except Exception as excp:
+            raise MartyConnectException("Serial send problem") from excp
+
+    def _serialRxLoop(self) -> None:
+        '''
+        Thread function used to process serial port data
+        '''
+        while self.serialThreadEnabled:
+            i = self.serialDevice.in_waiting
+            if i < 1:
+                time.sleep(0.001)
+                continue
+            byt = self.serialDevice.read(i)
+            for b in byt:
+                if self.overAscii:
+                    if b >= 128:
+                        decodedVal = self.protocolOverAscii.decodeByte(b)
+                        if decodedVal >= 0:
+                            # logger.debug(f"{decodedVal:02x}")
+                            self._hdlc.decodeData(decodedVal)
+                    else:
+                        if b == 0x0a:
+                            if self.logLineCB:
+                                self.logLineCB(self.serialLogLine)
+                            self.serialLogLine = ""
+                        else:
+                            self.serialLogLine += chr(b)
+                else:
+                    self._hdlc.decodeData(b)
+            # logger.debug(f"CommsSerial rx {byt.hex()}")
+        # logger.debug("Exiting serialRxLoop")
+
+    def _onHDLCFrame(self, frame: bytes) -> None:
+        if self.rxFrameCB is not None:
+            if self.DEBUG_HDLC_RX:
+                logger.debug(f"RICCommsSerial rx {len(frame)} {frame.hex()}")
+            self.rxFrameCB(frame)
+
+    def _onHDLCError(self) -> None:
+        pass
+
+    def _sendBytesToIF(self, bytesToSend: bytes) -> None:
+        # logger.debug(f"Sending to IF len {len(bytesToSend)} {str(bytesToSend)}")
+        if not self._isOpen:
+            return
+        # logger.debug(f"CommsSerial sendBytesToIF {''.join('{:02x}'.format(x) for x in bytesToSend)}")
+        if self.serialDevice is not None:
+            try:
+                self.serialDevice.write(bytesToSend)
+            except SerialException as excp:
+                # The port has connected but now failing to send characters
+                # This may sort itself out or require user intervention
+                self.serialPortErrors += 1
+                pass
+
+    def getTestOutput(self) -> dict:
+        return {}
+
+    def getMsgRespTimeoutSecs(self, defaultValue):
+        '''
+        Get the timeout for a message response
+        '''
+        return self.msgRespTimeoutSecs
+
+    def hintMsgTimeout(self, numTimedOut):
+        '''
+        Hint that messages are timing out from upper layers
+        '''
+        # Check if we've already found the right baud rate
+        if not self.baudRateCheckedOk:
+            # Count failed messages since last rate change
+            self.numMsgsTimedOutSinceRateChange += numTimedOut
+            if self.numMsgsTimedOutSinceRateChange >= self.numMsgsTimedOutBeforeRateChange:
+                # Enough messages timed out since last rate change, so try next rate
+                self._skipToNextBaudRate()
+                self.numMsgsTimedOutSinceRateChange = 0
+                # Back off the next rate change by a factor of 2
+                self.numMsgsTimedOutBeforeRateChange *= 2
+
+    def _skipToNextBaudRate(self):
+        '''
+        Skip to the next baud rate in the list
+        '''
+        if self.curBaudRate in self.baudRateAlternates:
+            curBaudIdx = self.baudRateAlternates.index(self.curBaudRate)
+            self.curBaudRate = self.baudRateAlternates[(curBaudIdx + 1) % len(self.baudRateAlternates)]
+        else:
+            self.curBaudRate = self.baudRateAlternates[0]
+        self.serialDevice.baudrate = self.curBaudRate
+        logger.info(f"_skipToNextBaudRate comms failing - changing baud-rate to {self.curBaudRate}")
```

### Comparing `martypy-3.4.3/martypy/RICCommsTest.py` & `martypy-3.5.0/martypy/RICCommsTest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-'''
-Test communications with a Robotical RIC
-'''
-from threading import Thread
-from typing import Callable, Dict, Union
-import serial
-import time
-import copy
-import logging
-from .RICCommsBase import RICCommsBase
-from .Exceptions import MartyConnectException
-
-logger = logging.getLogger(__name__)
-
-class RICCommsTest(RICCommsBase):
-    def __init__(self) -> None:
-        super().__init__()
-        self._isOpen = True
-        self.clearTestOutput()
-
-    def __del__(self) -> None:
-        try:
-            self.close()
-        except:
-            pass
-
-    def isOpen(self) -> bool:
-        return self._isOpen
-
-    def open(self, openParams: Dict) -> bool:
-        self.commsParams.conn = openParams
-        self.commsParams.fileTransfer = {"fileBlockMax": 5000, "fileXferSync": False}
-        return True
-
-    def close(self) -> None:
-        self._isOpen = False
-
-    def send(self, data: bytes) -> None:
-        self.outputInfo["buf"].append(data)
-
-    def getTestOutput(self) -> dict:
-        dictCopy = copy.deepcopy(self.outputInfo)
-        self.clearTestOutput()
-        return dictCopy
-
-    def clearTestOutput(self) -> None:
-        self.outputInfo: Dict[str, list] = {"buf":[]}
+'''
+Test communications with a Robotical RIC
+'''
+from threading import Thread
+from typing import Callable, Dict, Union
+import serial
+import time
+import copy
+import logging
+from .RICCommsBase import RICCommsBase
+from .Exceptions import MartyConnectException
+
+logger = logging.getLogger(__name__)
+
+class RICCommsTest(RICCommsBase):
+    def __init__(self) -> None:
+        super().__init__()
+        self._isOpen = True
+        self.clearTestOutput()
+
+    def __del__(self) -> None:
+        try:
+            self.close()
+        except:
+            pass
+
+    def isOpen(self) -> bool:
+        return self._isOpen
+
+    def open(self, openParams: Dict) -> bool:
+        self.commsParams.conn = openParams
+        self.commsParams.fileTransfer = {"fileBlockMax": 5000, "fileXferSync": False, "fileBatchAck": 1}
+        return True
+
+    def close(self) -> None:
+        self._isOpen = False
+
+    def send(self, data: bytes) -> None:
+        self.outputInfo["buf"].append(data)
+
+    def getTestOutput(self) -> dict:
+        dictCopy = copy.deepcopy(self.outputInfo)
+        self.clearTestOutput()
+        return dictCopy
+
+    def clearTestOutput(self) -> None:
+        self.outputInfo: Dict[str, list] = {"buf":[]}
```

### Comparing `martypy-3.4.3/martypy/RICCommsWiFi.py` & `martypy-3.5.0/martypy/RICCommsWiFi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,197 +1,202 @@
-'''
-WiFi communications with a Robotical RIC
-'''
-from threading import Thread
-from typing import Callable, Dict, Union
-import time
-import logging
-from .RICCommsBase import RICCommsBase
-from .LikeHDLC import LikeHDLC
-from .Exceptions import MartyConnectException
-from .WebSocket import WebSocket
-
-logger = logging.getLogger(__name__)
-#logger.setLevel(logging.DEBUG)
-
-class RICCommsWiFi(RICCommsBase):
-    '''
-    RICCommsWiFi
-    Provides an interface for RIC communications
-    '''
-    def __init__(self, onReconnect: Callable[[],None]) -> None:
-        '''
-        Initialise RICCommsWiFi
-        '''
-        super().__init__()
-        self._isOpen = False
-        self.webSocketThread: Thread = None
-        self.webSocket: WebSocket = None
-        self.webSocketThreadEnabled = False
-        self._hdlc = LikeHDLC(self._onHDLCFrame, self._onHDLCError)
-        self.socketErrors = 0
-        self._onReconnect = onReconnect
-
-    def __del__(self) -> None:
-        '''
-        Destructor
-        '''
-        try:
-            self.close()
-        except:
-            pass
-
-    def isOpen(self) -> bool:
-        '''
-        Check if comms open
-        Returns:
-            True if comms open
-        '''
-        return self._isOpen
-
-    def open(self, openParams: Dict) -> bool:
-        '''
-        Open connection
-        Args:
-            openParams: dict containing params used to open the connection, may include
-                        "ipAddrOrHostname", 
-                        "ipPort",
-                        "wsPath",
-                        "asciiEscapes",
-                        "autoReconnect"
-        Returns:
-            True if open succeeded or already open
-        Throws:
-            MartyConnectException: if a connection cannot be opened
-        '''
-        # Check not already open
-        if self._isOpen:
-            return True
-
-        # Get params
-        self.commsParams.conn = openParams
-        self.commsParams.fileTransfer = {"fileBlockMax": 5000, "fileXferSync": False}
-        ipAddrOrHostname = openParams.get("ipAddrOrHostname", "")
-        ipPort = openParams.get("ipPort", 80)
-        wsPath = openParams.get("wsPath", "/ws")
-        hdlcAsciiEscapes = openParams.get("asciiEscapes", False)
-        autoReconnect = openParams.get("autoReconnect", True)
-
-        # Validate
-        if len(ipAddrOrHostname) == 0:
-            return False
-
-        # Open websocket
-        try:
-            self.webSocket = WebSocket(self._onWSBinaryFrame, 
-                        self._onWSTextFrame, 
-                        self._onWSError, 
-                        self._onWSReconnect,
-                        ipAddrOrHostname, ipPort, wsPath,
-                        autoReconnect=autoReconnect)
-            self.webSocket.open()
-        except Exception as excp:
-            raise MartyConnectException("Websocket problem") from excp
-
-        # Configure HDLC
-        self._hdlc.setAsciiEscapes(hdlcAsciiEscapes)
-
-        # Start receive loop
-        self.webSocketThreadEnabled = True
-        self.webSocketThread = Thread(target=self._webSocketThreadFn)
-        self.webSocketThread.daemon = True
-        self.webSocketThread.start()
-        self._isOpen = True
-        return True
-
-    def close(self) -> None:
-        '''
-        Close connection
-        '''
-        if not self._isOpen:
-            return
-        # Stop thread function
-        if self.webSocketThread is not None:
-            self.webSocketThreadEnabled = False
-            time.sleep(0.01)
-            self.webSocketThread.join()
-            self.webSocketThread = None
-        # Close socket
-        if self.webSocket is not None:
-            self.webSocket.close()
-            self.webSocket = None
-        self._isOpen = False
-
-    def send(self, data: bytes) -> None:
-        '''
-        Send data
-        Args:
-            data: bytes to send
-        Returns:
-            none
-        Throws:
-            MartyConnectException: if the connection has an error
-        '''
-        # logger.debug(f"WiFi send len {len(data)} {''.join('{:02x}'.format(x) for x in data)}")
-        hdlcEncoded = self._hdlc.encode(data)
-        try:
-            self._sendBytesToIF(hdlcEncoded)
-        except Exception as excp:
-            raise MartyConnectException("Connection send problem") from excp
-
-    def _onHDLCFrame(self, frame: bytes) -> None:
-        if self.rxFrameCB is not None:
-            self.rxFrameCB(frame)
-        
-    def _onHDLCError(self) -> None:
-        pass
-        
-    def _sendBytesToIF(self, bytesToSend: bytes) -> None:
-        # logger.debug(f"Sending to IF len {len(bytesToSend)} {str(bytesToSend)}")
-        if not self._isOpen:
-            return
-        # logger.debug(f"CommsWiFi sendBytesToIF {''.join('{:02x}'.format(x) for x in bytesToSend)}")
-        if self.webSocket is not None:
-            try:
-                self.webSocket.writeBinary(bytesToSend)
-            except Exception as excp:
-                # The socket has connected but now failing to send characters
-                # This may sort itself out or require user intervention
-                self.socketErrors += 1
-                pass
-
-    def _webSocketThreadFn(self) -> None:
-        '''
-        Thread function used to process websocket data
-        '''
-        while self.webSocketThreadEnabled:
-            try:
-                self.webSocket.service()
-            except OSError as excp:
-                logger.debug(f"webSocket problem {excp}")
-                self.webSocketThreadEnabled = False
-            except Exception as excp:
-                logger.debug(f"WebSocket exception {excp}")
-            time.sleep(0.001)
-        logger.debug("Exiting WebSocket thread")
-        self._isOpen = False
-
-    def _onWSBinaryFrame(self, rxFrame: bytes) -> None:
-        # logger.debug(f"webSocketRx {rxFrame.hex()}")
-        for rxByte in rxFrame:
-            self._hdlc.decodeData(rxByte)
-
-    def _onWSTextFrame(self, rxFrame: str) -> None:
-        logger.debug(f"webSocketRx TEXT UNEXPECTED {rxFrame}")
-
-    def _onWSError(self, err: str) -> None:
-        logger.debug(f"CommsWiFi WS error {err}")
-
-    def _onWSReconnect(self) -> None:
-        # logger.debug(f"CommsWiFi WS reconnect")
-        self._hdlc.clear()
-        if self._onReconnect:
-            self._onReconnect()
-
-    def getTestOutput(self) -> dict:
-        return {}
+'''
+WiFi communications with a Robotical RIC
+'''
+from threading import Thread
+from typing import Callable, Dict, Union
+import time
+import logging
+from .RICCommsBase import RICCommsBase
+from .LikeHDLC import LikeHDLC
+from .Exceptions import MartyConnectException
+from .WebSocket import WebSocket
+
+logger = logging.getLogger(__name__)
+#logger.setLevel(logging.DEBUG)
+
+class RICCommsWiFi(RICCommsBase):
+    '''
+    RICCommsWiFi
+    Provides an interface for RIC communications
+    '''
+    def __init__(self, onReconnect: Callable[[],None]) -> None:
+        '''
+        Initialise RICCommsWiFi
+        '''
+        super().__init__()
+        self._isOpen = False
+        self.webSocketThread: Thread = None
+        self.webSocket: WebSocket = None
+        self.webSocketThreadEnabled = False
+        self._hdlc = LikeHDLC(self._onHDLCFrame, self._onHDLCError)
+        self.socketErrors = 0
+        self._onReconnect = onReconnect
+        # Debug
+        self.DEBUG_WEBSOCKET_CONNECT = False
+
+    def __del__(self) -> None:
+        '''
+        Destructor
+        '''
+        try:
+            self.close()
+        except:
+            pass
+
+    def isOpen(self) -> bool:
+        '''
+        Check if comms open
+        Returns:
+            True if comms open
+        '''
+        return self._isOpen
+
+    def open(self, openParams: Dict) -> bool:
+        '''
+        Open connection
+        Args:
+            openParams: dict containing params used to open the connection, may include
+                        "ipAddrOrHostname", 
+                        "ipPort",
+                        "wsPath",
+                        "asciiEscapes",
+                        "autoReconnect"
+        Returns:
+            True if open succeeded or already open
+        Throws:
+            MartyConnectException: if a connection cannot be opened
+        '''
+        # Check not already open
+        if self._isOpen:
+            return True
+
+        # Get params
+        self.commsParams.conn = openParams
+        self.commsParams.fileTransfer = {"fileBlockMax": 5000, "fileXferSync": False, "fileBatchAck": 10}
+        ipAddrOrHostname = openParams.get("ipAddrOrHostname", "")
+        ipPort = openParams.get("ipPort", 80)
+        wsPath = openParams.get("wsPath", "/ws")
+        hdlcAsciiEscapes = openParams.get("asciiEscapes", False)
+        autoReconnect = openParams.get("autoReconnect", True)
+
+        # Validate
+        if len(ipAddrOrHostname) == 0:
+            return False
+
+        # Open websocket
+        try:
+            debugStartTime = time.time()
+            self.webSocket = WebSocket(self._onWSBinaryFrame, 
+                        self._onWSTextFrame, 
+                        self._onWSError, 
+                        self._onWSReconnect,
+                        ipAddrOrHostname, ipPort, wsPath,
+                        autoReconnect=autoReconnect)
+            self.webSocket.open()
+            if self.DEBUG_WEBSOCKET_CONNECT:
+                logger.debug(f"WebSocket open took {time.time() - debugStartTime}")
+        except Exception as excp:
+            raise MartyConnectException("Websocket problem") from excp
+
+        # Configure HDLC
+        self._hdlc.setAsciiEscapes(hdlcAsciiEscapes)
+
+        # Start receive loop
+        self.webSocketThreadEnabled = True
+        self.webSocketThread = Thread(target=self._webSocketThreadFn)
+        self.webSocketThread.daemon = True
+        self.webSocketThread.start()
+        self._isOpen = True
+        return True
+
+    def close(self) -> None:
+        '''
+        Close connection
+        '''
+        if not self._isOpen:
+            return
+        # Stop thread function
+        if self.webSocketThread is not None:
+            self.webSocketThreadEnabled = False
+            time.sleep(0.01)
+            self.webSocketThread.join()
+            self.webSocketThread = None
+        # Close socket
+        if self.webSocket is not None:
+            self.webSocket.close()
+            self.webSocket = None
+        self._isOpen = False
+
+    def send(self, data: bytes) -> None:
+        '''
+        Send data
+        Args:
+            data: bytes to send
+        Returns:
+            none
+        Throws:
+            MartyConnectException: if the connection has an error
+        '''
+        # logger.debug(f"WiFi send len {len(data)} {''.join('{:02x}'.format(x) for x in data)}")
+        hdlcEncoded = self._hdlc.encode(data)
+        try:
+            self._sendBytesToIF(hdlcEncoded)
+        except Exception as excp:
+            raise MartyConnectException("Connection send problem") from excp
+
+    def _onHDLCFrame(self, frame: bytes) -> None:
+        if self.rxFrameCB is not None:
+            self.rxFrameCB(frame)
+        
+    def _onHDLCError(self) -> None:
+        pass
+        
+    def _sendBytesToIF(self, bytesToSend: bytes) -> None:
+        # logger.debug(f"Sending to IF len {len(bytesToSend)} {str(bytesToSend)}")
+        if not self._isOpen:
+            return
+        # logger.debug(f"CommsWiFi sendBytesToIF {''.join('{:02x}'.format(x) for x in bytesToSend)}")
+        if self.webSocket is not None:
+            try:
+                self.webSocket.writeBinary(bytesToSend)
+            except Exception as excp:
+                # The socket has connected but now failing to send characters
+                # This may sort itself out or require user intervention
+                self.socketErrors += 1
+                pass
+
+    def _webSocketThreadFn(self) -> None:
+        '''
+        Thread function used to process websocket data
+        '''
+        while self.webSocketThreadEnabled:
+            try:
+                self.webSocket.service()
+            except OSError as excp:
+                logger.debug(f"webSocket problem {excp}")
+                self.webSocketThreadEnabled = False
+            except Exception as excp:
+                logger.debug(f"WebSocket exception {excp}")
+            time.sleep(0.001)
+        logger.debug("Exiting WebSocket thread")
+        self._isOpen = False
+
+    def _onWSBinaryFrame(self, rxFrame: bytes) -> None:
+        # logger.debug(f"webSocketRx {rxFrame.hex()}")
+        for rxByte in rxFrame:
+            self._hdlc.decodeData(rxByte)
+
+    def _onWSTextFrame(self, rxFrame: str) -> None:
+        logger.debug(f"webSocketRx TEXT UNEXPECTED {rxFrame}")
+
+    def _onWSError(self, err: str) -> None:
+        logger.debug(f"CommsWiFi WS error {err}")
+
+    def _onWSReconnect(self) -> None:
+        # logger.debug(f"CommsWiFi WS reconnect")
+        self._hdlc.clear()
+        if self._onReconnect:
+            self._onReconnect()
+
+    def getTestOutput(self) -> dict:
+        return {}
```

### Comparing `martypy-3.4.3/martypy/RICInterface.py` & `martypy-3.5.0/martypy/RICInterface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,692 +1,757 @@
-'''
-RICInterface
-'''
-from typing import Callable, Dict, Union, Optional
-import time
-import threading
-import logging
-import json
-import os
-from .RICProtocols import DecodedMsg, RICProtocols
-from .RICCommsBase import RICCommsBase
-from .RateAverager import RateAverager
-from .ValueAverager import ValueAverager
-from .Exceptions import MartyTransferException
-
-logger = logging.getLogger(__name__)
-
-class RICInterface:
-    '''
-    RICInterface
-    '''
-    def __init__(self, commsHandler: RICCommsBase) -> None:
-        '''
-        Initialise RICInterface
-        '''
-        self.commsHandler = commsHandler
-        self.ricProtocols = RICProtocols()
-        self.decodedMsgCB = None
-        self.logLineCB = None
-        # Message command/response matching
-        self.msgTimerCB = None
-        self._msgsOutstanding: Dict = {}
-        self._msgsOutstandingLock = threading.Lock()
-        self.msgRespTimeoutSecs = 1.5
-        # AddOn QueryRaw message matching
-        self._rawQueryOutstanding: Dict = {}
-        self._rawQueryOutstandingLock = threading.Lock()
-        self._rawQueryMsgKey = 1
-        # Stats
-        self.msgRxRate = RateAverager()
-        self.msgTxRate = RateAverager()
-        self.roundTripInfo = ValueAverager()
-        self.statsMatched = 0
-        self.statsUnMatched = 0
-        self.statsUnNumbered = 0
-        self.statsTimedOut = 0
-        self.uploadBytesPerSec = ValueAverager()
-        # File send vars
-        self._fileOTAStartFailed = False
-        self._fileOTAStartedOK = False
-        self._fileNotStarted = False
-        self._fileUserCancel = False
-        self._fileSendOkTo = 0
-        self._fileSendNewOkTo = False
-        self._fileFailedInFirmware = False
-        self.BLOCK_ACK_TIMEOUT = 15
-        self.BATCH_RETRY_MAX = 3
-
-    def __del__(self) -> None:
-        self.commsHandler.close()
-
-    def open(self, openParams: Dict) -> bool:
-        '''
-        Open interface to RIC
-        Args:
-            openParams: dict containing params used to open the connection
-                    (see RICCommsBase and derived classes for details)
-        Returns:
-            True if open succeeded or port is already open
-        Throws:
-            SerialException: if the serial port cannot be opened
-        '''
-        self.commsHandler.setRxFrameCB(self._onRxFrameCB)
-        self.commsHandler.setRxLogLineCB(self._onLogLineCB)
-        openOk = self.commsHandler.open(openParams)
-
-        # Set default timeout based on interface
-        self.msgRespTimeoutSecs = self.commsHandler.getMsgRespTimeoutSecs(self.msgRespTimeoutSecs)
-
-        # Start timer to check message completion
-        self.msgTimeoutCheckTimer = threading.Timer(1.0, self._msgTimeoutCheck)
-        self.msgTimeoutCheckTimer.daemon = True
-        self.msgTimeoutCheckTimer.start()
-        return openOk
-
-    def close(self) -> None:
-        '''
-        Close interface to RIC
-        Args:
-            none
-        Returns:
-            None
-        '''
-        self.commsHandler.close()
-
-    def isOpen(self) -> None:
-        return self.commsHandler.isOpen()
-
-    def setDecodedMsgCB(self, onDecodedMsg: Callable[[DecodedMsg, 'RICInterface'], None]) -> None:
-        '''
-        Set callback on decoded message received from RIC
-        Args:
-            cb: callback function (takes 2 parameters: decoded message and this object)
-        Returns:
-            None
-        '''
-        self.decodedMsgCB = onDecodedMsg
-
-    def setLogLineCB(self, onLogLine: Callable[[str], None]) -> None:
-        '''
-        Set callback on logging line received
-        Args:
-            onLogLine: callback function (takes 1 parameter which is the line of logging information)
-        Returns:
-            None
-        '''
-        self.logLineCB = onLogLine
-
-    def setTimerCB(self, onMsgTimerCB: Callable[[], None]) -> None:
-        '''
-        Set callback which can be used to check for message types (e.g. publish)
-        Args:
-            onMsgTimerCB: callback function (takes 0 parameters)
-        Returns:
-            None
-        '''
-        self.msgTimerCB = onMsgTimerCB
-
-    def sendRICRESTURL(self, msg: str, timeOutSecs: Optional[float] = None) -> bool:
-        '''
-        Send RICREST URL message
-        Args:
-            msg: string containing command URL
-            timeOutSecs: message time-out override in seconds (or None to use default)
-        Returns:
-            True if message sent
-        '''
-        ricRestMsg, msgNum = self.ricProtocols.encodeRICRESTURL(msg)
-        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
-        with self._msgsOutstandingLock:
-            self._msgsOutstanding[msgNum] = {"timeSent": time.time(), "timeOutSecs": timeOutSecs}
-        # logger.debug(f"sendRICRESTURL msgNum {msgNum} time {time.time()} msg {msg}")
-        self.commsHandler.send(ricRestMsg)
-        self.msgTxRate.addSample()
-        return True
-
-    def cmdRICRESTURLSync(self, msg: str, timeOutSecs: Optional[float] = None) -> Dict:
-        '''
-        Send RICREST URL message and wait for response
-        Args:
-            msg: string containing command URL
-            timeOutSecs: message time-out override in seconds (or None to use default)
-        Returns:
-            Response turned into a dictionary (from JSON)
-        '''
-        ricRestMsg, msgNum = self.ricProtocols.encodeRICRESTURL(msg)
-        # logger.debug(f"msgNum {msgNum} msg {msg}")
-        msgSendTime = time.time()
-        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
-        # logger.debug(f"cmdRICRESTURLSync msgNum {msgNum} timeout {timeOutSecs} msg {msg}")
-        with self._msgsOutstandingLock:
-            self._msgsOutstanding[msgNum] = {"timeSent": msgSendTime, "timeOutSecs": timeOutSecs, "awaited":True}
-        self.commsHandler.send(ricRestMsg)
-        self.msgTxRate.addSample()
-        # Wait for result
-        while time.time() < msgSendTime + timeOutSecs:
-            with self._msgsOutstandingLock:
-                # Should be an outstanding message - if not there's a problem
-                if msgNum not in self._msgsOutstanding:
-                    logger.debug(f"sendRICRESTURLSync msgNum {msgNum} not in _msgsOutstanding")
-                    return {"rslt":"failResponse"}
-                # Check if response received
-                if self._msgsOutstanding[msgNum].get("respValid", False):
-                    try:
-                        # Get response
-                        respStr = self._msgsOutstanding[msgNum].get("resp", None)
-                        respObj = {}
-                        if respStr:
-                            respObj = json.loads(respStr.payload.rstrip('\0'))
-                        debugMsgRespTime = self._msgsOutstanding[msgNum].get("respTime", 0)
-                        # logger.debug(f"sendRICRESTURLSync msgNum {msgNum} msg {msg} resp {json.dumps(respObj)} sendTime {msgSendTime} respTime {debugMsgRespTime}")
-                        return respObj
-                    except Exception as excp:
-                        logger.warn(f"sendRICRESTURLSync msgNum {msgNum} response is not JSON {excp}")
-            time.sleep(0.01)
-        # Debug - if we get here we timed out
-        logger.debug(f"sendRICRESTURLSync msgNum {msgNum} failTimeout")
-        return {"rslt":"failTimeout"}
-
-    def cmdRICRESTRslt(self, msg: str, timeOutSecs: Optional[float] = None) -> bool:
-        '''
-        Send RICREST URL message and wait for response
-        Args:
-            msg: string containing command URL
-            timeOutSecs: message time-out override in seconds (or None to use default)
-        Returns:
-            Response turned into a dictionary (from JSON)
-        '''
-        response = self.cmdRICRESTURLSync(msg, timeOutSecs)
-        return response.get("rslt", "") == "ok"
-
-    def sendRICRESTCmdFrame(self, msg: Union[str,bytes], 
-                    payload: Union[bytes, str, None] = None, timeOutSecs: Optional[float] = None) -> bool:
-        '''
-        Send RICREST command frame message
-        Args:
-            msg: string or bytes containing command frame
-            payload: optional payload
-            timeOutSecs: message time-out override in seconds (or None to use default)
-        Returns:
-            True if message sent
-        '''
-        ricRestMsg, msgNum = self.ricProtocols.encodeRICRESTCmdFrame(msg, payload)
-        # logger.debug(f"sendRICRESTCmdFrame msgNum {msgNum} len {len(ricRestMsg)} msg {msg}")
-        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
-        with self._msgsOutstandingLock:
-            self._msgsOutstanding[msgNum] = {"timeSent": time.time(), "timeOutSecs": timeOutSecs}
-        self.commsHandler.send(ricRestMsg)
-        self.msgTxRate.addSample()
-        return True
-
-    def sendRICRESTCmdFrameSync(self, msg: Union[str,bytes], 
-                    payload: Union[bytes, str] = None,
-                    timeOutSecs: Optional[float] = None) -> Dict:
-        '''
-        Send RICREST command frame message and wait for response
-        Args:
-            msg: string or bytes containing command frame
-            payload: optional payload
-            timeOutSecs: message time-out override in seconds (or None to use default)
-        Returns:
-            Response turned into a dictionary (from JSON)
-        '''
-        # Encode frame
-        ricRestMsg, msgNum = self.ricProtocols.encodeRICRESTCmdFrame(msg, payload)
-        # logger.debug(f"sendRICRESTCmdFrameSync msgNum {msgNum} len {len(ricRestMsg)} msg {msg}")
-        msgSendTime = time.time()
-        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
-        with self._msgsOutstandingLock:
-            self._msgsOutstanding[msgNum] = {"timeSent": msgSendTime, "timeOutSecs": timeOutSecs, "awaited":True}
-        self.commsHandler.send(ricRestMsg)
-        self.msgTxRate.addSample()
-        # Wait for result
-        while time.time() < msgSendTime + timeOutSecs:
-            logger.debug(f"sendRICRESTCmdFrameSync while loop")
-            with self._msgsOutstandingLock:
-                # Should be an outstanding message - if not there's a problem
-                if msgNum not in self._msgsOutstanding:
-                    return {"rslt":"failResponse"}
-                # Check if response received
-                if self._msgsOutstanding[msgNum].get("respValid", False):
-                    try:
-                        # Get response
-                        respStr = self._msgsOutstanding[msgNum].get("resp", None)
-                        respObj = {}
-                        if respStr:
-                            respObj = json.loads(respStr.payload.rstrip('\0'))
-                        debugMsgRespTime = self._msgsOutstanding[msgNum].get("respTime", 0)
-                        # logger.debug(f"sendRICRESTCmdFrameSync msgNum {msgNum} msg {msg} resp {json.dumps(respObj)} sendTime {msgSendTime} respTime {debugMsgRespTime}")
-                        return respObj
-                    except Exception as excp:
-                        logger.debug(f"msgNum {msgNum} response is not JSON {excp}", )
-            time.sleep(0.01)
-        logger.debug(f"sendRICRESTCmdFrameSync msgNum {msgNum} msg {msg} sendTime {msgSendTime} timeNow {time.time()} timeout {timeOutSecs}")
-        return {"rslt":"failTimeout"}
-
-    def sendRICRESTFileBlock(self, data: bytes) -> bool:
-        '''
-        Send RICREST file block
-        Args:
-            data: bytes of file data
-        Returns:
-            True if message sent
-        '''
-        ricRestMsg, _ = self.ricProtocols.encodeRICRESTFileBlock(data)
-        # logger.debug(f"sendRICRESTFileBlock msgNum {msgNum} len {len(ricRestMsg)}")
-        self.commsHandler.send(ricRestMsg)
-        self.msgTxRate.addSample()
-        return True
-
-    def newRoundTrip(self, rtTime:int) -> None:
-        '''
-        Indicate a new round-trip for a message is complete - this is
-        for statistics gathering
-        Args:
-            rtTime: time taken for round-trip in seconds
-        Returns:
-            None
-        '''
-        self.roundTripInfo.add(rtTime)
-        # logger.debug(f"RTTime {self.roundTripInfo.getAvg()}")
-
-    def sendTestMsgs(self, numMsgs:int, bytesPerMsg: int) -> None:
-        '''
-        Send a batch of test messages
-        Args:
-            numMsgs: number of messages to send
-            bytesPerMsg: bytes in each message
-        Returns:
-            None
-        '''
-        dataBlock = bytearray(bytesPerMsg)
-        for i in range(numMsgs):
-            self.commsHandler.send(dataBlock)
-            self.msgTxRate.addSample()
-
-    def _sendFileProgressCheckAbort(self, progressCB: Callable[[int, int, 'RICInterface'], bool], 
-                    currentPos: int, fileSize: int) -> bool:
-        if self._fileOTAStartFailed or self._fileNotStarted or self._fileUserCancel or self._fileFailedInFirmware:
-            return True
-        if not progressCB:
-            return False
-        if not progressCB(currentPos, fileSize, self):
-            self.sendRICRESTCmdFrameSync('{"cmdName":"ufCancel"}')
-            return True
-        return False
-
-    def sendFile(self, filename: str, fileDest: str, reqStr: str = '', 
-                progressCB: Callable[[int, int, 'RICInterface'], bool] = None) -> bool:
-        '''
-        Send a file (from the file system)
-        Args:
-            filename: name of file to send
-            fileDest: "fs" to upload to file system, "ricfw" for new RIC firmware
-            reqStr: API request used for transfer, if left blank this is inferred from fileDest, other
-                    values include "fileupload" and "espfwupdate" - see RIC documentation for API
-            progressCB: callback used to indicate how file send is progressing, callable takes three params
-                    which are bytesSent, totalBytes and the interface to RIC (of type RICInterface) and
-                    returns a bool which should be True to continue the file upload or False to abort
-        Returns:
-            True if operation succeeded
-        Throws:
-            OSError: operating system exceptions
-            May throw other exceptions so include a general exception handler
-        '''
-        # Send new firmware in the bin folder using the CommandHandler protocol
-        with open(filename, "rb") as f:
-
-            # Read firmware
-            binaryImage = f.read()
-            binaryImageLen = len(binaryImage)
-            # logger.debug(f"File {filename} is {binaryImageLen} bytes long")
-
-            # Check if we're uploading firmware
-            isFirmware = fileDest == "ricfw"
-            if reqStr == '':
-                reqStr = 'espfwupdate' if isFirmware else 'fileupload'
-            uploadName = "fw" if isFirmware else os.path.basename(filename)
-            self._fileOTAStartFailed = False
-            self._fileOTAStartedOK = False
-            self._fileNotStarted = False
-            self._fileUserCancel = False
-            self._fileFailedInFirmware = False
-
-            # Frames follow the approach used in the web interface start, block..., end
-            resp = self.sendRICRESTCmdFrameSync('{' + f'"cmdName":"ufStart","reqStr":"{reqStr}","fileType":"{fileDest}",' + \
-                            f'"fileName":"{uploadName}","fileLen":{str(binaryImageLen)}' + '}', 
-                            timeOutSecs = 10)
-            if resp.get("rslt","") != "ok":
-                raise MartyTransferException("File transfer start not acknowledged")
-
-            # Block and batch sizes
-            blockMaxSize = self.commsHandler.commsParams.fileTransfer.get("fileBlockMax", 5000)
-            blockMaxSize = resp.get("batchMsgSize", blockMaxSize)
-            batchAckSize = resp.get("batchAckSize", 50)
-            self._fileSendOkTo = 0
-
-            # Debug
-            # logger.debug(f"ricIF sendFile blockMaxSize {blockMaxSize} batchAckSize {batchAckSize} resp {resp}")
-
-            # Progress and check for abort
-            if self._sendFileProgressCheckAbort(progressCB, self._fileSendOkTo, binaryImageLen):
-                return False
-
-            # Wait for a period depending on whether we're sending firmware - this is because starting
-            # a firmware update involves the ESP32 in a long-running activity and the firmware becomes
-            # unresponsive during this time
-            if isFirmware:
-                for i in range(5):
-                    time.sleep(1)
-                    if self._sendFileProgressCheckAbort(progressCB, 0, binaryImageLen):
-                        return False
-                    if self._fileOTAStartedOK:
-                        break
-
-            # Debug
-            # logger.debug(f"ricIF sendFile starting to send file data ...")
-
-            # Send file blocks
-            numBlocks = 0
-            batchRetryCount = 0
-            while self._fileSendOkTo < binaryImageLen:
-
-                # NOTE: first batch MUST be of size 1 (not batchAckSize) because RIC performs a long-running
-                # blocking task immediately after receiving the first message in a firmware
-                # update - although this could be relaxed for non-firmware update file uploads
-                sendFromPos = self._fileSendOkTo
-                batchStartPos = self._fileSendOkTo
-                batchStartTime = time.time()
-                batchSize = 1 if sendFromPos == 0 else batchAckSize
-                batchBlockIdx = 0
-                self._fileSendNewOkTo = False
-                while batchBlockIdx < batchSize and sendFromPos < binaryImageLen:
-
-                    # Send block
-                    blockToSend = binaryImage[sendFromPos:sendFromPos+blockMaxSize]
-                    self.sendRICRESTFileBlock(sendFromPos.to_bytes(4, 'big') + blockToSend)
-                    sendFromPos += blockMaxSize
-                    batchBlockIdx += 1
-
-                    # Check if we have received an error
-                    if self._fileNotStarted or self._fileUserCancel or self._fileFailedInFirmware:
-                        break
-
-                # Debug
-                # logger.debug(f"ricIF sendFile sent batch - start at {batchStartPos} end at {sendFromPos} okto {self._fileSendOkTo}")
-
-                # Wait for response (there is a timeout at the ESP end to ensure a response is always returned
-                # even if blocks are dropped on reception at ESP) - the timeout here is for these responses
-                # being dropped
-                timeNow = time.time()
-                while time.time() - timeNow < self.BLOCK_ACK_TIMEOUT:
-                    # Progress update
-                    if self._sendFileProgressCheckAbort(progressCB, self._fileSendOkTo, binaryImageLen):
-                        return False
-
-                    # Debug
-                    # logger.debug(f"ricIF sendFile checking for OKTO {self._fileSendOkTo} batchStartPos {batchStartPos}")
-
-                    # Check for okto
-                    if self._fileSendNewOkTo:
-                        batchRetryCount = 0
-                        # Update stats
-                        if self._fileSendOkTo > batchStartPos:
-                            batchBytesPerSec = (self._fileSendOkTo - batchStartPos) / (time.time() - batchStartTime)
-                            self.uploadBytesPerSec.add(batchBytesPerSec)
-                        break
-
-                    # Wait
-                    time.sleep(1)
-
-                # Check if no okto has been received with a greater position than batchStartPos
-                if self._fileSendOkTo <= batchStartPos:
-                    batchRetryCount += 1
-                    if batchRetryCount > self.BATCH_RETRY_MAX:
-                        return False
-
-                # Block count
-                numBlocks += 1
-
-            # Debug
-            # logger.debug(f"ricIF sendFile sending END")
-
-            # End frame
-            resp = self.sendRICRESTCmdFrameSync('{' + f'"cmdName":"ufEnd","reqStr":"fileupload","fileType":"{fileDest}",' + \
-                            f'"fileName":"{filename}","fileLen":{str(binaryImageLen)},' + \
-                            f'"blockCount":{str(numBlocks)}' + '}', 
-                            timeOutSecs = 5)
-            if resp.get("rslt","") != "ok":
-                return False
-            return True
-
-    def getStats(self) -> Dict:
-        return {
-            "roundTripAvgMS":self.roundTripInfo.getAvg()*1000,
-            "msgRxRatePS":self.msgRxRate.getAvg(),
-            "msgTxRatePS":self.msgTxRate.getAvg(),
-            "unmatched":self.statsUnMatched,
-            "matched":self.statsMatched,
-            "unnumbered":self.statsUnNumbered,
-            "timedOut":self.statsTimedOut,
-            "uploadBPS":self.uploadBytesPerSec.getAvg(),
-            "rxCount":self.msgRxRate.getTotal(),
-            "txCount":self.msgTxRate.getTotal(),
-        }
-
-    def addOnQueryRaw(self, addOnName: str, dataToWrite: bytes, numBytesToRead: int,
-                        timeOutSecs: Optional[float] = None) -> Dict:
-        '''
-        Write and read an addOn directly (raw-mode)
-        Args:
-            addOnName, name of the addOn (see get_add_ons_status() at the top level or response to
-                addon/list REST API command)
-            dataToWrite, can be zero length if nothing is to be written, the first byte will generally
-                be the register or opcode of the addOn
-            numBytesToRead: number of bytes to read from the device - can be zero
-            timeOutSecs: message time-out override in seconds (or None to use default)
-        Returns:
-            Dict with keys including:
-                "rslt" - the result which will be "ok" if the query succeeded
-                "dataRead" - the data read from the addOn
-        '''
-        # Handle msgKey
-        msgKey = self._rawQueryMsgKey
-        self._rawQueryMsgKey += 1
-        if self._rawQueryMsgKey > 99999:
-            self._rawQueryMsgKey = 1
-
-        # Form command
-        hexWrStr = dataToWrite.hex()
-        ricRestCmd = f"elem/{addOnName}/json?cmd=raw&hexWr={hexWrStr}&numToRd={numBytesToRead}&msgKey={msgKey}"
-
-        # Register in raw message matching
-        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
-        with self._rawQueryOutstandingLock:
-            self._rawQueryOutstanding[msgKey] = {"timeSent": time.time(), "timeOutSecs": timeOutSecs, "awaited":True}
-
-        # Send message
-        resp = self.cmdRICRESTURLSync(ricRestCmd)
-        resp["dataRead"] = b""
-        if resp.get("rslt", "") != "ok":
-            self._rawQueryOutstanding.pop(msgKey)
-            return resp
-
-        # Wait for a report message generated by the addOn access process
-        msgSendTime = time.time()
-        while time.time() < msgSendTime + timeOutSecs:
-            with self._rawQueryOutstandingLock:
-                # Should be an outstanding message - if not there's a problem
-                if msgKey not in self._rawQueryOutstanding:
-                    resp["rslt"] = "failReport"
-                    return resp
-                # Check if a report received
-                if self._rawQueryOutstanding[msgKey].get("reptValid", False):
-                    # Get report
-                    reptObj = self._rawQueryOutstanding[msgKey].get("reptObj", {})
-                    # logger.debug(f"msgKey {msgKey} msg {ricRestCmd} rept {json.dumps(reptObj)} sendTime {msgSendTime}")
-                    resp["dataRead"] = reptObj.get("hexRd", b"")
-                    return resp
-            time.sleep(0.01)
-        return {"rslt":"failTimeout"}
-
-    def _onRxFrameCB(self, frame: bytes) -> None:
-        self.msgRxRate.addSample()
-        decodedMsg = self.ricProtocols.decodeRICFrame(frame)
-        # logger.debug(f"_onRxFrameCB len {len(frame)} msgNum {decodedMsg.msgNum} type {decodedMsg.msgTypeCode} data {frame.hex()}")
-        # if decodedMsg.protocolID != RICProtocols.PROTOCOL_ROSSERIAL:
-        #     logger.debug(f"_onRxFrameCB {decodedMsg.toString()}")
-        doRxCallback = True
-        if decodedMsg.msgNum != 0:
-            # Numbered message - this is the response to a REST API command
-            # logger.debug(f"_onRxFrameCB msgNum {decodedMsg.msgNum} {decodedMsg.payload}")
-            isUnmatched = False
-            with self._msgsOutstandingLock:
-                if decodedMsg.msgNum in self._msgsOutstanding:
-                    msgRec = self._msgsOutstanding[decodedMsg.msgNum]
-                    roundTripTime = time.time() - msgRec["timeSent"]
-                    self.newRoundTrip(roundTripTime)
-                    if not msgRec.get("awaited", False):
-                        self._msgsOutstanding.pop(decodedMsg.msgNum)
-                    else:
-                        msgRec["resp"] = decodedMsg
-                        msgRec["respValid"] = True
-                        msgRec["respTime"] = time.time()
-                    self.statsMatched += 1
-                else:
-                    isUnmatched = True
-                    self.statsUnMatched += 1
-            if isUnmatched:
-                logger.warn(f"_onRxFrameCB Unmatched msgNum {decodedMsg.msgNum}")
-            doRxCallback = isUnmatched
-        else:
-            # logger.debug(f"_onRxFrameCB unnumbered restType {decodedMsg.restType} msgType {decodedMsg.msgTypeCode}")
-            if decodedMsg.msgTypeCode == RICProtocols.MSG_TYPE_REPORT:
-                # Report message - this can include results of accessing addOns
-                # logger.debug(f"_onRxFrameCB REPORT {decodedMsg.payload}")
-                reptObj = {}
-                try:
-                    reptObj = json.loads(decodedMsg.payload.rstrip('\0'))
-                except Exception as excp:
-                    logger.warn(f"_onRxFrameCB REPORT is not JSON {excp}")
-                msgKey = reptObj.get("msgKey", '')
-                if type(msgKey) is str:
-                    try:
-                        msgKey = int(msgKey)
-                    except:
-                        msgKey = 0
-                if msgKey != 0:
-                    isUnmatched = False
-                    with self._rawQueryOutstandingLock:
-                        if msgKey in self._rawQueryOutstanding:
-                            msgRec = self._rawQueryOutstanding[msgKey]
-                            if not msgRec.get("awaited", False):
-                                self._rawQueryOutstanding.pop(msgKey)
-                            else:
-                                msgRec["reptObj"] = reptObj
-                                msgRec["reptValid"] = True
-                        else:
-                            isUnmatched = True
-                    if isUnmatched:
-                        logger.debug(f"Unmatched msgKey {msgKey}")
-                    doRxCallback = isUnmatched
-            elif decodedMsg.msgTypeCode == RICProtocols.MSG_TYPE_RESPONSE:
-                # logger.debug(f"RESPONSE {decodedMsg.payload}")
-                # Check for okto message
-                reptObj = {}
-                try:
-                    reptObj = json.loads(decodedMsg.payload.rstrip('\0'))
-                except Exception as excp:
-                    logger.warn(f"_onRxFrameCB RESPONSE is not JSON {excp}")
-                if "okto" in reptObj:
-                    okto = reptObj.get("okto", -1)
-                    if self._fileSendOkTo < okto:
-                        self._fileSendOkTo = okto
-                    self._fileSendNewOkTo = True
-                    # logger.debug(f"OKTO MESSAGE {reptObj['okto']}")
-                elif "cmdName" in reptObj:
-                    cmdName = reptObj.get("cmdName","")
-                    if cmdName == "ufBlock" or cmdName == "ufStatus" or cmdName == "ufCancel":
-                        reason = reptObj.get("reason","")
-                        if reason == "OTAStartFailed":
-                            self._fileOTAStartFailed = True
-                        elif reason == "OTAStartedOK":
-                            self._fileOTAStartedOK = True
-                        elif reason == "notStarted":
-                            self._fileNotStarted = True
-                        elif reason == "userCancel":
-                            self._fileUserCancel = True
-                        elif reason == "failRetries" or reason == "failTimeout":
-                            self._fileFailedInFirmware = True
-                    logger.warn(f"_onRxFrameCB {cmdName} reason {reason}")
-                else:
-                    logger.warn(f"_onRxFrameCB response not OkTo or fileUpload ... {decodedMsg.payload}")
-
-            self.statsUnNumbered += 1
-        # Call the decoded-message callback with the message
-        if doRxCallback and self.decodedMsgCB is not None:
-            self.decodedMsgCB(decodedMsg, self)
-
-    def _onLogLineCB(self, line: str) -> None:
-        if self.logLineCB:
-            self.logLineCB(line)
-
-    def _msgTimeoutCheck(self) -> None:
-        # Check messages outstanding
-        # logger.debug("Check outstanding messages")
-        msgIdxsToRemove = []
-        msgIdxsTimedOut = []
-        with self._msgsOutstandingLock:
-            for msgItem in self._msgsOutstanding.items():
-                timeSinceSent = time.time() - msgItem[1].get("timeSent", 0)
-                if timeSinceSent > msgItem[1].get("timeOutSecs", self.msgRespTimeoutSecs):
-                    if not msgItem[1].get("respValid", False):
-                        msgIdxsTimedOut.append(msgItem[0])
-                    msgIdxsToRemove.append(msgItem[0])
-
-        # Hint to comms layer if messages are failing
-        if len(msgIdxsTimedOut) > 0:
-            self.commsHandler.hintMsgTimeout(len(msgIdxsTimedOut))
-
-        # Debug
-        for msgIdx in msgIdxsTimedOut:
-            logger.warn(f"Message {msgIdx} timed out timeSent {self._msgsOutstanding[msgIdx].get('timeSent',0)} timeNow {time.time()}")
-
-        # Remove timed-out messages
-        for msgIdx in msgIdxsToRemove:
-            with self._msgsOutstandingLock:
-                self._msgsOutstanding.pop(msgIdx)
-
-        # Check rawQuery reports outstanding
-        # logger.debug("Check rawQuery reports outstanding")
-        msgKeysToRemove = []
-        msgKeysTimedOut = []
-        with self._rawQueryOutstandingLock:
-            for msgItem in self._rawQueryOutstanding.items():
-                timeSinceSent = time.time() - msgItem[1].get("timeSent", 0)
-                if timeSinceSent > msgItem[1].get("timeOutSecs", self.msgRespTimeoutSecs):
-                    if not msgItem[1].get("reptValid", False):
-                        msgKeysTimedOut.append(msgItem[0])
-                    msgKeysToRemove.append(msgItem[0])
-
-        # Debug
-        for msgKey in msgKeysTimedOut:
-            logger.warn(f"rawQuery {msgKey} timed out at time {time.time()}")
-            self.statsTimedOut += 1
-
-        # Remove timed-out rawQueries
-        for msgKey in msgKeysToRemove:
-            with self._rawQueryOutstandingLock:
-                self._rawQueryOutstanding.pop(msgKey)
-
-        # Restart timer
-        if self.commsHandler is not None and self.commsHandler.isOpen():
-            self.msgTimeoutCheckTimer = threading.Timer(1.0, self._msgTimeoutCheck)
-            self.msgTimeoutCheckTimer.start()
-
-        # Callback on timer if required
-        if self.msgTimerCB:
-            self.msgTimerCB()
-
-    def getTestOutput(self) -> dict:
-        return self.commsHandler.getTestOutput()
+'''
+RICInterface
+'''
+from typing import Callable, Dict, Union, Optional
+import time
+import threading
+import logging
+import json
+import os
+from .RICProtocols import DecodedMsg, RICProtocols
+from .RICCommsBase import RICCommsBase
+from .RateAverager import RateAverager
+from .ValueAverager import ValueAverager
+from .Exceptions import MartyTransferException
+
+logger = logging.getLogger(__name__)
+
+class RICInterface:
+    '''
+    RICInterface
+    '''
+    def __init__(self, commsHandler: RICCommsBase) -> None:
+        '''
+        Initialise RICInterface
+        '''
+        self.commsHandler = commsHandler
+        self.ricProtocols = RICProtocols()
+        self.decodedMsgCB = None
+        self.logLineCB = None
+        # Message command/response matching
+        self.msgTimerCB = None
+        self._msgsOutstanding: Dict = {}
+        self._msgsOutstandingLock = threading.Lock()
+        self.msgRespTimeoutSecs = 1.5
+        # AddOn QueryRaw message matching
+        self._rawQueryOutstanding: Dict = {}
+        self._rawQueryOutstandingLock = threading.Lock()
+        self._rawQueryMsgKey = 1
+        # Stats
+        self.msgRxRate = RateAverager()
+        self.msgTxRate = RateAverager()
+        self.roundTripInfo = ValueAverager()
+        self.statsMatched = 0
+        self.statsUnMatched = 0
+        self.statsUnNumbered = 0
+        self.statsTimedOut = 0
+        self.uploadBytesPerSec = ValueAverager()
+        # File send vars
+        self._fileOTAStartFailed = False
+        self._fileOTAStartedOK = False
+        self._fileNotStarted = False
+        self._fileUserCancel = False
+        self._fileSendOkTo = 0
+        self._fileSendNewOkTo = False
+        self._fileFailedInFirmware = False
+        self.BLOCK_ACK_TIMEOUT = 15
+        self.BATCH_RETRY_MAX = 3
+        self._fileFailedWrite = False
+        self._streamSendOkTo = 0
+        self._streamClosed = False
+        self._streamSendNewOkTo = False
+        # Streaming
+        from .RICStreamHandler import RICStreamHandler
+        self._ricStreamHandler = RICStreamHandler(self)
+        # Debug
+        self.DEBUG_RIC_SEND_MSG = False
+        self.DEBUG_RIC_SEND_FILE_BLOCK = False
+        self.DEBUG_RIC_SEND_FILE = False
+        self.DEBUG_RIC_RECEIVE_MSG = False
+        self.DEBUG_RIC_STREAM = False
+        self.DEBUG_PERFORMANCE = False
+
+    def __del__(self) -> None:
+        self.commsHandler.close()
+
+    def open(self, openParams: Dict) -> bool:
+        '''
+        Open interface to RIC
+        Args:
+            openParams: dict containing params used to open the connection
+                    (see RICCommsBase and derived classes for details)
+        Returns:
+            True if open succeeded or port is already open
+        Throws:
+            SerialException: if the serial port cannot be opened
+        '''
+        self.commsHandler.setRxFrameCB(self._onRxFrameCB)
+        self.commsHandler.setRxLogLineCB(self._onLogLineCB)
+        openOk = self.commsHandler.open(openParams)
+
+        # Set default timeout based on interface
+        self.msgRespTimeoutSecs = self.commsHandler.getMsgRespTimeoutSecs(self.msgRespTimeoutSecs)
+
+        # Start timer to check message completion
+        self.msgTimeoutCheckTimer = threading.Timer(1.0, self._msgTimeoutCheck)
+        self.msgTimeoutCheckTimer.daemon = True
+        self.msgTimeoutCheckTimer.start()
+        return openOk
+
+    def close(self) -> None:
+        '''
+        Close interface to RIC
+        Args:
+            none
+        Returns:
+            None
+        '''
+        self.commsHandler.close()
+
+    def isOpen(self) -> None:
+        return self.commsHandler.isOpen()
+
+    def setDecodedMsgCB(self, onDecodedMsg: Callable[[DecodedMsg, 'RICInterface'], None]) -> None:
+        '''
+        Set callback on decoded message received from RIC
+        Args:
+            cb: callback function (takes 2 parameters: decoded message and this object)
+        Returns:
+            None
+        '''
+        self.decodedMsgCB = onDecodedMsg
+
+    def setLogLineCB(self, onLogLine: Callable[[str], None]) -> None:
+        '''
+        Set callback on logging line received
+        Args:
+            onLogLine: callback function (takes 1 parameter which is the line of logging information)
+        Returns:
+            None
+        '''
+        self.logLineCB = onLogLine
+
+    def setTimerCB(self, onMsgTimerCB: Callable[[], None]) -> None:
+        '''
+        Set callback which can be used to check for message types (e.g. publish)
+        Args:
+            onMsgTimerCB: callback function (takes 0 parameters)
+        Returns:
+            None
+        '''
+        self.msgTimerCB = onMsgTimerCB
+
+    def sendRICRESTURL(self, msg: str, timeOutSecs: Optional[float] = None) -> bool:
+        '''
+        Send RICREST URL message
+        Args:
+            msg: string containing command URL
+            timeOutSecs: message time-out override in seconds (or None to use default)
+        Returns:
+            True if message sent
+        '''
+        ricRestMsg, msgNum = self.ricProtocols.encodeRICRESTURL(msg)
+        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
+        with self._msgsOutstandingLock:
+            self._msgsOutstanding[msgNum] = {"timeSent": time.time(), "timeOutSecs": timeOutSecs}
+        if self.DEBUG_RIC_SEND_MSG:
+            logger.debug(f"sendRICRESTURL msgNum {msgNum} time {time.time()} msg {msg}")
+        self.commsHandler.send(ricRestMsg)
+        self.msgTxRate.addSample()
+        return True
+
+    def cmdRICRESTURLSync(self, msg: str, timeOutSecs: Optional[float] = None) -> Dict:
+        '''
+        Send RICREST URL message and wait for response
+        Args:
+            msg: string containing command URL
+            timeOutSecs: message time-out override in seconds (or None to use default)
+        Returns:
+            Response turned into a dictionary (from JSON)
+        '''
+        ricRestMsg, msgNum = self.ricProtocols.encodeRICRESTURL(msg)
+        msgSendTime = time.time()
+        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
+        if self.DEBUG_RIC_SEND_MSG:
+            logger.debug(f"cmdRICRESTURLSync msgNum {msgNum} timeout {timeOutSecs} msg {msg}")
+        with self._msgsOutstandingLock:
+            self._msgsOutstanding[msgNum] = {"timeSent": msgSendTime, "timeOutSecs": timeOutSecs, "awaited":True}
+        self.commsHandler.send(ricRestMsg)
+        self.msgTxRate.addSample()
+        # Wait for result
+        return self.waitForSyncResult(msgNum, msgSendTime, timeOutSecs)
+
+    def cmdRICRESTRslt(self, msg: str, timeOutSecs: Optional[float] = None) -> bool:
+        '''
+        Send RICREST URL message and wait for response
+        Args:
+            msg: string containing command URL
+            timeOutSecs: message time-out override in seconds (or None to use default)
+        Returns:
+            Response turned into a dictionary (from JSON)
+        '''
+        response = self.cmdRICRESTURLSync(msg, timeOutSecs)
+        return response.get("rslt", "") == "ok"
+
+    def sendRICRESTCmdFrame(self, msg: Union[str,bytes], 
+                    payload: Union[bytes, str, None] = None, timeOutSecs: Optional[float] = None) -> bool:
+        '''
+        Send RICREST command frame message
+        Args:
+            msg: string or bytes containing command frame
+            payload: optional payload
+            timeOutSecs: message time-out override in seconds (or None to use default)
+        Returns:
+            True if message sent
+        '''
+        ricRestMsg, msgNum = self.ricProtocols.encodeRICRESTCmdFrame(msg, payload)
+        if self.DEBUG_RIC_SEND_MSG:
+            logger.debug(f"sendRICRESTCmdFrame msgNum {msgNum} len {len(ricRestMsg)} msg {msg}")
+        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
+        with self._msgsOutstandingLock:
+            self._msgsOutstanding[msgNum] = {"timeSent": time.time(), "timeOutSecs": timeOutSecs}
+        self.commsHandler.send(ricRestMsg)
+        self.msgTxRate.addSample()
+        return True
+
+    def sendRICRESTCmdFrameSync(self, msg: Union[str,bytes], 
+                    payload: Union[bytes, str] = None,
+                    timeOutSecs: Optional[float] = None) -> Dict:
+        '''
+        Send RICREST command frame message and wait for response
+        Args:
+            msg: string or bytes containing command frame
+            payload: optional payload
+            timeOutSecs: message time-out override in seconds (or None to use default)
+        Returns:
+            Response turned into a dictionary (from JSON)
+        '''
+        # Encode frame
+        ricRestMsg, msgNum = self.ricProtocols.encodeRICRESTCmdFrame(msg, payload)
+        if self.DEBUG_RIC_SEND_MSG:
+            logger.debug(f"sendRICRESTCmdFrameSync msgNum {msgNum} len {len(ricRestMsg)} msg {msg}")
+        msgSendTime = time.time()
+        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
+        with self._msgsOutstandingLock:
+            self._msgsOutstanding[msgNum] = {"timeSent": msgSendTime, "timeOutSecs": timeOutSecs, "awaited":True}
+        self.commsHandler.send(ricRestMsg)
+        self.msgTxRate.addSample()
+        # Wait for result
+        return self.waitForSyncResult(msgNum, msgSendTime, timeOutSecs)
+
+    def waitForSyncResult(self, msgNum: int, msgSendTime: float, timeOutSecs: int):
+        while time.time() < msgSendTime + timeOutSecs:
+            with self._msgsOutstandingLock:
+                # Should be an outstanding message - if not there's a problem
+                if msgNum not in self._msgsOutstanding:
+                    logger.warning(f"sendRICRESTURLSync msgNum {msgNum} not in _msgsOutstanding")
+                    return {"rslt":"failResponse"}
+                # Check if response received
+                if self._msgsOutstanding[msgNum].get("respValid", False):
+                    try:
+                        # Get response
+                        respStr = self._msgsOutstanding[msgNum].get("resp", None)
+                        respObj = {}
+                        if respStr:
+                            respObj = json.loads(respStr.payload.rstrip('\0'))
+                        # debugMsgRespTime = self._msgsOutstanding[msgNum].get("respTime", 0)
+                        # logger.debug(f"waitForSyncResult msgNum {msgNum} msg {msg} resp {json.dumps(respObj)} sendTime {msgSendTime} respTime {debugMsgRespTime}")
+                        return respObj
+                    except Exception as excp:
+                        logger.warning(f"sendRICRESTURLSync msgNum {msgNum} response is not JSON", exc_info=True)
+            time.sleep(0.01)
+        # Debug - if we get here we timed out
+        logger.warning(f"waitForSyncResult failTimeout msgNum {msgNum} sendTime {msgSendTime} timeNow {time.time()} timeout {timeOutSecs}")
+        return {"rslt":"failTimeout"}
+
+    def sendRICRESTFileBlock(self, data: bytes) -> bool:
+        '''
+        Send RICREST file block
+        Args:
+            data: bytes of file data
+        Returns:
+            True if message sent
+        '''
+        ricRestMsg, _ = self.ricProtocols.encodeRICRESTFileBlock(data)
+        if self.DEBUG_RIC_SEND_FILE_BLOCK:
+            logger.debug(f"sendRICRESTFileBlock len {len(ricRestMsg)}")
+        self.commsHandler.send(ricRestMsg)
+        self.msgTxRate.addSample()
+        return True
+
+    def newRoundTrip(self, rtTime:int) -> None:
+        '''
+        Indicate a new round-trip for a message is complete - this is
+        for statistics gathering
+        Args:
+            rtTime: time taken for round-trip in seconds
+        Returns:
+            None
+        '''
+        self.roundTripInfo.add(rtTime)
+        if self.DEBUG_PERFORMANCE:
+            logger.debug(f"RTTime {self.roundTripInfo.getAvg()}")
+
+    def sendTestMsgs(self, numMsgs:int, bytesPerMsg: int) -> None:
+        '''
+        Send a batch of test messages
+        Args:
+            numMsgs: number of messages to send
+            bytesPerMsg: bytes in each message
+        Returns:
+            None
+        '''
+        dataBlock = bytearray(bytesPerMsg)
+        for i in range(numMsgs):
+            self.commsHandler.send(dataBlock)
+            self.msgTxRate.addSample()
+
+    def _sendFileProgressCheckAbort(self, progressCB: Callable[[int, int, 'RICInterface'], bool], 
+                    currentPos: int, fileSize: int) -> bool:
+        if self._fileOTAStartFailed or self._fileNotStarted or self._fileUserCancel or self._fileFailedInFirmware or self._fileFailedWrite:
+            return True
+        if progressCB is None:
+            return False
+        if not progressCB(currentPos, fileSize, self):
+            self.sendRICRESTCmdFrameSync('{"cmdName":"ufCancel"}')
+            return True
+        return False
+
+    def sendFile(self, filename: str, 
+                progressCB: Callable[[int, int, 'RICInterface'], bool] = None,
+                fileDest: str = "fs", reqStr: str = '') -> bool:
+        '''
+        Send a file (from the file system)
+        Args:
+            filename: name of file to send
+            progressCB: callback used to indicate how file send is progressing, callable takes three params
+                    which are bytesSent, totalBytes and the interface to RIC (of type RICInterface) and
+                    returns a bool which should be True to continue the file upload or False to abort
+            fileDest: "fs" to upload to file system, "ricfw" for new RIC firmware
+            reqStr: API request used for transfer, if left blank this is inferred from fileDest, other
+                    values include "fileupload" and "espfwupdate" - see RIC documentation for API
+        Returns:
+            True if operation succeeded
+        Throws:
+            OSError: operating system exceptions
+            May throw other exceptions so include a general exception handler
+        '''
+        # Send the file using the file upload
+        with open(filename, "rb") as f:
+
+            # Read data
+            binaryImage = f.read()
+            binaryImageLen = len(binaryImage)
+            if self.DEBUG_RIC_SEND_FILE:
+                logger.debug(f"File {filename} is {binaryImageLen} bytes long")
+
+            # Check if we're uploading firmware
+            isFirmware = fileDest == "ricfw"
+            if reqStr == '':
+                reqStr = 'espfwupdate' if isFirmware else 'fileupload'
+            uploadName = "fw" if isFirmware else os.path.basename(filename)
+            self._fileOTAStartFailed = False
+            self._fileOTAStartedOK = False
+            self._fileNotStarted = False
+            self._fileUserCancel = False
+            self._fileFailedWrite = False
+            self._fileFailedInFirmware = False
+
+            # Block and batch sizes
+            blockMaxSize = self.commsHandler.commsParams.fileTransfer.get("fileBlockMax", 5000)
+            batchAckSize = self.commsHandler.commsParams.fileTransfer.get("fileBatchAck", 1)
+
+            # Debug
+            if self.DEBUG_RIC_SEND_FILE:
+                logger.debug(f"ricIF sendFile ideal blockMaxSize {blockMaxSize} batchAckSize {batchAckSize}")
+
+            # Frames follow the approach used in the web interface start, block..., end
+            sendFileReq = '{' + f'"cmdName":"ufStart","reqStr":"{reqStr}","fileType":"{fileDest}",' + \
+                            f'"batchMsgSize":{blockMaxSize},"batchAckSize":{batchAckSize},' + \
+                            f'"fileName":"{uploadName}","fileLen":{str(binaryImageLen)}' + '}'
+            resp = self.sendRICRESTCmdFrameSync(sendFileReq, 
+                            timeOutSecs = 10)
+            if resp.get("rslt","") != "ok":
+                raise MartyTransferException("File transfer start not acknowledged")
+
+            # Block and batch sizes
+            blockMaxSize = resp.get("batchMsgSize", blockMaxSize)
+            batchAckSize = resp.get("batchAckSize", 50)
+            self._fileSendOkTo = 0
+
+            # Debug
+            if self.DEBUG_RIC_SEND_FILE:
+                logger.debug(f"ricIF sendFile negotiated blockMaxSize {blockMaxSize} batchAckSize {batchAckSize} resp {resp}")
+
+            # Progress and check for abort
+            if self._sendFileProgressCheckAbort(progressCB, self._fileSendOkTo, binaryImageLen):
+                return False
+
+            # Wait for a period depending on whether we're sending firmware - this is because starting
+            # a firmware update involves the ESP32 in a long-running activity and the firmware becomes
+            # unresponsive during this time
+            if isFirmware:
+                for i in range(5):
+                    time.sleep(1)
+                    if self._sendFileProgressCheckAbort(progressCB, 0, binaryImageLen):
+                        return False
+                    if self._fileOTAStartedOK:
+                        break
+
+            # Debug
+            if self.DEBUG_RIC_SEND_FILE:
+                logger.debug(f"ricIF sendFile starting to send file data ...")
+
+            # Send file blocks
+            numBlocks = 0
+            batchRetryCount = 0
+            while self._fileSendOkTo < binaryImageLen:
+
+                # NOTE: first batch MUST be of size 1 (not batchAckSize) because RIC performs a long-running
+                # blocking task immediately after receiving the first message in a firmware
+                # update - although this could be relaxed for non-firmware update file uploads
+                sendFromPos = self._fileSendOkTo
+                batchStartPos = self._fileSendOkTo
+                batchStartTime = time.time()
+                batchSize = 1 if sendFromPos == 0 else batchAckSize
+                batchBlockIdx = 0
+                self._fileSendNewOkTo = False
+                while batchBlockIdx < batchSize and sendFromPos < binaryImageLen:
+
+                    # Send block
+                    blockToSend = binaryImage[sendFromPos:sendFromPos+blockMaxSize]
+                    self.sendRICRESTFileBlock(sendFromPos.to_bytes(4, 'big') + blockToSend)
+                    sendFromPos += blockMaxSize
+                    batchBlockIdx += 1
+
+                    # Check if we have received an error
+                    if self._fileNotStarted or self._fileUserCancel or self._fileFailedInFirmware or self._fileFailedWrite:
+                        break
+
+                # Debug
+                if self.DEBUG_RIC_SEND_FILE:
+                    logger.debug(f"ricIF sendFile sent batch - start at {batchStartPos} end at {sendFromPos} len {sendFromPos-batchStartPos} okto {self._fileSendOkTo}")
+
+                # Wait for response (there is a timeout at the ESP end to ensure a response is always returned
+                # even if blocks are dropped on reception at ESP) - the timeout here is for these responses
+                # being dropped
+                timeNow = time.time()
+                while time.time() - timeNow < self.BLOCK_ACK_TIMEOUT:
+                    # Progress update
+                    if self._sendFileProgressCheckAbort(progressCB, self._fileSendOkTo, binaryImageLen):
+                        return False
+
+                    # Debug
+                    if self.DEBUG_RIC_SEND_FILE:
+                        logger.debug(f"ricIF sendFile checking for OKTO {self._fileSendOkTo} batchStartPos {batchStartPos}")
+
+                    # Check for okto
+                    if self._fileSendNewOkTo:
+                        batchRetryCount = 0
+                        # Update stats
+                        if self._fileSendOkTo > batchStartPos:
+                            elapsedTime = time.time() - batchStartTime
+                            if elapsedTime > 0:
+                                batchBytesPerSec = (self._fileSendOkTo - batchStartPos) / elapsedTime
+                                self.uploadBytesPerSec.add(batchBytesPerSec)
+                        break
+
+                    # Wait
+                    time.sleep(1)
+
+                # Check if no okto has been received with a greater position than batchStartPos
+                if self._fileSendOkTo <= batchStartPos:
+                    batchRetryCount += 1
+                    if batchRetryCount > self.BATCH_RETRY_MAX:
+                        return False
+
+                # Block count
+                numBlocks += 1
+
+            # Debug
+            if self.DEBUG_RIC_SEND_FILE:
+                logger.debug(f"ricIF sendFile sending END")
+
+            # End frame
+            resp = self.sendRICRESTCmdFrameSync('{' + f'"cmdName":"ufEnd","reqStr":"fileupload","fileType":"{fileDest}",' + \
+                            f'"fileName":"{uploadName}","fileLen":{str(binaryImageLen)},' + \
+                            f'"blockCount":{str(numBlocks)}' + '}', 
+                            timeOutSecs = 5)
+            if resp.get("rslt","") != "ok":
+                return False
+            return True
+
+    def streamSoundFile(self, fileName: str, targetEndpoint: str,
+                progressCB: Callable[[int, int, 'RICInterface'], bool] = None) -> bool:
+        '''
+        Stream sound from the file system
+        Args:
+            fileName: The file to stream
+            progressCB: callback used to indicate how stream is progressing, callable takes three params
+                    which are bytesSent, totalBytes and the interface to RIC (of type RICInterface) and
+                    returns a bool which should be True to continue the stream or False to abort
+        Returns:
+            True if operation succeeded
+        Throws:
+            OSError: operating system exceptions
+            May throw other exceptions so include a general exception handler
+        '''
+        return self._ricStreamHandler.streamSoundFile(fileName, targetEndpoint, progressCB)
+
+    def getStats(self) -> Dict:
+        return {
+            "roundTripAvgMS":self.roundTripInfo.getAvg()*1000,
+            "msgRxRatePS":self.msgRxRate.getAvg(),
+            "msgTxRatePS":self.msgTxRate.getAvg(),
+            "unmatched":self.statsUnMatched,
+            "matched":self.statsMatched,
+            "unnumbered":self.statsUnNumbered,
+            "timedOut":self.statsTimedOut,
+            "uploadBPS":self.uploadBytesPerSec.getAvg(),
+            "rxCount":self.msgRxRate.getTotal(),
+            "txCount":self.msgTxRate.getTotal(),
+        }
+
+    def addOnQueryRaw(self, addOnName: str, dataToWrite: bytes, numBytesToRead: int,
+                        timeOutSecs: Optional[float] = None) -> Dict:
+        '''
+        Write and read an addOn directly (raw-mode)
+        Args:
+            addOnName, name of the addOn (see get_add_ons_status() at the top level or response to
+                addon/list REST API command)
+            dataToWrite, can be zero length if nothing is to be written, the first byte will generally
+                be the register or opcode of the addOn
+            numBytesToRead: number of bytes to read from the device - can be zero
+            timeOutSecs: message time-out override in seconds (or None to use default)
+        Returns:
+            Dict with keys including:
+                "rslt" - the result which will be "ok" if the query succeeded
+                "dataRead" - the data read from the addOn
+        '''
+        # Handle msgKey
+        msgKey = self._rawQueryMsgKey
+        self._rawQueryMsgKey += 1
+        if self._rawQueryMsgKey > 99999:
+            self._rawQueryMsgKey = 1
+
+        # Form command
+        hexWrStr = dataToWrite.hex()
+        ricRestCmd = f"elem/{addOnName}/json?cmd=raw&hexWr={hexWrStr}&numToRd={numBytesToRead}&msgKey={msgKey}"
+
+        # Register in raw message matching
+        timeOutSecs = timeOutSecs if timeOutSecs is not None else self.msgRespTimeoutSecs
+        with self._rawQueryOutstandingLock:
+            self._rawQueryOutstanding[msgKey] = {"timeSent": time.time(), "timeOutSecs": timeOutSecs, "awaited":True}
+
+        # Send message
+        resp = self.cmdRICRESTURLSync(ricRestCmd)
+        resp["dataRead"] = b""
+        if resp.get("rslt", "") != "ok":
+            self._rawQueryOutstanding.pop(msgKey)
+            return resp
+
+        # Wait for a report message generated by the addOn access process
+        msgSendTime = time.time()
+        while time.time() < msgSendTime + timeOutSecs:
+            with self._rawQueryOutstandingLock:
+                # Should be an outstanding message - if not there's a problem
+                if msgKey not in self._rawQueryOutstanding:
+                    resp["rslt"] = "failReport"
+                    return resp
+                # Check if a report received
+                if self._rawQueryOutstanding[msgKey].get("reptValid", False):
+                    # Get report
+                    reptObj = self._rawQueryOutstanding[msgKey].get("reptObj", {})
+                    # logger.debug(f"msgKey {msgKey} msg {ricRestCmd} rept {json.dumps(reptObj)} sendTime {msgSendTime}")
+                    resp["dataRead"] = reptObj.get("hexRd", b"")
+                    return resp
+            time.sleep(0.01)
+        return {"rslt":"failTimeout"}
+
+    def _onRxFrameCB(self, frame: bytes) -> None:
+        self.msgRxRate.addSample()
+        decodedMsg = self.ricProtocols.decodeRICFrame(frame)
+        if self.DEBUG_RIC_RECEIVE_MSG:
+            logger.debug(f"_onRxFrameCB len {len(frame)} msgNum {decodedMsg.msgNum} type {decodedMsg.msgTypeCode} data {frame.hex()}")
+            if decodedMsg.protocolID != RICProtocols.PROTOCOL_ROSSERIAL:
+                logger.debug(f"_onRxFrameCB {decodedMsg.toString()}")
+        doRxCallback = True
+        if decodedMsg.msgNum != 0:
+            # Numbered message - this is the response to a REST API command
+            if self.DEBUG_RIC_RECEIVE_MSG:
+                logger.debug(f"_onRxFrameCB msgNum {decodedMsg.msgNum} {decodedMsg.payload}")
+            isUnmatched = False
+            with self._msgsOutstandingLock:
+                if decodedMsg.msgNum in self._msgsOutstanding:
+                    msgRec = self._msgsOutstanding[decodedMsg.msgNum]
+                    roundTripTime = time.time() - msgRec["timeSent"]
+                    self.newRoundTrip(roundTripTime)
+                    if not msgRec.get("awaited", False):
+                        self._msgsOutstanding.pop(decodedMsg.msgNum)
+                    else:
+                        msgRec["resp"] = decodedMsg
+                        msgRec["respValid"] = True
+                        msgRec["respTime"] = time.time()
+                    self.statsMatched += 1
+                else:
+                    isUnmatched = True
+                    self.statsUnMatched += 1
+            if isUnmatched:
+                logger.warning(f"_onRxFrameCB Unmatched msgNum {decodedMsg.msgNum}")
+            doRxCallback = isUnmatched
+        else:
+            if self.DEBUG_RIC_RECEIVE_MSG:
+                logger.debug(f"_onRxFrameCB unnumbered restType {decodedMsg.restType} msgType {decodedMsg.msgTypeCode}")
+            if decodedMsg.msgTypeCode == RICProtocols.MSG_TYPE_REPORT:
+                # Report message - this can include results of accessing addOns
+                # logger.debug(f"_onRxFrameCB REPORT {decodedMsg.payload}")
+                reptObj = {}
+                try:
+                    reptObj = json.loads(decodedMsg.payload.rstrip('\0'))
+                except Exception as excp:
+                    logger.warning(f"_onRxFrameCB REPORT is not JSON {excp}")
+                msgKey = reptObj.get("msgKey", '')
+                if type(msgKey) is str:
+                    try:
+                        msgKey = int(msgKey)
+                    except:
+                        msgKey = 0
+                if msgKey != 0:
+                    isUnmatched = False
+                    with self._rawQueryOutstandingLock:
+                        if msgKey in self._rawQueryOutstanding:
+                            msgRec = self._rawQueryOutstanding[msgKey]
+                            if not msgRec.get("awaited", False):
+                                self._rawQueryOutstanding.pop(msgKey)
+                            else:
+                                msgRec["reptObj"] = reptObj
+                                msgRec["reptValid"] = True
+                        else:
+                            isUnmatched = True
+                    if isUnmatched:
+                        logger.debug(f"Unmatched msgKey {msgKey}")
+                    doRxCallback = isUnmatched
+            elif decodedMsg.msgTypeCode == RICProtocols.MSG_TYPE_RESPONSE:
+                if self.DEBUG_RIC_RECEIVE_MSG:
+                    logger.debug(f"RESPONSE received {decodedMsg.payload}")
+                # Check for okto message
+                reptObj = {}
+                try:
+                    reptObj = json.loads(decodedMsg.payload.rstrip('\0'))
+                except Exception as excp:
+                    logger.warning(f"_onRxFrameCB RESPONSE is not JSON {excp}")
+                if "okto" in reptObj:
+                    okto = reptObj.get("okto", -1)
+                    if self._fileSendOkTo < okto:
+                        self._fileSendOkTo = okto
+                    self._fileSendNewOkTo = True
+                    if self.DEBUG_RIC_SEND_FILE:
+                        logger.warning(f"OKTO MESSAGE {reptObj['okto']}")
+                if "sokto" in reptObj:
+                    sokto = reptObj.get("sokto", -1)
+                    if self._streamSendOkTo < sokto:
+                        self._streamSendOkTo = sokto
+                    self._streamSendNewOkTo = True
+                    if self.DEBUG_RIC_STREAM:
+                        logger.debug(f"SOKTO MESSAGE {reptObj['sokto']}")
+                elif "cmdName" in reptObj:
+                    cmdName = reptObj.get("cmdName","")
+                    if cmdName == "ufBlock" or cmdName == "ufStatus" or cmdName == "ufCancel":
+                        reason = reptObj.get("reason","")
+                        if reason == "OTAStartFailed":
+                            self._fileOTAStartFailed = True
+                        elif reason == "OTAStartedOK":
+                            self._fileOTAStartedOK = True
+                        elif reason == "notStarted":
+                            self._fileNotStarted = True
+                        elif reason == "userCancel":
+                            self._fileUserCancel = True
+                        elif reason == "failRetries" or reason == "failTimeout":
+                            self._fileFailedInFirmware = True
+                        elif reason == 'failFileWrite':
+                            self._fileFailedWrite = True
+                    logger.warning(f"_onRxFrameCB {cmdName} reason {reason}")
+                elif "rslt" in reptObj:
+                    if reptObj["rslt"].startswith("fail"):
+                        logger.warning(f"_onRxFrameCB {reptObj['rslt']}")
+                        self._streamClosed = True
+                else:
+                    logger.warning(f"_onRxFrameCB response not OkTo or fileUpload ... {decodedMsg.payload}")
+
+            self.statsUnNumbered += 1
+        # Call the decoded-message callback with the message
+        if doRxCallback and self.decodedMsgCB is not None:
+            self.decodedMsgCB(decodedMsg, self)
+
+    def _onLogLineCB(self, line: str) -> None:
+        if self.logLineCB:
+            self.logLineCB(line.rstrip())
+
+    def _msgTimeoutCheck(self) -> None:
+        # Check messages outstanding
+        # logger.debug("Check outstanding messages")
+        msgIdxsToRemove = []
+        msgIdxsTimedOut = []
+        with self._msgsOutstandingLock:
+            for msgItem in self._msgsOutstanding.items():
+                timeSinceSent = time.time() - msgItem[1].get("timeSent", 0)
+                if timeSinceSent > msgItem[1].get("timeOutSecs", self.msgRespTimeoutSecs):
+                    if not msgItem[1].get("respValid", False):
+                        msgIdxsTimedOut.append(msgItem[0])
+                    msgIdxsToRemove.append(msgItem[0])
+
+        # Hint to comms layer if messages are failing
+        if len(msgIdxsTimedOut) > 0:
+            self.commsHandler.hintMsgTimeout(len(msgIdxsTimedOut))
+
+        # Debug
+        for msgIdx in msgIdxsTimedOut:
+            logger.warning(f"Message {msgIdx} timed out timeSent {self._msgsOutstanding[msgIdx].get('timeSent',0)} timeNow {time.time()}")
+
+        # Remove timed-out messages
+        for msgIdx in msgIdxsToRemove:
+            with self._msgsOutstandingLock:
+                self._msgsOutstanding.pop(msgIdx)
+
+        # Check rawQuery reports outstanding
+        # logger.debug("Check rawQuery reports outstanding")
+        msgKeysToRemove = []
+        msgKeysTimedOut = []
+        with self._rawQueryOutstandingLock:
+            for msgItem in self._rawQueryOutstanding.items():
+                timeSinceSent = time.time() - msgItem[1].get("timeSent", 0)
+                if timeSinceSent > msgItem[1].get("timeOutSecs", self.msgRespTimeoutSecs):
+                    if not msgItem[1].get("reptValid", False):
+                        msgKeysTimedOut.append(msgItem[0])
+                    msgKeysToRemove.append(msgItem[0])
+
+        # Debug
+        for msgKey in msgKeysTimedOut:
+            logger.warning(f"rawQuery {msgKey} timed out at time {time.time()}")
+            self.statsTimedOut += 1
+
+        # Remove timed-out rawQueries
+        for msgKey in msgKeysToRemove:
+            with self._rawQueryOutstandingLock:
+                self._rawQueryOutstanding.pop(msgKey)
+
+        # Restart timer
+        if self.commsHandler is not None and self.commsHandler.isOpen():
+            self.msgTimeoutCheckTimer = threading.Timer(1.0, self._msgTimeoutCheck)
+            self.msgTimeoutCheckTimer.start()
+
+        # Callback on timer if required
+        if self.msgTimerCB:
+            self.msgTimerCB()
+
+    def getTestOutput(self) -> dict:
+        return self.commsHandler.getTestOutput()
+
+    def _streamStart(self):
+        self._streamSendOkTo = 0
+        self._streamSendNewOkTo = False
+        self._streamClosed = False
+
+    def _streamGetLatest(self):
+        isNew = self._streamSendNewOkTo
+        self._streamSendNewOkTo = False
+        return isNew, self._streamSendOkTo, self._streamClosed
```

### Comparing `martypy-3.4.3/martypy/RICROSSerial.py` & `martypy-3.5.0/martypy/RICROSSerial.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,240 +1,240 @@
-'''
-RICROSSerial
-'''
-import logging
-import math
-import struct
-from typing import Callable, Dict, List, Tuple
-
-logger = logging.getLogger(__name__)
-
-class RICROSSerial:
-
-    # ROSSerial ROSTopics
-    ROSTOPIC_V2_SMART_SERVOS = 120
-    ROSTOPIC_V2_ACCEL = 121
-    ROSTOPIC_V2_POWER_STATUS = 122
-    ROSTOPIC_V2_ADDONS = 123
-    ROSTOPIC_V2_ROBOT_STATUS = 124
-
-    # ROSSerial message format
-    RS_MSG_MIN_LENGTH = 8
-    RS_MSG_LEN_LOW_POS = 2
-    RS_MSG_LEN_HIGH_POS = 3
-    RS_MSG_TOPIC_ID_LOW_POS = 5
-    RS_MSG_TOPIC_ID_HIGH_POS = 6
-    RS_MSG_PAYLOAD_POS = 7
-
-    # Max payload length
-    MAX_VALID_PAYLOAD_LEN = 1000
-
-    # V2 ROSTOPIC SMART_SERVOS message layout
-    ROS_SMART_SERVOS_MAX_NUM_SERVOS = 15
-    ROS_SMART_SERVOS_ATTR_GROUP_BYTES = 6
-    ROS_SMART_SERVOS_ATTR_ID_IDX = 0
-    ROS_SMART_SERVOS_ATTR_SERVO_POS_IDX = 1
-    ROS_SMART_SERVOS_ATTR_MOTOR_CURRENT_IDX = 3
-    ROS_SMART_SERVOS_ATTR_STATUS_IDX = 5
-    ROS_SMART_SERVOS_INVALID_POS = -32768
-    ROS_SMART_SERVOS_INVALID_CURRENT = -32768
-
-    # V2 ROSTOPIC ACCEL message layout
-    ROS_ACCEL_BYTES = 14
-    ROS_ACCEL_POS_X = 0
-    ROS_ACCEL_POS_Y = 4
-    ROS_ACCEL_POS_Z = 8
-    ROS_ACCEL_POS_IDNO = 12
-    ROS_ACCEL_POS_FLAGS = 13
-
-    # V2 ROSTOPIC POWER STATUS message layout
-    ROS_POWER_STATUS_BYTES = 13
-    ROS_POWER_STATUS_REMCAPPC = 0
-    ROS_POWER_STATUS_BATTTEMPC = 1
-    ROS_POWER_STATUS_REMCAPMAH = 2
-    ROS_POWER_STATUS_FULLCAPMAH = 4
-    ROS_POWER_STATUS_CURRENTMA = 6
-    ROS_POWER_STATUS_5V_ON_SECS = 8
-    ROS_POWER_STATUS_POWERFLAGS = 10
-    ROS_POWER_STATUS_FLAGBIT_USB_POWER = 0
-    ROS_POWER_STATUS_FLAGBIT_5V_ON = 1
-    ROS_POWER_STATUS_IDNO = 12
-
-    # V2 ROSTOPIC ROBOT STATUS message layout
-    ROS_ROBOT_STATUS_BYTES = 24
-    ROS_ROBOT_STATUS_BYTES_MINIMAL = 2
-    ROS_ROBOT_STATUS_MOTION_FLAGS = 0
-    ROS_ROBOT_STATUS_IS_MOVING_MASK = 0x01
-    ROS_ROBOT_STATUS_IS_PAUSED_MASK = 0x02
-    ROS_ROBOT_STATUS_FW_UPDATE_MASK = 0x04
-    ROS_ROBOT_STATUS_QUEUED_WORK_COUNT = 1
-    ROS_ROBOT_STATUS_HEAP_FREE_POS = 2
-    ROS_ROBOT_STATUS_HEAP_FREE_BYTES = 4
-    ROS_ROBOT_STATUS_HEAP_MIN_POS = 6
-    ROS_ROBOT_STATUS_HEAP_MIN_BYTES = 4
-    ROS_ROBOT_STATUS_INDICATORS_POS = 10
-    ROS_ROBOT_STATUS_INDICATOR_BYTES = 4
-    ROS_ROBOT_STATUS_INDICATORS_NUM = 3
-    ROS_ROBOT_STATUS_SYSMOD_LOOPMS_AVG_POS = 22
-    ROS_ROBOT_STATUS_SYSMOD_LOOPMS_AVG_SIZE = 1
-    ROS_ROBOT_STATUS_SYSMOD_LOOPMS_MAX_POS = 23
-    ROS_ROBOT_STATUS_SYSMOD_LOOPMS_MAX_SIZE = 1
-
-    # V2 ROSTOPIC ADDONS message layout
-    ROS_ADDONS_MAX_NUM_ADDONS = 15
-    ROS_ADDON_GROUP_BYTES = 12
-    ROS_ADDON_IDNO_POS = 0
-    ROS_ADDON_FLAGS_POS = 1
-    ROS_ADDON_DATAVALID_FLAG_MASK = 0x80
-    ROS_ADDON_STATUS_POS = 2
-    ROS_ADDON_STATUS_BYTES = 10
-
-    @classmethod
-    def decode(cls, rosSerialMsg: bytes, startPos: int, elemDecodeCB: Callable[[int,bytes],None]) -> None:
-
-        # Payload may contain multiple ROSSerial messages
-        msgPos = startPos
-        while True:
-            remainingMsgLen = len(rosSerialMsg) - msgPos
-
-            # logger.debug(f'ROSSerial Decode {remainingMsgLen}')
-
-            if remainingMsgLen < cls.RS_MSG_MIN_LENGTH:
-                break
-
-            # Extract header
-            payloadLength = rosSerialMsg[msgPos + cls.RS_MSG_LEN_LOW_POS] + \
-                    rosSerialMsg[msgPos + cls.RS_MSG_LEN_HIGH_POS] * 256
-            topicID = rosSerialMsg[msgPos + cls.RS_MSG_TOPIC_ID_LOW_POS] + \
-                rosSerialMsg[msgPos + cls.RS_MSG_TOPIC_ID_HIGH_POS] * 256
-
-            # logger.debug(f'ROSSerial len {payloadLength} topic {topicID}')
-
-            # Check max length
-            if payloadLength < 0 or payloadLength > cls.MAX_VALID_PAYLOAD_LEN:
-                break
-
-            # Check min length
-            if len(rosSerialMsg) < payloadLength + cls.RS_MSG_MIN_LENGTH:
-                break
-
-            # Extract payload
-            payload = rosSerialMsg[msgPos + cls.RS_MSG_PAYLOAD_POS : msgPos + cls.RS_MSG_PAYLOAD_POS + payloadLength]
-            # logger.debug('ROSSerial {}'.format(''.join('{:02x}'.format(x) for x in payload)))
-
-            # Callback with payload
-            if elemDecodeCB:
-                elemDecodeCB(topicID, payload)
-
-            # Move msgPos on
-            msgPos += cls.RS_MSG_PAYLOAD_POS + payloadLength + 1
-
-            # logger.debug(f'ROSSerial decode msgPos {msgPos}')
-
-    @classmethod
-    def extractSmartServos(cls, buf: bytes) -> Dict:
-        #  Each group of attributes for a servo is a fixed size
-        numGroups = math.floor(len(buf) / cls.ROS_SMART_SERVOS_ATTR_GROUP_BYTES)
-        servos = {}
-        bufPos = 0
-        for _ in range(numGroups):
-            servoData = struct.unpack(">BhhB", buf[bufPos:bufPos+cls.ROS_SMART_SERVOS_ATTR_GROUP_BYTES])
-            servos[servoData[0]] = {
-                "IDNo": servoData[0],
-                "pos": servoData[1],
-                "current": servoData[2],
-                "flags": servoData[3],
-                "enabled": (servoData[3] & 0x01) != 0,
-                "commsOK": (servoData[3] & 0x80) != 0,
-            }
-            bufPos += cls.ROS_SMART_SERVOS_ATTR_GROUP_BYTES
-        return servos
-
-    @classmethod
-    def extractAccel(cls, buf: bytes) -> Tuple[float, float, float]:
-        xyzTimes1024 = struct.unpack(">fffBB", buf[0:cls.ROS_ACCEL_BYTES])
-        return [round(val/1024,2) for val in xyzTimes1024[0:3]]
-
-    @classmethod
-    def extractPowerStatus(cls, buf: bytes) -> Dict:
-        pst = struct.unpack(">BBHHhHHB", buf[0:cls.ROS_POWER_STATUS_BYTES])
-        power5VIsOn = (pst[6] & 0x0002) != 0
-        battInfoValid = (pst[6] & 0x0004) == 0
-        powerUSBIsValid = (pst[6] & 0x0008) == 0
-        powerInfo = {
-            "powerFlags": pst[6],
-            "power5VIsOn": power5VIsOn,
-            "powerUSBIsConnected": (pst[6] & 0x0001) != 0 and powerUSBIsValid,
-            "battInfoValid": battInfoValid,
-            "powerUSBIsValid": powerUSBIsValid,
-            "IDNo": pst[7]
-        }
-        if battInfoValid:
-            powerInfo.update({
-                "battRemainCapacityPercent": pst[0],
-                "battTempDegC": pst[1],
-                "battRemainCapacityMAH": pst[2],
-                "battFullCapacityMAH": pst[3],
-                "battCurrentMA": pst[4],
-            })
-        if power5VIsOn:
-            powerInfo.update({
-                "power5VOnTimeSecs": pst[5]
-            })
-        return powerInfo
-
-    @classmethod
-    def extractRGBT(cls, rgbtVal:int):
-        stateVal = rgbtVal & 0xff
-        rgbtStates = ["off","on","breathe","override"]
-        rgbtState = "unknown"
-        if stateVal >= 0 and stateVal < len(rgbtStates):
-            rgbtState = rgbtStates[stateVal]
-        return {
-            "r": (rgbtVal >> 24) & 0xff,
-            "g": (rgbtVal >> 16) & 0xff,
-            "b": (rgbtVal >> 8) & 0xff,
-            "state": rgbtState
-        }
-
-
-    @classmethod
-    def extractRobotStatus(cls, buf: bytes) -> Dict:
-        if len(buf) >= cls.ROS_ROBOT_STATUS_BYTES:
-            robotStat = struct.unpack(">BBIIIIIBB", buf[0:cls.ROS_ROBOT_STATUS_BYTES])
-            return {
-                "flags": robotStat[0],
-                "workQCount": robotStat[1],
-                "isMoving": (robotStat[0] & 0x01) != 0,
-                "isPaused": (robotStat[0] & 0x02) != 0,
-                "isFwUpdating": (robotStat[0] & 0x04) != 0,
-                "heapFree": robotStat[2],
-                "heapMin": robotStat[3],
-                "pixRGBT": list(cls.extractRGBT(robotStat[i+4]) for i in range(3)),
-                "loopMsAvg": robotStat[7],
-                "loopMsMax": robotStat[8]
-            }
-        else:
-            robotStat = struct.unpack(">BB", buf[0:cls.ROS_ROBOT_STATUS_BYTES_MINIMAL])
-            return {
-                "flags": robotStat[0],
-                "workQCount": robotStat[1],
-                "isMoving": (robotStat[0] & 0x01) != 0,
-                "isPaused": (robotStat[0] & 0x02) != 0,
-                "isFwUpdating": (robotStat[0] & 0x04) != 0,
-            }
-
-    @classmethod
-    def extractAddOnStatus(cls, buf: bytes) -> List:
-        #  Each group of attributes for an add-on is a fixed size
-        numGroups = math.floor(len(buf) / cls.ROS_ADDON_GROUP_BYTES)
-        addOns = {}
-        bufPos = 0
-        for _ in range(numGroups):
-            adb = buf[bufPos:bufPos+cls.ROS_ADDON_GROUP_BYTES]
-            addOns[adb[0]] = {
-                "IDNo": adb[0],
-                "valid": (adb[1] & 0x80) != 0,
-                "data": adb[2:]
-            }
-            bufPos += cls.ROS_ADDON_GROUP_BYTES
-        return addOns
+'''
+RICROSSerial
+'''
+import logging
+import math
+import struct
+from typing import Callable, Dict, List, Tuple
+
+logger = logging.getLogger(__name__)
+
+class RICROSSerial:
+
+    # ROSSerial ROSTopics
+    ROSTOPIC_V2_SMART_SERVOS = 120
+    ROSTOPIC_V2_ACCEL = 121
+    ROSTOPIC_V2_POWER_STATUS = 122
+    ROSTOPIC_V2_ADDONS = 123
+    ROSTOPIC_V2_ROBOT_STATUS = 124
+
+    # ROSSerial message format
+    RS_MSG_MIN_LENGTH = 8
+    RS_MSG_LEN_LOW_POS = 2
+    RS_MSG_LEN_HIGH_POS = 3
+    RS_MSG_TOPIC_ID_LOW_POS = 5
+    RS_MSG_TOPIC_ID_HIGH_POS = 6
+    RS_MSG_PAYLOAD_POS = 7
+
+    # Max payload length
+    MAX_VALID_PAYLOAD_LEN = 1000
+
+    # V2 ROSTOPIC SMART_SERVOS message layout
+    ROS_SMART_SERVOS_MAX_NUM_SERVOS = 15
+    ROS_SMART_SERVOS_ATTR_GROUP_BYTES = 6
+    ROS_SMART_SERVOS_ATTR_ID_IDX = 0
+    ROS_SMART_SERVOS_ATTR_SERVO_POS_IDX = 1
+    ROS_SMART_SERVOS_ATTR_MOTOR_CURRENT_IDX = 3
+    ROS_SMART_SERVOS_ATTR_STATUS_IDX = 5
+    ROS_SMART_SERVOS_INVALID_POS = -32768
+    ROS_SMART_SERVOS_INVALID_CURRENT = -32768
+
+    # V2 ROSTOPIC ACCEL message layout
+    ROS_ACCEL_BYTES = 14
+    ROS_ACCEL_POS_X = 0
+    ROS_ACCEL_POS_Y = 4
+    ROS_ACCEL_POS_Z = 8
+    ROS_ACCEL_POS_IDNO = 12
+    ROS_ACCEL_POS_FLAGS = 13
+
+    # V2 ROSTOPIC POWER STATUS message layout
+    ROS_POWER_STATUS_BYTES = 13
+    ROS_POWER_STATUS_REMCAPPC = 0
+    ROS_POWER_STATUS_BATTTEMPC = 1
+    ROS_POWER_STATUS_REMCAPMAH = 2
+    ROS_POWER_STATUS_FULLCAPMAH = 4
+    ROS_POWER_STATUS_CURRENTMA = 6
+    ROS_POWER_STATUS_5V_ON_SECS = 8
+    ROS_POWER_STATUS_POWERFLAGS = 10
+    ROS_POWER_STATUS_FLAGBIT_USB_POWER = 0
+    ROS_POWER_STATUS_FLAGBIT_5V_ON = 1
+    ROS_POWER_STATUS_IDNO = 12
+
+    # V2 ROSTOPIC ROBOT STATUS message layout
+    ROS_ROBOT_STATUS_BYTES = 24
+    ROS_ROBOT_STATUS_BYTES_MINIMAL = 2
+    ROS_ROBOT_STATUS_MOTION_FLAGS = 0
+    ROS_ROBOT_STATUS_IS_MOVING_MASK = 0x01
+    ROS_ROBOT_STATUS_IS_PAUSED_MASK = 0x02
+    ROS_ROBOT_STATUS_FW_UPDATE_MASK = 0x04
+    ROS_ROBOT_STATUS_QUEUED_WORK_COUNT = 1
+    ROS_ROBOT_STATUS_HEAP_FREE_POS = 2
+    ROS_ROBOT_STATUS_HEAP_FREE_BYTES = 4
+    ROS_ROBOT_STATUS_HEAP_MIN_POS = 6
+    ROS_ROBOT_STATUS_HEAP_MIN_BYTES = 4
+    ROS_ROBOT_STATUS_INDICATORS_POS = 10
+    ROS_ROBOT_STATUS_INDICATOR_BYTES = 4
+    ROS_ROBOT_STATUS_INDICATORS_NUM = 3
+    ROS_ROBOT_STATUS_SYSMOD_LOOPMS_AVG_POS = 22
+    ROS_ROBOT_STATUS_SYSMOD_LOOPMS_AVG_SIZE = 1
+    ROS_ROBOT_STATUS_SYSMOD_LOOPMS_MAX_POS = 23
+    ROS_ROBOT_STATUS_SYSMOD_LOOPMS_MAX_SIZE = 1
+
+    # V2 ROSTOPIC ADDONS message layout
+    ROS_ADDONS_MAX_NUM_ADDONS = 15
+    ROS_ADDON_GROUP_BYTES = 12
+    ROS_ADDON_IDNO_POS = 0
+    ROS_ADDON_FLAGS_POS = 1
+    ROS_ADDON_DATAVALID_FLAG_MASK = 0x80
+    ROS_ADDON_STATUS_POS = 2
+    ROS_ADDON_STATUS_BYTES = 10
+
+    @classmethod
+    def decode(cls, rosSerialMsg: bytes, startPos: int, elemDecodeCB: Callable[[int,bytes],None]) -> None:
+
+        # Payload may contain multiple ROSSerial messages
+        msgPos = startPos
+        while True:
+            remainingMsgLen = len(rosSerialMsg) - msgPos
+
+            # logger.debug(f'ROSSerial Decode {remainingMsgLen}')
+
+            if remainingMsgLen < cls.RS_MSG_MIN_LENGTH:
+                break
+
+            # Extract header
+            payloadLength = rosSerialMsg[msgPos + cls.RS_MSG_LEN_LOW_POS] + \
+                    rosSerialMsg[msgPos + cls.RS_MSG_LEN_HIGH_POS] * 256
+            topicID = rosSerialMsg[msgPos + cls.RS_MSG_TOPIC_ID_LOW_POS] + \
+                rosSerialMsg[msgPos + cls.RS_MSG_TOPIC_ID_HIGH_POS] * 256
+
+            # logger.debug(f'ROSSerial len {payloadLength} topic {topicID}')
+
+            # Check max length
+            if payloadLength < 0 or payloadLength > cls.MAX_VALID_PAYLOAD_LEN:
+                break
+
+            # Check min length
+            if len(rosSerialMsg) < payloadLength + cls.RS_MSG_MIN_LENGTH:
+                break
+
+            # Extract payload
+            payload = rosSerialMsg[msgPos + cls.RS_MSG_PAYLOAD_POS : msgPos + cls.RS_MSG_PAYLOAD_POS + payloadLength]
+            # logger.debug('ROSSerial {}'.format(''.join('{:02x}'.format(x) for x in payload)))
+
+            # Callback with payload
+            if elemDecodeCB:
+                elemDecodeCB(topicID, payload)
+
+            # Move msgPos on
+            msgPos += cls.RS_MSG_PAYLOAD_POS + payloadLength + 1
+
+            # logger.debug(f'ROSSerial decode msgPos {msgPos}')
+
+    @classmethod
+    def extractSmartServos(cls, buf: bytes) -> Dict:
+        #  Each group of attributes for a servo is a fixed size
+        numGroups = math.floor(len(buf) / cls.ROS_SMART_SERVOS_ATTR_GROUP_BYTES)
+        servos = {}
+        bufPos = 0
+        for _ in range(numGroups):
+            servoData = struct.unpack(">BhhB", buf[bufPos:bufPos+cls.ROS_SMART_SERVOS_ATTR_GROUP_BYTES])
+            servos[servoData[0]] = {
+                "IDNo": servoData[0],
+                "pos": servoData[1],
+                "current": servoData[2],
+                "flags": servoData[3],
+                "enabled": (servoData[3] & 0x01) != 0,
+                "commsOK": (servoData[3] & 0x80) != 0,
+            }
+            bufPos += cls.ROS_SMART_SERVOS_ATTR_GROUP_BYTES
+        return servos
+
+    @classmethod
+    def extractAccel(cls, buf: bytes) -> Tuple[float, float, float]:
+        xyzTimes1024 = struct.unpack(">fffBB", buf[0:cls.ROS_ACCEL_BYTES])
+        return [round(val/1024,2) for val in xyzTimes1024[0:3]]
+
+    @classmethod
+    def extractPowerStatus(cls, buf: bytes) -> Dict:
+        pst = struct.unpack(">BBHHhHHB", buf[0:cls.ROS_POWER_STATUS_BYTES])
+        power5VIsOn = (pst[6] & 0x0002) != 0
+        battInfoValid = (pst[6] & 0x0004) == 0
+        powerUSBIsValid = (pst[6] & 0x0008) == 0
+        powerInfo = {
+            "powerFlags": pst[6],
+            "power5VIsOn": power5VIsOn,
+            "powerUSBIsConnected": (pst[6] & 0x0001) != 0 and powerUSBIsValid,
+            "battInfoValid": battInfoValid,
+            "powerUSBIsValid": powerUSBIsValid,
+            "IDNo": pst[7]
+        }
+        if battInfoValid:
+            powerInfo.update({
+                "battRemainCapacityPercent": pst[0],
+                "battTempDegC": pst[1],
+                "battRemainCapacityMAH": pst[2],
+                "battFullCapacityMAH": pst[3],
+                "battCurrentMA": pst[4],
+            })
+        if power5VIsOn:
+            powerInfo.update({
+                "power5VOnTimeSecs": pst[5]
+            })
+        return powerInfo
+
+    @classmethod
+    def extractRGBT(cls, rgbtVal:int):
+        stateVal = rgbtVal & 0xff
+        rgbtStates = ["off","on","breathe","override"]
+        rgbtState = "unknown"
+        if stateVal >= 0 and stateVal < len(rgbtStates):
+            rgbtState = rgbtStates[stateVal]
+        return {
+            "r": (rgbtVal >> 24) & 0xff,
+            "g": (rgbtVal >> 16) & 0xff,
+            "b": (rgbtVal >> 8) & 0xff,
+            "state": rgbtState
+        }
+
+
+    @classmethod
+    def extractRobotStatus(cls, buf: bytes) -> Dict:
+        if len(buf) >= cls.ROS_ROBOT_STATUS_BYTES:
+            robotStat = struct.unpack(">BBIIIIIBB", buf[0:cls.ROS_ROBOT_STATUS_BYTES])
+            return {
+                "flags": robotStat[0],
+                "workQCount": robotStat[1],
+                "isMoving": (robotStat[0] & 0x01) != 0,
+                "isPaused": (robotStat[0] & 0x02) != 0,
+                "isFwUpdating": (robotStat[0] & 0x04) != 0,
+                "heapFree": robotStat[2],
+                "heapMin": robotStat[3],
+                "pixRGBT": list(cls.extractRGBT(robotStat[i+4]) for i in range(3)),
+                "loopMsAvg": robotStat[7],
+                "loopMsMax": robotStat[8]
+            }
+        else:
+            robotStat = struct.unpack(">BB", buf[0:cls.ROS_ROBOT_STATUS_BYTES_MINIMAL])
+            return {
+                "flags": robotStat[0],
+                "workQCount": robotStat[1],
+                "isMoving": (robotStat[0] & 0x01) != 0,
+                "isPaused": (robotStat[0] & 0x02) != 0,
+                "isFwUpdating": (robotStat[0] & 0x04) != 0,
+            }
+
+    @classmethod
+    def extractAddOnStatus(cls, buf: bytes) -> List:
+        #  Each group of attributes for an add-on is a fixed size
+        numGroups = math.floor(len(buf) / cls.ROS_ADDON_GROUP_BYTES)
+        addOns = {}
+        bufPos = 0
+        for _ in range(numGroups):
+            adb = buf[bufPos:bufPos+cls.ROS_ADDON_GROUP_BYTES]
+            addOns[adb[0]] = {
+                "IDNo": adb[0],
+                "valid": (adb[1] & 0x80) != 0,
+                "data": adb[2:]
+            }
+            bufPos += cls.ROS_ADDON_GROUP_BYTES
+        return addOns
```

### Comparing `martypy-3.4.3/martypy/RateAverager.py` & `martypy-3.5.0/martypy/RateAverager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import time
-
-class RateAverager:
-    
-    def __init__(self, windowSizeMinSecs = 1):
-        self.sampleCount = 0
-        self.windowSizeMinSecs = windowSizeMinSecs
-        self.lastCalcSecs = time.time()
-        self.prevVal = 0
-        self.totalCount = 0
-
-    def addSample(self):
-        self.sampleCount += 1
-        self.totalCount += 1
-
-    def getAvg(self):
-        if self.lastCalcSecs + self.windowSizeMinSecs < time.time():
-            rsltVal = self.sampleCount / (time.time() - self.lastCalcSecs)
-            self.lastCalcSecs = time.time()
-            self.sampleCount = 0
-            self.prevVal = rsltVal
-            return rsltVal
-        return self.prevVal
-
-    def getTotal(self):
-        return self.totalCount
+import time
+
+class RateAverager:
+    
+    def __init__(self, windowSizeMinSecs = 1):
+        self.sampleCount = 0
+        self.windowSizeMinSecs = windowSizeMinSecs
+        self.lastCalcSecs = time.time()
+        self.prevVal = 0
+        self.totalCount = 0
+
+    def addSample(self):
+        self.sampleCount += 1
+        self.totalCount += 1
+
+    def getAvg(self):
+        if self.lastCalcSecs + self.windowSizeMinSecs < time.time():
+            rsltVal = self.sampleCount / (time.time() - self.lastCalcSecs)
+            self.lastCalcSecs = time.time()
+            self.sampleCount = 0
+            self.prevVal = rsltVal
+            return round(rsltVal,2)
+        return round(self.prevVal,2)
+
+    def getTotal(self):
+        return self.totalCount
```

### Comparing `martypy-3.4.3/martypy/WebSocket.py` & `martypy-3.5.0/martypy/WebSocket.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,152 +1,163 @@
-
-import socket
-import logging
-from typing import Callable, Optional
-from .WebSocketFrame import WebSocketFrame
-import time
-
-logger = logging.getLogger(__name__)
-# logger.setLevel(logging.DEBUG)
-
-class WebSocket():
-
-    maxSocketBytes = 2000
-    MAX_RX_PREUPGRADE_LEN = 2000
-    SOCKET_AWAITING_UPGRADE = 0
-    SOCKET_UPGRADED = 1
-
-    def __init__(self,
-            onBinaryFrame: Callable[[bytes], None],
-            onTextFrame: Callable[[str], None],
-            onError: Callable[[str], None],
-            onReconnect: Callable[[], None],
-            ipAddrOrHostname: str,
-            ipPort: int = 80,
-            wsPath: str = "/ws",
-            timeout: float = 5.0,
-            autoReconnect: bool = True,
-            reconnectRepeatSecs: int = 5.0) -> None:
-        self.ipAddr = socket.gethostbyname(ipAddrOrHostname)
-        self.wsPath = wsPath
-        self.ipPort = ipPort
-        self.timeout = timeout
-        self.autoReconnect = autoReconnect
-        self.reconnectRepeatSecs = reconnectRepeatSecs
-        self.onBinaryFrame = onBinaryFrame
-        self.onTextFrame = onTextFrame
-        self.onError = onError
-        self.onReconnect = onReconnect
-        self._clear()
-
-    def __del__(self) -> None:
-        self.close()
-
-    def open(self) -> bool:
-        # Clear
-        self._clear()
-        # Open socket
-        self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.sock.settimeout(self.timeout)
-        self.sock.connect((self.ipAddr, self.ipPort))
-        # Initiate upgrade
-        self._sendUpgradeReq()
-
-    def writeBinary(self, inFrame: bytes) -> int:
-        if not self.sock:
-            return 0
-        frame = WebSocketFrame.encode(inFrame, False, WebSocketFrame.OPCODE_BINARY, True)
-        # logger.debug(f"WebSocket write {''.join('{:02x}'.format(x) for x in frame)}")
-        return self.sock.send(frame)
-
-    def close(self) -> None:
-        if self.sock:
-            try:
-                self.sock.close()
-            except Exception as excp:
-                logger.debug("WebSocket exception while closing", exc_info=True)
-        self.sock = None
-
-    def _sendUpgradeReq(self) -> None:
-        if not self.sock:
-            return
-        headerStr = f"GET {self.wsPath} HTTP/1.1\r\n" + \
-            "Connection: upgrade\r\n" + \
-            "Upgrade: websocket\r\n" + \
-            "\r\n"
-        self.sock.send(headerStr.encode())
-
-    def service(self) -> None:
-        # Get any data
-        reconnectRequired = False
-        try:
-            rxData = self.sock.recv(self.maxSocketBytes)
-        except Exception as excp:
-            logger.debug("WebSocket exception on recv:", exc_info=True)
-            if not self.autoReconnect:
-                raise excp
-            reconnectRequired = True
-        # Check for reconnect
-        if reconnectRequired:
-            if self.reconnectLastTime is None or time.time() > self.reconnectLastTime + self.reconnectRepeatSecs:
-                self.close()
-                try:
-                    if self.onReconnect:
-                        self.onReconnect()
-                    self.open()
-                    logger.debug("WebSocket reopened automatically")
-                except Exception as excp:
-                    logger.debug("WebSocket exception trying to reopen websocket:", exc_info=True)
-                self.reconnectLastTime = time.time()
-            else:
-                time.sleep(0.01)
-            return
-        if self.sock is None:
-            return
-        # Check state of socket connection
-        if self.socketState == self.SOCKET_AWAITING_UPGRADE:
-            self.rxPreUpgrade += rxData
-            # Check for upgrade header complete
-            headerEndPos = self.rxPreUpgrade.find(b"\r\n\r\n")
-            if headerEndPos > 0:
-                # Check upgrade ok
-                if b"Sec-WebSocket-Accept" in self.rxPreUpgrade:
-                    self.socketState = self.SOCKET_UPGRADED
-                    self.wsFrameCodec.addDataToDecode(self.rxPreUpgrade[headerEndPos+4:])
-                    # logger.debug("WebSocket upgraded")
-            elif len(self.rxPreUpgrade) > self.MAX_RX_PREUPGRADE_LEN:
-                self.rxPreUpgrade.clear()
-        else:
-            self.wsFrameCodec.addDataToDecode(rxData)
-            checkForData = True
-            while checkForData:
-                checkForData = False
-                # Check for actions required
-                if self.wsFrameCodec.getPongRequired():
-                    # logging.debug("WebSocket sending pong")
-                    self._sendPong()
-                    checkForData = True
-                binaryFrame = self.wsFrameCodec.getBinaryMsg()
-                if binaryFrame:
-                    checkForData = True
-                    # logger.debug(f"WebSocket proc binary len {len(binaryFrame)}")
-                    if self.onBinaryFrame:
-                        self.onBinaryFrame(binaryFrame)
-                textFrame = self.wsFrameCodec.getTextMsg()
-                if textFrame and self.onTextFrame:
-                    checkForData = True
-                    self.onTextFrame(textFrame)
-
-    def _sendPong(self) -> None:
-        if not self.sock:
-            return 0
-        frame = WebSocketFrame.encode(self.wsFrameCodec.getPongData(),
-                    False, WebSocketFrame.OPCODE_PONG, True)
-        # logger.debug(f"WebSocket pong {''.join('{:02x}'.format(x) for x in self.wsFrameCodec.getPongData())}")
-        return self.sock.send(frame)
-
-    def _clear(self) -> None:
-        self.sock = None
-        self.socketState = self.SOCKET_AWAITING_UPGRADE
-        self.reconnectLastTime = None
-        self.rxPreUpgrade = bytearray()
-        self.wsFrameCodec = WebSocketFrame()
+
+import socket
+import logging
+from typing import Callable, Optional
+from .WebSocketFrame import WebSocketFrame
+import time
+
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
+
+class WebSocket():
+
+    maxSocketBytes = 2000
+    MAX_RX_PREUPGRADE_LEN = 2000
+    SOCKET_AWAITING_UPGRADE = 0
+    SOCKET_UPGRADED = 1
+
+    def __init__(self,
+            onBinaryFrame: Callable[[bytes], None],
+            onTextFrame: Callable[[str], None],
+            onError: Callable[[str], None],
+            onReconnect: Callable[[], None],
+            ipAddrOrHostname: str,
+            ipPort: int = 80,
+            wsPath: str = "/ws",
+            timeout: float = 5.0,
+            autoReconnect: bool = True,
+            reconnectRepeatSecs: int = 5.0) -> None:
+        self.ipAddr = socket.gethostbyname(ipAddrOrHostname)
+        self.wsPath = wsPath
+        self.ipPort = ipPort
+        self.timeout = timeout
+        self.autoReconnect = autoReconnect
+        self.reconnectRepeatSecs = reconnectRepeatSecs
+        self.onBinaryFrame = onBinaryFrame
+        self.onTextFrame = onTextFrame
+        self.onError = onError
+        self.onReconnect = onReconnect
+        self._clear()
+        # Debug
+        self.DEBUG_WEBSOCKET_OPEN = False
+
+    def __del__(self) -> None:
+        self.close()
+
+    def open(self) -> bool:
+        # Debug
+        debugStartTime = time.time()
+        # Clear
+        self._clear()
+        # Open socket
+        self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self.sock.settimeout(self.timeout)
+        self.sock.connect((self.ipAddr, self.ipPort))
+        # Debug
+        if self.DEBUG_WEBSOCKET_OPEN:
+            logger.debug(f"WebSocket open {self.ipAddr}:{self.ipPort} took {time.time() - debugStartTime}")
+        # Initiate upgrade
+        debugStartTime = time.time()
+        self._sendUpgradeReq()
+        # Debug
+        if self.DEBUG_WEBSOCKET_OPEN:
+            logger.debug(f"WebSocket upgrade {self.ipAddr}:{self.ipPort} took {time.time() - debugStartTime}")
+
+    def writeBinary(self, inFrame: bytes) -> int:
+        if not self.sock:
+            return 0
+        frame = WebSocketFrame.encode(inFrame, False, WebSocketFrame.OPCODE_BINARY, True)
+        # logger.debug(f"WebSocket write {''.join('{:02x}'.format(x) for x in frame)}")
+        return self.sock.send(frame)
+
+    def close(self) -> None:
+        if self.sock:
+            try:
+                self.sock.close()
+            except Exception as excp:
+                logger.debug("WebSocket exception while closing", exc_info=True)
+        self.sock = None
+
+    def _sendUpgradeReq(self) -> None:
+        if not self.sock:
+            return
+        headerStr = f"GET {self.wsPath} HTTP/1.1\r\n" + \
+            "Connection: upgrade\r\n" + \
+            "Upgrade: websocket\r\n" + \
+            "\r\n"
+        self.sock.send(headerStr.encode())
+
+    def service(self) -> None:
+        # Get any data
+        reconnectRequired = False
+        try:
+            rxData = self.sock.recv(self.maxSocketBytes)
+        except Exception as excp:
+            logger.debug("WebSocket exception on recv:", exc_info=True)
+            if not self.autoReconnect:
+                raise excp
+            reconnectRequired = True
+        # Check for reconnect
+        if reconnectRequired:
+            if self.reconnectLastTime is None or time.time() > self.reconnectLastTime + self.reconnectRepeatSecs:
+                self.close()
+                try:
+                    self.open()
+                    if self.onReconnect:
+                        self.onReconnect()
+                    logger.debug("WebSocket reopened automatically")
+                except Exception as excp:
+                    logger.debug("WebSocket exception trying to reopen websocket:", exc_info=True)
+                self.reconnectLastTime = time.time()
+            else:
+                time.sleep(0.01)
+            return
+        if self.sock is None:
+            return
+        # Check state of socket connection
+        if self.socketState == self.SOCKET_AWAITING_UPGRADE:
+            self.rxPreUpgrade += rxData
+            # Check for upgrade header complete
+            headerEndPos = self.rxPreUpgrade.find(b"\r\n\r\n")
+            if headerEndPos > 0:
+                # Check upgrade ok
+                if b"Sec-WebSocket-Accept" in self.rxPreUpgrade:
+                    self.socketState = self.SOCKET_UPGRADED
+                    self.wsFrameCodec.addDataToDecode(self.rxPreUpgrade[headerEndPos+4:])
+                    # logger.debug("WebSocket upgraded")
+            elif len(self.rxPreUpgrade) > self.MAX_RX_PREUPGRADE_LEN:
+                self.rxPreUpgrade.clear()
+        else:
+            self.wsFrameCodec.addDataToDecode(rxData)
+            checkForData = True
+            while checkForData:
+                checkForData = False
+                # Check for actions required
+                if self.wsFrameCodec.getPongRequired():
+                    # logging.debug("WebSocket sending pong")
+                    self._sendPong()
+                    checkForData = True
+                binaryFrame = self.wsFrameCodec.getBinaryMsg()
+                if binaryFrame:
+                    checkForData = True
+                    # logger.debug(f"WebSocket proc binary len {len(binaryFrame)}")
+                    if self.onBinaryFrame:
+                        self.onBinaryFrame(binaryFrame)
+                textFrame = self.wsFrameCodec.getTextMsg()
+                if textFrame and self.onTextFrame:
+                    checkForData = True
+                    self.onTextFrame(textFrame)
+
+    def _sendPong(self) -> None:
+        if not self.sock:
+            return 0
+        frame = WebSocketFrame.encode(self.wsFrameCodec.getPongData(),
+                    False, WebSocketFrame.OPCODE_PONG, True)
+        # logger.debug(f"WebSocket pong {frame.hex()}")
+        return self.sock.send(frame)
+
+    def _clear(self) -> None:
+        self.sock = None
+        self.socketState = self.SOCKET_AWAITING_UPGRADE
+        self.reconnectLastTime = None
+        self.rxPreUpgrade = bytearray()
+        self.wsFrameCodec = WebSocketFrame()
```

### Comparing `martypy-3.4.3/martypy/WebSocketFrame.py` & `martypy-3.5.0/martypy/WebSocketFrame.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,182 @@
-'''
-WebSocketFrame
-'''
-import io
-import struct
-import secrets
-import itertools
-import collections
-import logging
-import time
-from typing import Deque
-
-logger = logging.getLogger(__name__)
-
-class WebSocketFrame():
-
-    max_size = 20000
-    OPCODE_CONT = 0x00
-    OPCODE_TEXT = 0x01
-    OPCODE_BINARY = 0x02
-    OPCODE_CLOSE = 0x08
-    OPCODE_PING = 0x09
-    OPCODE_PONG = 0x0a
-
-    def __init__(self) -> None:
-        self.curInputData: bytearray = bytearray()
-        self.rxFrameData: bytearray = bytearray()
-        self.rxFrameIsText = False
-        self.pongRequired = False
-        self.pongData = bytearray()
-        self.closeRequired = False
-        self.textMsgs: Deque[str] = collections.deque()
-        self.binaryMsgs: Deque[bytes] = collections.deque()
-        self.statsPings = 0
-        self.statsPongs = 0
-        self.statsText = 0
-        self.statsBinary = 0
-
-    def getPongRequired(self) -> bool:
-        tmpPongReq = self.pongRequired
-        self.pongRequired = False
-        return tmpPongReq
-
-    def getPongData(self) -> bytes:
-        return self.pongData
-
-    def getCloseRequired(self) -> bool:
-        return self.closeRequired
-
-    def getTextMsg(self) -> str:
-        if len(self.textMsgs) > 0:
-            return self.textMsgs.popleft()
-        return None
-
-    def getBinaryMsg(self) -> bytes:
-        if len(self.binaryMsgs) > 0:
-            binaryMsg = self.binaryMsgs.popleft()
-            return binaryMsg
-        return None
-
-    def addDataToDecode(self, data: bytes) -> None:
-        '''
-        Add data to be decoded
-        Args:
-            data bytes to add
-        Returns:
-            None
-        '''
-        # Add data
-        self.curInputData += data
-        # logger.debug(f"{''.join('{:02x}'.format(x) for x in data)}")
-        while self._extractFrames():
-            pass
-
-    def _extractFrames(self) -> bool:
-        if len(self.curInputData) < 2:
-            return False
-        head1, head2 = struct.unpack("!BB", self.curInputData[:2])
-
-        # Extract header info
-        fin = (head1 & 0b10000000) != 0
-        opcode = head1 & 0b00001111
-        mask = (head2 & 0b10000000) != 0
-        frameLen = head2 & 0b01111111
-        curPos = 2
-        if frameLen == 126:
-            if len(self.curInputData) < 4:
-                return False
-            (frameLen,) = struct.unpack("!H", self.curInputData[2:4])
-            curPos = 4
-        elif frameLen == 127:
-            if len(self.curInputData) < 10:
-                return False
-            (frameLen,) = struct.unpack("!Q", self.curInputData[2:10])
-            curPos = 10
-        if frameLen > self.max_size:
-            self.curInputData.clear()
-            return False
-        if mask and len(self.curInputData) < curPos + 4:
-            return False
-        if mask:
-            self.mask_bytes = self.curInputData[curPos:curPos+4]
-            curPos += 4
-
-        # Check data is present
-        if len(self.curInputData) < curPos + frameLen:
-            return False
-        rxDataBlock = self.curInputData[curPos : curPos + frameLen]
-        if mask:
-            rxDataBlock = self.applyMask(rxDataBlock, self.mask_bytes)
-        
-        # Remove data consumed
-        self.curInputData = self.curInputData[curPos + frameLen:]
-
-        # Check for pings
-        if opcode == self.OPCODE_PING:
-            self.pongRequired = True
-            self.pongData = rxDataBlock
-            self.statsPings += 1
-            # logger.debug(f"wsFrame PING {''.join('{:02x}'.format(x) for x in rxDataBlock)}")
-            return True
-        elif opcode == self.OPCODE_PONG:
-            self.statsPongs += 1
-            # logger.debug(f"wsFrame PONG {''.join('{:02x}'.format(x) for x in rxDataBlock)}")
-            return True
-        elif opcode == self.OPCODE_CLOSE:
-            # logger.debug(f"wsFrame CLOSE")
-            self.closeRequired = True
-            return True
-        elif opcode == self.OPCODE_BINARY:
-            # logger.debug(f"wsFrame BINARY PART {''.join('{:02x}'.format(x) for x in rxDataBlock)}")
-            self.rxFrameIsText = False
-        elif opcode == self.OPCODE_TEXT:
-            # logger.debug(f"wsFrame TEXT PART {''.join('{:02x}'.format(x) for x in rxDataBlock)}")
-            self.rxFrameIsText = True
-
-        # Add data to received frame
-        self.rxFrameData += rxDataBlock
-
-        # Add completed frame to queue
-        if fin:
-            if self.rxFrameIsText:
-                self.textMsgs.append(self.rxFrameData.decode('utf-8'))
-                self.statsText += 1
-            else:
-                # logger.debug(f"wsFrame BINARY DONE {''.join('{:02x}'.format(x) for x in self.rxFrameData)}")
-                self.binaryMsgs.append(self.rxFrameData[:])
-                self.statsBinary += 1
-            self.rxFrameData.clear()
-        return True
-
-    @classmethod
-    def encode(self, inFrame: bytes, useMask: bool,
-                opcode: int, fin: bool) -> bytes:
-
-        output = io.BytesIO()
-
-        # Prepare the header.
-        head1 = 0b10000000 if fin else 0 | opcode
-        head2 = 0b10000000 if useMask else 0
-        length = len(inFrame)
-        if length < 126:
-            output.write(struct.pack("!BB", head1, head2 | length))
-        elif length < 65536:
-            output.write(struct.pack("!BBH", head1, head2 | 126, length))
-        else:
-            output.write(struct.pack("!BBQ", head1, head2 | 127, length))
-
-        if useMask:
-            mask_bytes = secrets.token_bytes(4)
-            output.write(mask_bytes)
-            data = self.applyMask(inFrame, mask_bytes)
-        else:
-            data = inFrame
-        output.write(data)
-        return output.getvalue()
-
-    @classmethod
-    def applyMask(cls, data: bytes, mask: bytes) -> bytes:
-        if len(mask) != 4:
-            return
-        return bytes(b ^ m for b, m in zip(data, itertools.cycle(mask)))
+'''
+WebSocketFrame
+'''
+import io
+import struct
+import secrets
+import itertools
+import collections
+import logging
+import time
+from typing import Deque
+
+logger = logging.getLogger(__name__)
+
+class WebSocketFrame():
+
+    max_size = 20000
+    OPCODE_CONT = 0x00
+    OPCODE_TEXT = 0x01
+    OPCODE_BINARY = 0x02
+    OPCODE_CLOSE = 0x08
+    OPCODE_PING = 0x09
+    OPCODE_PONG = 0x0a
+
+    def __init__(self) -> None:
+        self.curInputData: bytearray = bytearray()
+        self.rxFrameData: bytearray = bytearray()
+        self.rxFrameIsText = False
+        self.pongRequired = False
+        self.pongData = bytearray()
+        self.closeRequired = False
+        self.textMsgs: Deque[str] = collections.deque()
+        self.binaryMsgs: Deque[bytes] = collections.deque()
+        self.statsPings = 0
+        self.statsPongs = 0
+        self.statsText = 0
+        self.statsBinary = 0
+
+    def getPongRequired(self) -> bool:
+        tmpPongReq = self.pongRequired
+        self.pongRequired = False
+        return tmpPongReq
+
+    def getPongData(self) -> bytes:
+        return self.pongData
+
+    def getCloseRequired(self) -> bool:
+        return self.closeRequired
+
+    def getTextMsg(self) -> str:
+        if len(self.textMsgs) > 0:
+            return self.textMsgs.popleft()
+        return None
+
+    def getBinaryMsg(self) -> bytes:
+        if len(self.binaryMsgs) > 0:
+            binaryMsg = self.binaryMsgs.popleft()
+            return binaryMsg
+        return None
+
+    def addDataToDecode(self, data: bytes) -> None:
+        '''
+        Add data to be decoded
+        Args:
+            data bytes to add
+        Returns:
+            None
+        '''
+        # Add data
+        self.curInputData += data
+        # logger.debug(f"{''.join('{:02x}'.format(x) for x in data)}")
+        while self._extractFrames():
+            pass
+
+    def _extractFrames(self) -> bool:
+        if len(self.curInputData) < 2:
+            return False
+        head1, head2 = struct.unpack("!BB", self.curInputData[:2])
+
+        # Extract header info
+        fin = (head1 & 0b10000000) != 0
+        opcode = head1 & 0b00001111
+        mask = (head2 & 0b10000000) != 0
+        frameLen = head2 & 0b01111111
+        curPos = 2
+        if frameLen == 126:
+            if len(self.curInputData) < 4:
+                return False
+            (frameLen,) = struct.unpack("!H", self.curInputData[2:4])
+            curPos = 4
+        elif frameLen == 127:
+            if len(self.curInputData) < 10:
+                return False
+            (frameLen,) = struct.unpack("!Q", self.curInputData[2:10])
+            curPos = 10
+        if frameLen > self.max_size:
+            self.curInputData.clear()
+            return False
+        if mask and len(self.curInputData) < curPos + 4:
+            return False
+        if mask:
+            self.mask_bytes = self.curInputData[curPos:curPos+4]
+            curPos += 4
+
+        # Check data is present
+        if len(self.curInputData) < curPos + frameLen:
+            return False
+        rxDataBlock = self.curInputData[curPos : curPos + frameLen]
+        if mask:
+            rxDataBlock = self.applyMask(rxDataBlock, self.mask_bytes)
+        
+        # Remove data consumed
+        self.curInputData = self.curInputData[curPos + frameLen:]
+
+        # Check for pings
+        if opcode == self.OPCODE_PING:
+            self.pongRequired = True
+            self.pongData = rxDataBlock
+            self.statsPings += 1
+            # logger.debug(f"wsFrame PING {''.join('{:02x}'.format(x) for x in rxDataBlock)}")
+            return True
+        elif opcode == self.OPCODE_PONG:
+            self.statsPongs += 1
+            # logger.debug(f"wsFrame PONG {''.join('{:02x}'.format(x) for x in rxDataBlock)}")
+            return True
+        elif opcode == self.OPCODE_CLOSE:
+            # logger.debug(f"wsFrame CLOSE")
+            self.closeRequired = True
+            return True
+        elif opcode == self.OPCODE_BINARY:
+            # logger.debug(f"wsFrame BINARY PART {''.join('{:02x}'.format(x) for x in rxDataBlock)}")
+            self.rxFrameIsText = False
+        elif opcode == self.OPCODE_TEXT:
+            # logger.debug(f"wsFrame TEXT PART {''.join('{:02x}'.format(x) for x in rxDataBlock)}")
+            self.rxFrameIsText = True
+
+        # Add data to received frame
+        self.rxFrameData += rxDataBlock
+
+        # Add completed frame to queue
+        if fin:
+            if self.rxFrameIsText:
+                self.textMsgs.append(self.rxFrameData.decode('utf-8'))
+                self.statsText += 1
+            else:
+                # logger.debug(f"wsFrame BINARY DONE {''.join('{:02x}'.format(x) for x in self.rxFrameData)}")
+                self.binaryMsgs.append(self.rxFrameData[:])
+                self.statsBinary += 1
+            self.rxFrameData.clear()
+        return True
+
+    @classmethod
+    def encode(self, inFrame: bytes, useMask: bool,
+                opcode: int, fin: bool) -> bytes:
+
+        output = io.BytesIO()
+
+        # Prepare the header.
+        head1 = (0b10000000 if fin else 0) | opcode
+        head2 = 0b10000000 if useMask else 0
+        length = len(inFrame)
+        if length < 126:
+            output.write(struct.pack("!BB", head1, head2 | length))
+        elif length < 65536:
+            output.write(struct.pack("!BBH", head1, head2 | 126, length))
+        else:
+            output.write(struct.pack("!BBQ", head1, head2 | 127, length))
+
+        if useMask:
+            mask_bytes = secrets.token_bytes(4)
+            output.write(mask_bytes)
+            data = self.applyMask(inFrame, mask_bytes)
+        else:
+            data = inFrame
+        output.write(data)
+        return output.getvalue()
+
+    @classmethod
+    def applyMask(cls, data: bytes, mask: bytes) -> bytes:
+        if len(mask) != 4:
+            return
+        return bytes(b ^ m for b, m in zip(data, itertools.cycle(mask)))
```

### Comparing `martypy-3.4.3/martypy/tests/testBaudRateSelection.py` & `martypy-3.5.0/martypy/tests/testBaudRateSelection.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import sys
-import logging
-
-import pathlib
-cur_path = pathlib.Path(__file__).parent.resolve()
-sys.path.insert(0, str(cur_path.parent.parent.resolve()))
-
-from martypy import Marty
-import time
-
-# Setup logging
-logging.basicConfig(format='%(levelname)s: %(asctime)s %(funcName)s(%(lineno)d) -- %(message)s', level=logging.DEBUG)
-logger = logging.getLogger("testBaudRateSelection")
-
-mm = Marty("usb")
-# try:
-# mm = Marty("wifi://192.168.86.81")
-# except Exception as excp:
-#     print(f"Couldn't connect to marty")
-#     exit()
-
-# mm.eyes(100)
-# mm.eyes(0)
-
-logger.info(f"RIC version info 1: {mm.get_system_info()}")
-mm.circle_dance()
-logger.info(f"RIC version info 2: {mm.get_system_info()}")
-time.sleep(5)
-logger.info(f"RIC version info 3: {mm.get_system_info()}")
-
-mm.close()
+import sys
+import logging
+
+import pathlib
+cur_path = pathlib.Path(__file__).parent.resolve()
+sys.path.insert(0, str(cur_path.parent.parent.resolve()))
+
+from martypy import Marty
+import time
+
+# Setup logging
+logging.basicConfig(format='%(levelname)s: %(asctime)s %(funcName)s(%(lineno)d) -- %(message)s', level=logging.DEBUG)
+logger = logging.getLogger("testBaudRateSelection")
+
+mm = Marty("usb")
+# try:
+# mm = Marty("wifi://192.168.86.81")
+# except Exception as excp:
+#     print(f"Couldn't connect to marty")
+#     exit()
+
+# mm.eyes(100)
+# mm.eyes(0)
+
+logger.info(f"RIC version info 1: {mm.get_system_info()}")
+mm.circle_dance()
+logger.info(f"RIC version info 2: {mm.get_system_info()}")
+time.sleep(5)
+logger.info(f"RIC version info 3: {mm.get_system_info()}")
+
+mm.close()
```

### Comparing `martypy-3.4.3/martypy/tests/testColourSensor.py` & `martypy-3.5.0/martypy/tests/testColourSensor.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import sys    
-import logging
-
-import pathlib
-cur_path = pathlib.Path(__file__).parent.resolve()
-sys.path.insert(0, str(cur_path.parent.parent.resolve()))
-
-from martypy import Marty
-import time
-
-# Setup logging
-logging.basicConfig(format='%(levelname)s: %(asctime)s %(funcName)s(%(lineno)d) -- %(message)s', level=logging.DEBUG)
-logger = logging.getLogger("testColourSensor")
-handler = logging.StreamHandler(sys.stdout)
-handler.setLevel(logging.DEBUG)
-logger.addHandler(handler)
-
-mm = Marty("usb")
-
-# time.sleep(2)
-
-for i in range(100):
-    try:
-        onGroundL = mm.foot_on_ground('left')
-        onGroundR = mm.foot_on_ground('right')
-        obstacleL = mm.foot_obstacle_sensed('left')
-        obstacleR = mm.foot_obstacle_sensed('right')
-        obstSensorL = mm.get_obstacle_sensor_reading('left')
-        obstSensorR = mm.get_obstacle_sensor_reading('right')
-        groundSensorL = mm.get_ground_sensor_reading('left')
-        groundSensorR = mm.get_ground_sensor_reading('right')
-        print(
-            f"onGroundL={onGroundL!s:<5} onGroundR={onGroundR!s:<5} | "
-            f"obstacleL={obstacleL!s:<5} obstacleR={obstacleR!s:<5} || "
-            f"obstSensorL={obstSensorL:5} obstSensorR={obstSensorR:5} | "
-            f"groundSensorL={groundSensorL:5} groundSensorR={groundSensorR:5}"
-        )
-    except Exception as e:
-        logger.exception(f"Failed to get addon values")        
-    time.sleep(.2)
-
-# try:
-# mm = Marty("wifi://192.168.86.81")
-# except Exception as excp:
-#     print(f"Couldn't connect to marty")
-#     exit()
-
-
-# time.sleep(5)
-
-mm.close()
+import sys    
+import logging
+
+import pathlib
+cur_path = pathlib.Path(__file__).parent.resolve()
+sys.path.insert(0, str(cur_path.parent.parent.resolve()))
+
+from martypy import Marty
+import time
+
+# Setup logging
+logging.basicConfig(format='%(levelname)s: %(asctime)s %(funcName)s(%(lineno)d) -- %(message)s', level=logging.DEBUG)
+logger = logging.getLogger("testColourSensor")
+handler = logging.StreamHandler(sys.stdout)
+handler.setLevel(logging.DEBUG)
+logger.addHandler(handler)
+
+mm = Marty("usb")
+
+# time.sleep(2)
+
+for i in range(100):
+    try:
+        onGroundL = mm.foot_on_ground('left')
+        onGroundR = mm.foot_on_ground('right')
+        obstacleL = mm.foot_obstacle_sensed('left')
+        obstacleR = mm.foot_obstacle_sensed('right')
+        obstSensorL = mm.get_obstacle_sensor_reading('left')
+        obstSensorR = mm.get_obstacle_sensor_reading('right')
+        groundSensorL = mm.get_ground_sensor_reading('left')
+        groundSensorR = mm.get_ground_sensor_reading('right')
+        print(
+            f"onGroundL={onGroundL!s:<5} onGroundR={onGroundR!s:<5} | "
+            f"obstacleL={obstacleL!s:<5} obstacleR={obstacleR!s:<5} || "
+            f"obstSensorL={obstSensorL:5} obstSensorR={obstSensorR:5} | "
+            f"groundSensorL={groundSensorL:5} groundSensorR={groundSensorR:5}"
+        )
+    except Exception as e:
+        logger.exception(f"Failed to get addon values")        
+    time.sleep(.2)
+
+# try:
+# mm = Marty("wifi://192.168.86.81")
+# except Exception as excp:
+#     print(f"Couldn't connect to marty")
+#     exit()
+
+
+# time.sleep(5)
+
+mm.close()
```

### Comparing `martypy-3.4.3/martypy/tests/test_martypy.py` & `martypy-3.5.0/martypy/tests/test_martypy.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import pytest
-import time
-import sys
-import pathlib
-cur_path = pathlib.Path(__file__).parent.resolve()
-sys.path.insert(0, str(cur_path.parent.parent.resolve()))
-from martypy import Marty
-
-def test_close() -> None:
-    marty = Marty("test", "", blocking=True)
-    time.sleep(6)
-    marty.close()
-    testOutput = marty.get_test_output()
-    testExpected = {"buf":
-            [
-                bytearray(b'\x01\x02\x00v\x00'), 
-                bytearray(b'\x02\x02\x00hwstatus\x00'),
-                bytearray(b'\x03\x02\x03{"cmdName":"subscription","action":"update","pubRecs":[{"name":"MultiStatus","rateHz":10.0,}{"name":"PowerStatus","rateHz":1.0},{"name":"AddOnStatus","rateHz":10.0}]}\x00\x00'), 
-                bytearray(b'\x04\x02\x03{"cmdName":"subscription","action":"update","pubRecs":[{"name":"MultiStatus","rateHz":0},{"name":"PowerStatus","rateHz":0},{"name":"AddOnStatus","rateHz":0}]}\x00\x00')
-            ]
-        }
-    assert(testOutput==testExpected)
-
-def test_circle_dance() -> None:
-    marty = Marty("test","",subscribeRateHz=0)
-    marty.circle_dance()
-    testOutput = marty.get_test_output()
-    testExpected = {"buf":
-            [
-                bytearray(b'\x01\x02\x00v\x00'),
-                bytearray(b'\x02\x02\x00hwstatus\x00'),
-                bytearray(b'\x03\x02\x00traj/circle?side=0&moveTime=1500\x00')
-            ]
-        }
-    assert(testOutput==testExpected)
-
+import pytest
+import time
+import sys
+import pathlib
+cur_path = pathlib.Path(__file__).parent.resolve()
+sys.path.insert(0, str(cur_path.parent.parent.resolve()))
+from martypy import Marty
+
+def test_close() -> None:
+    marty = Marty("test", "", blocking=True)
+    time.sleep(6)
+    marty.close()
+    testOutput = marty.get_test_output()
+    testExpected = {"buf":
+            [
+                bytearray(b'\x01\x02\x00v\x00'), 
+                bytearray(b'\x02\x02\x00hwstatus\x00'),
+                bytearray(b'\x03\x02\x03{"cmdName":"subscription","action":"update","pubRecs":[{"name":"MultiStatus","rateHz":10.0,}{"name":"PowerStatus","rateHz":1.0},{"name":"AddOnStatus","rateHz":10.0}]}\x00\x00'), 
+                bytearray(b'\x04\x02\x03{"cmdName":"subscription","action":"update","pubRecs":[{"name":"MultiStatus","rateHz":0},{"name":"PowerStatus","rateHz":0},{"name":"AddOnStatus","rateHz":0}]}\x00\x00')
+            ]
+        }
+    assert(testOutput==testExpected)
+
+def test_circle_dance() -> None:
+    marty = Marty("test","",subscribeRateHz=0)
+    marty.circle_dance()
+    testOutput = marty.get_test_output()
+    testExpected = {"buf":
+            [
+                bytearray(b'\x01\x02\x00v\x00'),
+                bytearray(b'\x02\x02\x00hwstatus\x00'),
+                bytearray(b'\x03\x02\x00traj/circle?side=0&moveTime=1500\x00')
+            ]
+        }
+    assert(testOutput==testExpected)
+
```

### Comparing `martypy-3.4.3/martypy/tests/testrob.py` & `martypy-3.5.0/martypy/tests/testrob.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-import time
-import logging
-import os
-import sys
-import json
-import pathlib
-cur_path = pathlib.Path(__file__).parent.resolve()
-sys.path.insert(0, str(cur_path.parent.parent.resolve()))
-from martypy import Marty
-
-jointNames = [
-    'left hip',
-    'left twist',
-    'left knee',
-    'right hip',
-    'right twist',
-    'right knee',
-    'left arm',
-    'right arm', 
-    'eyes'   
-]
-
-def betweenCommands():
-    time.sleep(3)
-
-def testBoolCmd(cmdStr: str, cmdRslt: bool):
-    logger.info(f"{cmdStr}, rslt = {cmdRslt}")
-    betweenCommands()
-
-def loggingCB(logStr: str) -> None:
-    logger.debug(logStr)
-
-# Check the log folder exists
-logsFolder = "logs"
-if not os.path.exists(logsFolder):
-    os.mkdir(logsFolder)
-
-# Log file name
-logFileName = "MartyPyLogTest_" + time.strftime("%Y%m%d-%H%M%S") + ".log"
-logFileName = os.path.join(logsFolder, logFileName)
-print("Logging to file " + logFileName)
-
-# Setup logging
-logging.basicConfig(filename=logFileName, format='%(levelname)s: %(asctime)s %(funcName)s(%(lineno)d) -- %(message)s', level=logging.DEBUG)
-logger = logging.getLogger("MartyPyTest")
-handler = logging.StreamHandler(sys.stdout)
-handler.setLevel(logging.DEBUG)
-logger.addHandler(handler)
-
-mymarty = None
-try:
-    # mymarty = Marty('wifi', '192.168.86.11')
-    # mymarty = Marty('wifi', '192.168.86.11', subscribeRateHz=0)
-    mymarty = Marty('wifi://192.168.86.18', blocking=True)
-    # mymarty = Marty("usb", "COM9", debug=True)
-    # mymarty = Marty('usb:///dev/tty.SLAB_USBtoUART', debug=True)
-except Exception as excp:
-    logger.debug(f"Couldn't connect to marty {excp}")
-    exit()
-
-mymarty.register_logging_callback(loggingCB)
-
-martySysInfo = mymarty.get_system_info()
-martyVersion2 = martySysInfo.get("HardwareVersion", "1.0") == "2.0"
-
-if martyVersion2:
-    logger.info(f"Marty has {len(mymarty.get_hw_elems_list())} hardware parts")
-
-if martyVersion2:
-    logger.info(f"Calibration flag {mymarty.is_calibrated()}")
-testBoolCmd("Calibration flag clear", mymarty.clear_calibration())
-if martyVersion2:
-    logger.info(f"Calibration flag should be False ... {mymarty.is_calibrated()}")
-    assert not mymarty.is_calibrated()
-testBoolCmd("Calibration flag set", mymarty.save_calibration())
-if martyVersion2:
-    logger.info(f"Calibration flag should be True ... {mymarty.is_calibrated()}")
-time.sleep(0.1)
-if martyVersion2:
-    assert mymarty.is_calibrated()
-
-logger.info(f"Marty interface stats {json.dumps(mymarty.get_interface_stats())}")
-
-testBoolCmd("Get ready", mymarty.get_ready())
-testBoolCmd("Circle Dance", mymarty.circle_dance())
-testBoolCmd("Eyes excited", mymarty.eyes('excited'))
-testBoolCmd("Eyes wide", mymarty.eyes('wide'))
-testBoolCmd("Eyes angry", mymarty.eyes('angry'))
-testBoolCmd("Eyes normal", mymarty.eyes('normal'))
-testBoolCmd("Kick left", mymarty.kick('left'))
-testBoolCmd("Kick right", mymarty.kick('right'))
-testBoolCmd("Stop", mymarty.stop())
-testBoolCmd("Arms 45", mymarty.arms(45, 45, 500))
-testBoolCmd("Arms 0", mymarty.arms(0, 0, 500))
-
-testBoolCmd("Arms 0", mymarty.play_sound("disbelief"))
-testBoolCmd("Arms 0", mymarty.play_sound("excited"))
-testBoolCmd("Arms 0", mymarty.play_sound("screenfree"))
-
-logger.info(f"Marty interface stats {json.dumps(mymarty.get_interface_stats())}")
-
-for i in range(9): 
-    testBoolCmd(f"Move joint {i}", mymarty.move_joint(i, i * 10, 500))
-for jointName in jointNames: 
-    testBoolCmd(f"Move joint {jointName}", mymarty.move_joint(jointName, 123, 500))
-
-logger.info(f"Accelerometer x {mymarty.get_accelerometer('x')}")
-logger.info(f"Accelerometer y { mymarty.get_accelerometer('y')}")
-logger.info(f"Accelerometer z { mymarty.get_accelerometer('z')}")
-
-if martyVersion2:
-    testBoolCmd("Dance", mymarty.dance())
-    testBoolCmd("Eyes wiggle", mymarty.eyes('wiggle'))
-    testBoolCmd("Hold position", mymarty.hold_position(6000))
-    testBoolCmd("is_moving", mymarty.is_moving())
-    logger.info("Joint positions: ", [mymarty.get_joint_position(pos) for pos in range(9)])
-
-time.sleep(5)
-
-mymarty.close()
+import time
+import logging
+import os
+import sys
+import json
+import pathlib
+cur_path = pathlib.Path(__file__).parent.resolve()
+sys.path.insert(0, str(cur_path.parent.parent.resolve()))
+from martypy import Marty
+
+jointNames = [
+    'left hip',
+    'left twist',
+    'left knee',
+    'right hip',
+    'right twist',
+    'right knee',
+    'left arm',
+    'right arm', 
+    'eyes'   
+]
+
+def betweenCommands():
+    time.sleep(3)
+
+def testBoolCmd(cmdStr: str, cmdRslt: bool):
+    logger.info(f"{cmdStr}, rslt = {cmdRslt}")
+    betweenCommands()
+
+def loggingCB(logStr: str) -> None:
+    logger.debug(logStr)
+
+# Check the log folder exists
+logsFolder = "logs"
+if not os.path.exists(logsFolder):
+    os.mkdir(logsFolder)
+
+# Log file name
+logFileName = "MartyPyLogTest_" + time.strftime("%Y%m%d-%H%M%S") + ".log"
+logFileName = os.path.join(logsFolder, logFileName)
+print("Logging to file " + logFileName)
+
+# Setup logging
+logging.basicConfig(filename=logFileName, format='%(levelname)s: %(asctime)s %(funcName)s(%(lineno)d) -- %(message)s', level=logging.DEBUG)
+logger = logging.getLogger("MartyPyTest")
+handler = logging.StreamHandler(sys.stdout)
+handler.setLevel(logging.DEBUG)
+logger.addHandler(handler)
+
+mymarty = None
+try:
+    # mymarty = Marty('wifi', '192.168.86.11')
+    # mymarty = Marty('wifi', '192.168.86.11', subscribeRateHz=0)
+    mymarty = Marty('wifi://192.168.86.18', blocking=True)
+    # mymarty = Marty("usb", "COM9", debug=True)
+    # mymarty = Marty('usb:///dev/tty.SLAB_USBtoUART', debug=True)
+except Exception as excp:
+    logger.debug(f"Couldn't connect to marty {excp}")
+    exit()
+
+mymarty.register_logging_callback(loggingCB)
+
+martySysInfo = mymarty.get_system_info()
+martyVersion2 = martySysInfo.get("HardwareVersion", "1.0") == "2.0"
+
+if martyVersion2:
+    logger.info(f"Marty has {len(mymarty.get_hw_elems_list())} hardware parts")
+
+if martyVersion2:
+    logger.info(f"Calibration flag {mymarty.is_calibrated()}")
+testBoolCmd("Calibration flag clear", mymarty.clear_calibration())
+if martyVersion2:
+    logger.info(f"Calibration flag should be False ... {mymarty.is_calibrated()}")
+    assert not mymarty.is_calibrated()
+testBoolCmd("Calibration flag set", mymarty.save_calibration())
+if martyVersion2:
+    logger.info(f"Calibration flag should be True ... {mymarty.is_calibrated()}")
+time.sleep(0.1)
+if martyVersion2:
+    assert mymarty.is_calibrated()
+
+logger.info(f"Marty interface stats {json.dumps(mymarty.get_interface_stats())}")
+
+testBoolCmd("Get ready", mymarty.get_ready())
+testBoolCmd("Circle Dance", mymarty.circle_dance())
+testBoolCmd("Eyes excited", mymarty.eyes('excited'))
+testBoolCmd("Eyes wide", mymarty.eyes('wide'))
+testBoolCmd("Eyes angry", mymarty.eyes('angry'))
+testBoolCmd("Eyes normal", mymarty.eyes('normal'))
+testBoolCmd("Kick left", mymarty.kick('left'))
+testBoolCmd("Kick right", mymarty.kick('right'))
+testBoolCmd("Stop", mymarty.stop())
+testBoolCmd("Arms 45", mymarty.arms(45, 45, 500))
+testBoolCmd("Arms 0", mymarty.arms(0, 0, 500))
+
+testBoolCmd("Arms 0", mymarty.play_sound("disbelief"))
+testBoolCmd("Arms 0", mymarty.play_sound("excited"))
+testBoolCmd("Arms 0", mymarty.play_sound("screenfree"))
+
+logger.info(f"Marty interface stats {json.dumps(mymarty.get_interface_stats())}")
+
+for i in range(9): 
+    testBoolCmd(f"Move joint {i}", mymarty.move_joint(i, i * 10, 500))
+for jointName in jointNames: 
+    testBoolCmd(f"Move joint {jointName}", mymarty.move_joint(jointName, 123, 500))
+
+logger.info(f"Accelerometer x {mymarty.get_accelerometer('x')}")
+logger.info(f"Accelerometer y { mymarty.get_accelerometer('y')}")
+logger.info(f"Accelerometer z { mymarty.get_accelerometer('z')}")
+
+if martyVersion2:
+    testBoolCmd("Dance", mymarty.dance())
+    testBoolCmd("Eyes wiggle", mymarty.eyes('wiggle'))
+    testBoolCmd("Hold position", mymarty.hold_position(6000))
+    testBoolCmd("is_moving", mymarty.is_moving())
+    logger.info("Joint positions: ", [mymarty.get_joint_position(pos) for pos in range(9)])
+
+time.sleep(5)
+
+mymarty.close()
```

### Comparing `martypy-3.4.3/martypy.egg-info/PKG-INFO` & `martypy-3.5.0/martypy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,63 @@
-Metadata-Version: 2.1
-Name: martypy
-Version: 3.4.3
-Summary: Python library for Marty the Robot V1 and V2
-Home-page: http://github.com/robotical/martypy
-Author: Robotical
-Author-email: hello@robotical.io
-Maintainer: Robotical
-Maintainer-email: hello@robotical.io
-License: Apache 2.0
-Keywords: ros,robot,marty,marty the robot,robotical
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: Apache Software License
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE.md
-
-# martypy
-
-Python library to communicate with Marty the Robot V1 and V2 by Robotical
-
-[See the API Documentation](https://userguides.robotical.io/martyv2/documentation/python_function_reference)
-
-To regenerate documentation:
-- pip install -r dev-requirements.txt
-- pydoc-markdown --server --open
-
-## How to run example scripts
-
-If you cloned the repository or downloaded the source code to try the [example scripts](examples),
-you will need to make sure you have MartyPy installed before you can run the examples.
-
-The easiest way to install MartyPy is with the `pip install martypy` script as explained in
-[step 2 here](https://userguides.robotical.io/martyv2/userguides/python/setting_up_python_on_your_computer).
-
-If you would like to make modifications to the martypy library itself, it will be better to install
-it from source using the command `pip install --editable /path/to/martypy/repo` (replacing
-`/path/to/martypy/repo` as appropriate of course).
-
-If you do not want to "`pip install`" the MartyPy library, you can add the following 4 lines at the
-top (before any other code) of each script you want to run:
-
-```python
-import sys
-import pathlib
-cur_path = pathlib.Path(__file__).parent.resolve()
-sys.path.append(str(cur_path.parent.resolve()))
-```
+Metadata-Version: 2.1
+Name: martypy
+Version: 3.5.0
+Summary: Python library for Marty the Robot V1 and V2
+Home-page: http://github.com/robotical/martypy
+Author: Robotical
+Author-email: hello@robotical.io
+Maintainer: Robotical
+Maintainer-email: hello@robotical.io
+License: Apache 2.0
+Keywords: ros,robot,marty,marty the robot,robotical
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+License-File: LICENSE.md
+
+# martypy
+
+Python library to communicate with Marty the Robot V1 and V2 by Robotical
+
+[See the API Documentation](https://userguides.robotical.io/martyv2/documentation/python_function_reference)
+
+To regenerate documentation:
+- pip install -r dev-requirements.txt
+- pydoc-markdown --server --open
+
+## How to run example scripts
+
+If you cloned the repository or downloaded the source code to try the [example scripts](examples),
+you will need to make sure you have MartyPy installed before you can run the examples.
+
+The easiest way to install MartyPy is with the `pip install martypy` script as explained in
+[step 2 here](https://userguides.robotical.io/martyv2/userguides/python/setting_up_python_on_your_computer).
+
+Once martypy is installed you can run each example using python.
+The following (for the dance example) assumes you have connected your marty using the USB cable to a Windows computer
+
+python example_dance.py USB
+
+To run the sound example over WiFi when your Marty is connected on IP address 192.168.86.10, use:
+
+python example_sound.py WiFi 192.168.0.10
+
+If you would like to make modifications to the martypy library itself, it will be better to install
+it from source using the command `pip install --editable /path/to/martypy/repo` (replacing
+`/path/to/martypy/repo` as appropriate of course).
+
+If you do not want to "`pip install`" the MartyPy library, you can add the following 4 lines at the
+top (before any other code) of each script you want to run:
+
+```python
+import sys
+import pathlib
+cur_path = pathlib.Path(__file__).parent.resolve()
+sys.path.append(str(cur_path.parent.resolve()))
+```
```

### Comparing `martypy-3.4.3/martypy.egg-info/SOURCES.txt` & `martypy-3.5.0/martypy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 CHANGES.md
 LICENSE.md
 MANIFEST.in
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 martypy/ClientGeneric.py
 martypy/ClientMV1.py
 martypy/ClientMV2.py
 martypy/Exceptions.py
 martypy/LikeHDLC.py
@@ -17,22 +16,24 @@
 martypy/RICCommsSerial.py
 martypy/RICCommsTest.py
 martypy/RICCommsWiFi.py
 martypy/RICHWElems.py
 martypy/RICInterface.py
 martypy/RICProtocols.py
 martypy/RICROSSerial.py
+martypy/RICStreamHandler.py
 martypy/RateAverager.py
 martypy/ValueAverager.py
 martypy/WebSocket.py
 martypy/WebSocketFrame.py
 martypy/__init__.py
 martypy.egg-info/PKG-INFO
 martypy.egg-info/SOURCES.txt
 martypy.egg-info/dependency_links.txt
 martypy.egg-info/requires.txt
 martypy.egg-info/top_level.txt
 martypy/tests/__init__.py
 martypy/tests/testBaudRateSelection.py
 martypy/tests/testColourSensor.py
+martypy/tests/testStreamMP3.py
 martypy/tests/test_martypy.py
 martypy/tests/testrob.py
```

### Comparing `martypy-3.4.3/setup.py` & `martypy-3.5.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,59 @@
-from setuptools import setup, find_packages
-
-with open('README.md') as f:
-    readme = f.read()
-
-setup(
-    name="martypy",
-    version="3.4.3",
-    description="Python library for Marty the Robot V1 and V2",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    author="Robotical",
-    author_email="hello@robotical.io",
-    copyright="Robotical",
-    maintainer='Robotical',
-    maintainer_email='hello@robotical.io',
-    packages=find_packages(),
-    url='http://github.com/robotical/martypy',
-    license='Apache 2.0',
-    install_requires=[
-        'pyserial>=3.4',
-        'packaging>=21.3'
-    ],
-    extras_require={
-        "tests": [
-            "pytest",
-        ],
-    },
-    keywords=[
-        'ros',
-        'robot',
-        'marty',
-        'marty the robot',
-        'robotical',
-    ],
-    classifiers= [
-        # As from https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        # 'Development Status :: 1 - Planning',
-        # 'Development Status :: 2 - Pre-Alpha',
-        # 'Development Status :: 3 - Alpha',
-        #'Development Status :: 4 - Beta',
-        'Development Status :: 5 - Production/Stable',
-        # 'Development Status :: 6 - Mature',
-        # 'Development Status :: 7 - Inactive',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        "Operating System :: OS Independent",
-        'License :: OSI Approved :: Apache Software License',
-    ]
-)
-
-# To Publish:
-# First, build a source distribution:
-# $ python setup.py sdist
-# Then upload this to PyPi (have ~/.pypirc exist)
-# $ twine upload dist/*
-
+from setuptools import setup, find_packages
+
+with open('README.md') as f:
+    readme = f.read()
+
+setup(
+    name="martypy",
+    version="3.5.0",
+    description="Python library for Marty the Robot V1 and V2",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    author="Robotical",
+    author_email="hello@robotical.io",
+    copyright="Robotical",
+    maintainer='Robotical',
+    maintainer_email='hello@robotical.io',
+    packages=find_packages(),
+    url='http://github.com/robotical/martypy',
+    license='Apache 2.0',
+    install_requires=[
+        'pyserial',
+    ],
+    extras_require={
+        "tests": [
+            "pytest",
+        ],
+    },
+    keywords=[
+        'ros',
+        'robot',
+        'marty',
+        'marty the robot',
+        'robotical',
+    ],
+    classifiers= [
+        # As from https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        # 'Development Status :: 1 - Planning',
+        # 'Development Status :: 2 - Pre-Alpha',
+        # 'Development Status :: 3 - Alpha',
+        #'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
+        # 'Development Status :: 6 - Mature',
+        # 'Development Status :: 7 - Inactive',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        "Operating System :: OS Independent",
+        'License :: OSI Approved :: Apache Software License',
+    ]
+)
+
+# To Publish:
+# First, build a source distribution:
+# $ python setup.py sdist
+# Then upload this to PyPi (have ~/.pypirc exist)
+# $ twine upload dist/*
+
```

