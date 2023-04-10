# Comparing `tmp/get_patchlib-0.0.0.tar.gz` & `tmp/get_patchlib-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_patchlib-0.0.0.tar", last modified: Mon Apr 10 20:20:03 2023, max compression
+gzip compressed data, was "get_patchlib-1.1.tar", last modified: Mon Apr 10 22:03:13 2023, max compression
```

## Comparing `get_patchlib-0.0.0.tar` & `get_patchlib-1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 20:20:03.277169 get_patchlib-0.0.0/
--rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 get_patchlib-0.0.0/LICENSE
--rw-rw-rw-   0        0        0       82 2023-04-10 20:20:03.277169 get_patchlib-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2023-04-10 16:52:06.000000 get_patchlib-0.0.0/README.md
--rw-rw-rw-   0        0        0      271 2023-04-10 18:45:39.000000 get_patchlib-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      537 2023-04-10 20:20:03.294159 get_patchlib-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-10 20:20:03.076284 get_patchlib-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-10 20:20:03.172232 get_patchlib-0.0.0/src/get_patchlib/
--rw-rw-rw-   0        0        0      190 2023-04-10 16:52:20.000000 get_patchlib-0.0.0/src/get_patchlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:20:03.267177 get_patchlib-0.0.0/src/get_patchlib/bps/
--rw-rw-rw-   0        0        0     6180 2023-04-09 23:10:26.000000 get_patchlib-0.0.0/src/get_patchlib/bps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:20:03.274172 get_patchlib-0.0.0/src/get_patchlib/ips/
--rw-rw-rw-   0        0        0    16519 2023-04-09 23:10:20.000000 get_patchlib-0.0.0/src/get_patchlib/ips/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 20:20:03.260179 get_patchlib-0.0.0/src/get_patchlib.egg-info/
--rw-rw-rw-   0        0        0       82 2023-04-10 20:20:02.000000 get_patchlib-0.0.0/src/get_patchlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-04-10 20:20:03.000000 get_patchlib-0.0.0/src/get_patchlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 20:20:02.000000 get_patchlib-0.0.0/src/get_patchlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 20:20:02.000000 get_patchlib-0.0.0/src/get_patchlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 22:03:13.480810 get_patchlib-1.1/
+-rw-rw-rw-   0        0        0        0 2021-07-31 02:25:56.000000 get_patchlib-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2143 2023-04-10 22:03:13.480810 get_patchlib-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1735 2023-04-10 16:52:06.000000 get_patchlib-1.1/README.md
+-rw-rw-rw-   0        0        0      271 2023-04-10 21:37:21.000000 get_patchlib-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      464 2023-04-10 22:03:13.493804 get_patchlib-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-10 22:03:13.413849 get_patchlib-1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-10 22:03:13.471816 get_patchlib-1.1/src/get_patchlib.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-04-10 22:03:13.000000 get_patchlib-1.1/src/get_patchlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-10 22:03:13.000000 get_patchlib-1.1/src/get_patchlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 22:03:13.000000 get_patchlib-1.1/src/get_patchlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-10 22:03:13.000000 get_patchlib-1.1/src/get_patchlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 22:03:13.474814 get_patchlib-1.1/src/patchlib/
+-rw-rw-rw-   0        0        0       86 2023-04-10 22:02:09.000000 get_patchlib-1.1/src/patchlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:03:13.476812 get_patchlib-1.1/src/patchlib/bps/
+-rw-rw-rw-   0        0        0     6180 2023-04-09 23:10:26.000000 get_patchlib-1.1/src/patchlib/bps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 22:03:13.478814 get_patchlib-1.1/src/patchlib/ips/
+-rw-rw-rw-   0        0        0    16519 2023-04-09 23:10:20.000000 get_patchlib-1.1/src/patchlib/ips/__init__.py
```

### Comparing `get_patchlib-0.0.0/README.md` & `get_patchlib-1.1/README.md`

 * *Files identical despite different names*

### Comparing `get_patchlib-0.0.0/src/get_patchlib/bps/__init__.py` & `get_patchlib-1.1/src/patchlib/bps/__init__.py`

 * *Files identical despite different names*

### Comparing `get_patchlib-0.0.0/src/get_patchlib/ips/__init__.py` & `get_patchlib-1.1/src/patchlib/ips/__init__.py`

 * *Files identical despite different names*

