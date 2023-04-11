# Comparing `tmp/pvcobra-1.2.0.tar.gz` & `tmp/pvcobra-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvcobra-1.2.0.tar", last modified: Wed Jan 25 21:18:13 2023, max compression
+gzip compressed data, was "pvcobra-1.2.1.tar", last modified: Tue Apr 11 00:43:01 2023, max compression
```

## Comparing `pvcobra-1.2.0.tar` & `pvcobra-1.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/
--rw-rw-r--   0 eric      (1000) eric      (1000)      425 2023-01-25 21:18:13.000000 pvcobra-1.2.0/MANIFEST.in
--rw-rw-r--   0 eric      (1000) eric      (1000)     2265 2023-01-25 21:18:13.109261 pvcobra-1.2.0/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1602 2022-06-07 19:58:39.000000 pvcobra-1.2.0/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/
--rw-rw-r--   0 eric      (1000) eric      (1000)    11344 2023-01-25 21:18:13.000000 pvcobra-1.2.0/pvcobra/LICENSE
--rw-rw-r--   0 eric      (1000) eric      (1000)     1118 2023-01-25 21:18:13.000000 pvcobra-1.2.0/pvcobra/__init__.py
--rw-rw-r--   0 eric      (1000) eric      (1000)     5865 2023-01-25 21:18:13.000000 pvcobra-1.2.0/pvcobra/cobra.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/beaglebone/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   198464 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/beaglebone/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.105261 pvcobra-1.2.0/pvcobra/lib/jetson/
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/jetson/cortex-a57-aarch64/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   211472 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/jetson/cortex-a57-aarch64/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/linux/
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/linux/x86_64/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   224096 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/linux/x86_64/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/mac/
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/mac/arm64/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   286302 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/mac/arm64/libpv_cobra.dylib
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/mac/x86_64/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   283968 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/mac/x86_64/libpv_cobra.dylib
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/arm11/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   194352 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/arm11/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a53/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   198468 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a53/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a53-aarch64/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   211560 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a53-aarch64/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a7/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   198468 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a7/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a72/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   202564 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a72/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a72-aarch64/
--rwxrwxr-x   0 eric      (1000) eric      (1000)   211560 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a72-aarch64/libpv_cobra.so
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/windows/
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra/lib/windows/amd64/
--rw-rw-r--   0 eric      (1000) eric      (1000)   321536 2023-01-25 21:15:39.000000 pvcobra-1.2.0/pvcobra/lib/windows/amd64/libpv_cobra.dll
--rw-rw-r--   0 eric      (1000) eric      (1000)     3347 2023-01-25 21:18:13.000000 pvcobra-1.2.0/pvcobra/util.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-01-25 21:18:13.109261 pvcobra-1.2.0/pvcobra.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)     2265 2023-01-25 21:18:13.000000 pvcobra-1.2.0/pvcobra.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)      793 2023-01-25 21:18:13.000000 pvcobra-1.2.0/pvcobra.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-01-25 21:18:13.000000 pvcobra-1.2.0/pvcobra.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        8 2023-01-25 21:18:13.000000 pvcobra-1.2.0/pvcobra.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-01-25 21:18:13.109261 pvcobra-1.2.0/setup.cfg
--rw-rw-r--   0 eric      (1000) eric      (1000)     2859 2023-01-25 21:17:17.000000 pvcobra-1.2.0/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.371711 pvcobra-1.2.1/
+-rw-rw-r--   0 eric      (1000) eric      (1000)      425 2023-04-11 00:43:01.000000 pvcobra-1.2.1/MANIFEST.in
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2265 2023-04-11 00:43:01.371711 pvcobra-1.2.1/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1602 2022-06-07 19:58:39.000000 pvcobra-1.2.1/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/
+-rw-rw-r--   0 eric      (1000) eric      (1000)    11344 2023-04-11 00:43:01.000000 pvcobra-1.2.1/pvcobra/LICENSE
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1118 2023-04-11 00:43:01.000000 pvcobra-1.2.1/pvcobra/__init__.py
+-rw-rw-r--   0 eric      (1000) eric      (1000)     5865 2023-04-11 00:43:01.000000 pvcobra-1.2.1/pvcobra/cobra.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/beaglebone/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   198464 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/beaglebone/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/jetson/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/jetson/cortex-a57-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   211472 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/jetson/cortex-a57-aarch64/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/linux/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/linux/x86_64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   224096 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/linux/x86_64/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/mac/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/mac/arm64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   286302 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/mac/arm64/libpv_cobra.dylib
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/mac/x86_64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   283968 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/mac/x86_64/libpv_cobra.dylib
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/arm11/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   194352 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/arm11/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a53/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   198468 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a53/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a53-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   211560 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a53-aarch64/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a7/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   198468 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a7/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a72/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   202564 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a72/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a72-aarch64/
+-rwxrwxr-x   0 eric      (1000) eric      (1000)   211560 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a72-aarch64/libpv_cobra.so
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/windows/
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra/lib/windows/amd64/
+-rw-rw-r--   0 eric      (1000) eric      (1000)   321536 2023-02-08 19:29:31.000000 pvcobra-1.2.1/pvcobra/lib/windows/amd64/libpv_cobra.dll
+-rw-rw-r--   0 eric      (1000) eric      (1000)     3527 2023-04-11 00:43:01.000000 pvcobra-1.2.1/pvcobra/util.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-04-11 00:43:01.367711 pvcobra-1.2.1/pvcobra.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2265 2023-04-11 00:43:01.000000 pvcobra-1.2.1/pvcobra.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      793 2023-04-11 00:43:01.000000 pvcobra-1.2.1/pvcobra.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-04-11 00:43:01.000000 pvcobra-1.2.1/pvcobra.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        8 2023-04-11 00:43:01.000000 pvcobra-1.2.1/pvcobra.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-04-11 00:43:01.371711 pvcobra-1.2.1/setup.cfg
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2859 2023-04-10 21:22:19.000000 pvcobra-1.2.1/setup.py
```

### Comparing `pvcobra-1.2.0/PKG-INFO` & `pvcobra-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvcobra
-Version: 1.2.0
+Version: 1.2.1
 Summary: Cobra voice activity detection (VAD) engine
 Home-page: https://github.com/Picovoice/cobra
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: voice activity detection engine,VAD
 Platform: UNKNOWN
```

### Comparing `pvcobra-1.2.0/README.md` & `pvcobra-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/LICENSE` & `pvcobra-1.2.1/pvcobra/LICENSE`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/__init__.py` & `pvcobra-1.2.1/pvcobra/__init__.py`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/cobra.py` & `pvcobra-1.2.1/pvcobra/cobra.py`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/beaglebone/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/beaglebone/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/jetson/cortex-a57-aarch64/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/jetson/cortex-a57-aarch64/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/linux/x86_64/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/linux/x86_64/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/mac/arm64/libpv_cobra.dylib` & `pvcobra-1.2.1/pvcobra/lib/mac/arm64/libpv_cobra.dylib`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/mac/x86_64/libpv_cobra.dylib` & `pvcobra-1.2.1/pvcobra/lib/mac/x86_64/libpv_cobra.dylib`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/raspberry-pi/arm11/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/raspberry-pi/arm11/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a53/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a53/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a53-aarch64/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a53-aarch64/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a7/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a7/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a72/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a72/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/raspberry-pi/cortex-a72-aarch64/libpv_cobra.so` & `pvcobra-1.2.1/pvcobra/lib/raspberry-pi/cortex-a72-aarch64/libpv_cobra.so`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/lib/windows/amd64/libpv_cobra.dll` & `pvcobra-1.2.1/pvcobra/lib/windows/amd64/libpv_cobra.dll`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/pvcobra/util.py` & `pvcobra-1.2.1/pvcobra/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 #
-# Copyright 2021 Picovoice Inc.
+# Copyright 2021-2023 Picovoice Inc.
 #
 # You may not use this file except in compliance with the license. A copy of the license is located in the "LICENSE"
 # file accompanying this source.
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 #
 
 import os
 import platform
 import subprocess
 
 
+def _is_64bit():
+    return '64bit' in platform.architecture()[0]
+
+
 def _pv_linux_machine(machine):
     if machine == 'x86_64':
         return machine
-
-    if machine == 'aarch64':
-        arch_info = '-' + machine
+    elif machine in ['aarch64', 'armv7l', 'armv6l']:
+        arch_info = ('-' + machine) if _is_64bit() else ''
     else:
-        arch_info = ''
+        raise NotImplementedError("Unsupported CPU architecture: `%s`" % machine)
 
     cpu_info = subprocess.check_output(['cat', '/proc/cpuinfo']).decode()
     cpu_part_list = [x for x in cpu_info.split('\n') if 'CPU part' in x]
     if len(cpu_part_list) == 0:
         raise RuntimeError('Unsupported CPU.\n%s' % cpu_info)
 
     cpu_part = cpu_part_list[0].split(' ')[-1].lower()
```

### Comparing `pvcobra-1.2.0/pvcobra.egg-info/PKG-INFO` & `pvcobra-1.2.1/pvcobra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvcobra
-Version: 1.2.0
+Version: 1.2.1
 Summary: Cobra voice activity detection (VAD) engine
 Home-page: https://github.com/Picovoice/cobra
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: voice activity detection engine,VAD
 Platform: UNKNOWN
```

### Comparing `pvcobra-1.2.0/pvcobra.egg-info/SOURCES.txt` & `pvcobra-1.2.1/pvcobra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pvcobra-1.2.0/setup.py` & `pvcobra-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     f.write(MANIFEST_IN.strip('\n '))
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvcobra",
-    version="1.2.0",
+    version="1.2.1",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Cobra voice activity detection (VAD) engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/cobra",
     packages=["pvcobra"],
```

