# Comparing `tmp/shard_client-0.0.4.tar.gz` & `tmp/shard_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shard_client-0.0.4.tar", last modified: Tue Apr 11 01:21:42 2023, max compression
+gzip compressed data, was "shard_client-0.0.5.tar", last modified: Tue Apr 11 01:27:33 2023, max compression
```

## Comparing `shard_client-0.0.4.tar` & `shard_client-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 01:21:42.520941 shard_client-0.0.4/
--rw-r--r--   0 anon      (1000) anon      (1000)      375 2023-04-11 01:21:42.520941 shard_client-0.0.4/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)      450 2023-04-11 01:21:20.000000 shard_client-0.0.4/pyproject.toml
--rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-11 01:21:42.520941 shard_client-0.0.4/setup.cfg
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 01:21:42.516941 shard_client-0.0.4/src/
--rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-04-10 21:12:34.000000 shard_client-0.0.4/src/__init__.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 01:21:42.520941 shard_client-0.0.4/src/lib/
--rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-04-04 22:34:06.000000 shard_client-0.0.4/src/lib/color_printer.py
--rw-r--r--   0 anon      (1000) anon      (1000)      766 2023-04-01 20:15:34.000000 shard_client-0.0.4/src/lib/logclass.py
--rw-r--r--   0 anon      (1000) anon      (1000)     3432 2023-04-05 01:55:08.000000 shard_client-0.0.4/src/lib/mqlib.py
--rw-r--r--   0 anon      (1000) anon      (1000)      304 2023-03-31 23:23:46.000000 shard_client-0.0.4/src/lib/mqtt_queue.py
--rw-r--r--   0 anon      (1000) anon      (1000)       59 2023-04-01 19:54:16.000000 shard_client-0.0.4/src/lib/status.py
--rwxr-xr-x   0 anon      (1000) anon      (1000)     7311 2023-04-11 00:49:22.000000 shard_client-0.0.4/src/scanner.py
-drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 01:21:42.520941 shard_client-0.0.4/src/shard_client.egg-info/
--rw-r--r--   0 anon      (1000) anon      (1000)      375 2023-04-11 01:21:42.000000 shard_client-0.0.4/src/shard_client.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) anon      (1000)      346 2023-04-11 01:21:42.000000 shard_client-0.0.4/src/shard_client.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-11 01:21:42.000000 shard_client-0.0.4/src/shard_client.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       37 2023-04-11 01:21:42.000000 shard_client-0.0.4/src/shard_client.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) anon      (1000)       26 2023-04-11 01:21:42.000000 shard_client-0.0.4/src/shard_client.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 01:27:33.660953 shard_client-0.0.5/
+-rw-r--r--   0 anon      (1000) anon      (1000)      375 2023-04-11 01:27:33.660953 shard_client-0.0.5/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)      450 2023-04-11 01:27:14.000000 shard_client-0.0.5/pyproject.toml
+-rw-r--r--   0 anon      (1000) anon      (1000)       38 2023-04-11 01:27:33.660953 shard_client-0.0.5/setup.cfg
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 01:27:33.656953 shard_client-0.0.5/shard_client/
+-rw-r--r--   0 anon      (1000) anon      (1000)        0 2023-04-10 21:12:34.000000 shard_client-0.0.5/shard_client/__init__.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 01:27:33.660953 shard_client-0.0.5/shard_client/lib/
+-rw-r--r--   0 anon      (1000) anon      (1000)     1590 2023-04-04 22:34:06.000000 shard_client-0.0.5/shard_client/lib/color_printer.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      766 2023-04-01 20:15:34.000000 shard_client-0.0.5/shard_client/lib/logclass.py
+-rw-r--r--   0 anon      (1000) anon      (1000)     3432 2023-04-05 01:55:08.000000 shard_client-0.0.5/shard_client/lib/mqlib.py
+-rw-r--r--   0 anon      (1000) anon      (1000)      304 2023-03-31 23:23:46.000000 shard_client-0.0.5/shard_client/lib/mqtt_queue.py
+-rw-r--r--   0 anon      (1000) anon      (1000)       59 2023-04-01 19:54:16.000000 shard_client-0.0.5/shard_client/lib/status.py
+-rwxr-xr-x   0 anon      (1000) anon      (1000)     7311 2023-04-11 00:49:22.000000 shard_client-0.0.5/shard_client/scanner.py
+drwxr-xr-x   0 anon      (1000) anon      (1000)        0 2023-04-11 01:27:33.660953 shard_client-0.0.5/shard_client.egg-info/
+-rw-r--r--   0 anon      (1000) anon      (1000)      375 2023-04-11 01:27:33.000000 shard_client-0.0.5/shard_client.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) anon      (1000)      389 2023-04-11 01:27:33.000000 shard_client-0.0.5/shard_client.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)        1 2023-04-11 01:27:33.000000 shard_client-0.0.5/shard_client.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       37 2023-04-11 01:27:33.000000 shard_client-0.0.5/shard_client.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) anon      (1000)       13 2023-04-11 01:27:33.000000 shard_client-0.0.5/shard_client.egg-info/top_level.txt
```

### Comparing `shard_client-0.0.4/src/lib/color_printer.py` & `shard_client-0.0.5/shard_client/lib/color_printer.py`

 * *Files identical despite different names*

### Comparing `shard_client-0.0.4/src/lib/logclass.py` & `shard_client-0.0.5/shard_client/lib/logclass.py`

 * *Files identical despite different names*

### Comparing `shard_client-0.0.4/src/lib/mqlib.py` & `shard_client-0.0.5/shard_client/lib/mqlib.py`

 * *Files identical despite different names*

### Comparing `shard_client-0.0.4/src/scanner.py` & `shard_client-0.0.5/shard_client/scanner.py`

 * *Files identical despite different names*

