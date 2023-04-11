# Comparing `tmp/bpctl-1.1.tar.gz` & `tmp/bpctl-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpctl-1.1.tar", last modified: Tue Apr 11 13:18:13 2023, max compression
+gzip compressed data, was "bpctl-1.2.tar", last modified: Tue Apr 11 14:01:59 2023, max compression
```

## Comparing `bpctl-1.1.tar` & `bpctl-1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 opstree   (1000) opstree   (1000)        0 2023-04-11 13:18:13.615686 bpctl-1.1/
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      179 2023-04-11 10:56:21.000000 bpctl-1.1/MANIFEST.in
--rw-rw-r--   0 opstree   (1000) opstree   (1000)        0 2023-04-11 10:56:21.000000 bpctl-1.1/Makefile
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      272 2023-04-11 13:18:13.615686 bpctl-1.1/PKG-INFO
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      231 2023-04-11 10:56:21.000000 bpctl-1.1/README.md
-drwxrwxr-x   0 opstree   (1000) opstree   (1000)        0 2023-04-11 13:18:13.615686 bpctl-1.1/bpctl.egg-info/
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      272 2023-04-11 13:18:13.000000 bpctl-1.1/bpctl.egg-info/PKG-INFO
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      424 2023-04-11 13:18:13.000000 bpctl-1.1/bpctl.egg-info/SOURCES.txt
--rw-rw-r--   0 opstree   (1000) opstree   (1000)        1 2023-04-11 13:18:13.000000 bpctl-1.1/bpctl.egg-info/dependency_links.txt
--rw-rw-r--   0 opstree   (1000) opstree   (1000)       35 2023-04-11 13:18:13.000000 bpctl-1.1/bpctl.egg-info/requires.txt
--rw-rw-r--   0 opstree   (1000) opstree   (1000)        4 2023-04-11 13:18:13.000000 bpctl-1.1/bpctl.egg-info/top_level.txt
-drwxrwxr-x   0 opstree   (1000) opstree   (1000)        0 2023-04-11 13:18:13.615686 bpctl-1.1/lib/
--rw-rw-r--   0 opstree   (1000) opstree   (1000)        0 2023-04-11 10:56:21.000000 bpctl-1.1/lib/__init__.py
-drwxrwxr-x   0 opstree   (1000) opstree   (1000)        0 2023-04-11 13:18:13.615686 bpctl-1.1/lib/bpctl/
--rw-rw-r--   0 opstree   (1000) opstree   (1000)        0 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/__init__.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      901 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/authenticate.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)     2777 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/base.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)     5879 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/bp_manifest.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)     1695 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/bpctl.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      457 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/config.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)     3341 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/load_data.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)       51 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/read_bp_yaml.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)        0 2023-04-11 10:56:21.000000 bpctl-1.1/lib/bpctl/utils.py
--rw-rw-r--   0 opstree   (1000) opstree   (1000)       21 2023-04-11 10:56:21.000000 bpctl-1.1/requirements.txt
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      163 2023-04-11 13:18:13.615686 bpctl-1.1/setup.cfg
--rw-rw-r--   0 opstree   (1000) opstree   (1000)      409 2023-04-11 13:13:49.000000 bpctl-1.1/setup.py
+drwxrwxr-x   0 opstree   (1000) opstree   (1000)        0 2023-04-11 14:01:59.680633 bpctl-1.2/
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      179 2023-04-11 10:56:21.000000 bpctl-1.2/MANIFEST.in
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)        0 2023-04-11 10:56:21.000000 bpctl-1.2/Makefile
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      285 2023-04-11 14:01:59.680633 bpctl-1.2/PKG-INFO
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      231 2023-04-11 10:56:21.000000 bpctl-1.2/README.md
+drwxrwxr-x   0 opstree   (1000) opstree   (1000)        0 2023-04-11 14:01:59.676633 bpctl-1.2/bpctl.egg-info/
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      285 2023-04-11 14:01:59.000000 bpctl-1.2/bpctl.egg-info/PKG-INFO
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      424 2023-04-11 14:01:59.000000 bpctl-1.2/bpctl.egg-info/SOURCES.txt
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)        1 2023-04-11 14:01:59.000000 bpctl-1.2/bpctl.egg-info/dependency_links.txt
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)       35 2023-04-11 14:01:59.000000 bpctl-1.2/bpctl.egg-info/requires.txt
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)        4 2023-04-11 14:01:59.000000 bpctl-1.2/bpctl.egg-info/top_level.txt
+drwxrwxr-x   0 opstree   (1000) opstree   (1000)        0 2023-04-11 14:01:59.676633 bpctl-1.2/lib/
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)        0 2023-04-11 10:56:21.000000 bpctl-1.2/lib/__init__.py
+drwxrwxr-x   0 opstree   (1000) opstree   (1000)        0 2023-04-11 14:01:59.680633 bpctl-1.2/lib/bpctl/
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)        0 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/__init__.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      901 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/authenticate.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)     2777 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/base.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)     5879 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/bp_manifest.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)     1695 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/bpctl.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      457 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/config.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)     3341 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/load_data.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)       51 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/read_bp_yaml.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)        0 2023-04-11 10:56:21.000000 bpctl-1.2/lib/bpctl/utils.py
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)       21 2023-04-11 10:56:21.000000 bpctl-1.2/requirements.txt
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      163 2023-04-11 14:01:59.680633 bpctl-1.2/setup.cfg
+-rw-rw-r--   0 opstree   (1000) opstree   (1000)      422 2023-04-11 14:00:24.000000 bpctl-1.2/setup.py
```

### Comparing `bpctl-1.1/lib/bpctl/authenticate.py` & `bpctl-1.2/lib/bpctl/authenticate.py`

 * *Files identical despite different names*

### Comparing `bpctl-1.1/lib/bpctl/base.py` & `bpctl-1.2/lib/bpctl/base.py`

 * *Files identical despite different names*

### Comparing `bpctl-1.1/lib/bpctl/bp_manifest.py` & `bpctl-1.2/lib/bpctl/bp_manifest.py`

 * *Files identical despite different names*

### Comparing `bpctl-1.1/lib/bpctl/bpctl.py` & `bpctl-1.2/lib/bpctl/bpctl.py`

 * *Files identical despite different names*

### Comparing `bpctl-1.1/lib/bpctl/load_data.py` & `bpctl-1.2/lib/bpctl/load_data.py`

 * *Files identical despite different names*

