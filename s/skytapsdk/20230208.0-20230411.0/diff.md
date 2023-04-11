# Comparing `tmp/skytapsdk-20230208.0.tar.gz` & `tmp/skytapsdk-20230411.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytapsdk-20230208.0.tar", last modified: Wed Feb  8 11:57:39 2023, max compression
+gzip compressed data, was "skytapsdk-20230411.0.tar", last modified: Tue Apr 11 14:14:39 2023, max compression
```

## Comparing `skytapsdk-20230208.0.tar` & `skytapsdk-20230411.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-02-08 11:57:39.204956 skytapsdk-20230208.0/
--rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:30.000000 skytapsdk-20230208.0/LICENSE.md
--rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-02-08 11:57:39.205031 skytapsdk-20230208.0/PKG-INFO
--rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-02-08 11:57:39.205253 skytapsdk-20230208.0/setup.cfg
--rw-r--r--   0 dmickelson   (503) staff       (20)     1389 2023-02-08 11:56:01.000000 skytapsdk-20230208.0/setup.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-02-08 11:57:39.202948 skytapsdk-20230208.0/skytapsdk/
--rw-r--r--   0 dmickelson   (503) staff       (20)      102 2023-02-07 14:36:46.000000 skytapsdk-20230208.0/skytapsdk/__init__.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-02-08 11:57:39.204304 skytapsdk-20230208.0/skytapsdk/api_endpoints/
--rw-r--r--   0 dmickelson   (503) staff       (20)        0 2023-02-07 14:36:46.000000 skytapsdk-20230208.0/skytapsdk/api_endpoints/__init__.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1068 2023-02-07 14:36:46.000000 skytapsdk-20230208.0/skytapsdk/api_endpoints/assets.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1141 2023-02-07 14:36:46.000000 skytapsdk-20230208.0/skytapsdk/api_endpoints/environments.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1609 2023-02-08 11:56:12.000000 skytapsdk-20230208.0/skytapsdk/api_endpoints/projects.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1138 2023-02-07 15:20:17.000000 skytapsdk-20230208.0/skytapsdk/api_endpoints/reports.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1102 2023-02-07 14:36:46.000000 skytapsdk-20230208.0/skytapsdk/api_endpoints/templates.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1060 2023-02-07 14:36:46.000000 skytapsdk-20230208.0/skytapsdk/api_endpoints/users.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1481 2023-02-07 15:11:48.000000 skytapsdk-20230208.0/skytapsdk/helpers.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     3286 2023-02-08 11:56:12.000000 skytapsdk-20230208.0/skytapsdk/skytap.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-02-08 11:57:39.203517 skytapsdk-20230208.0/skytapsdk.egg-info/
--rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-02-08 11:57:39.000000 skytapsdk-20230208.0/skytapsdk.egg-info/PKG-INFO
--rw-r--r--   0 dmickelson   (503) staff       (20)      507 2023-02-08 11:57:39.000000 skytapsdk-20230208.0/skytapsdk.egg-info/SOURCES.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-02-08 11:57:39.000000 skytapsdk-20230208.0/skytapsdk.egg-info/dependency_links.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        8 2023-02-08 11:57:39.000000 skytapsdk-20230208.0/skytapsdk.egg-info/requires.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)       10 2023-02-08 11:57:39.000000 skytapsdk-20230208.0/skytapsdk.egg-info/top_level.txt
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-11 14:14:39.908495 skytapsdk-20230411.0/
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:30.000000 skytapsdk-20230411.0/LICENSE.md
+-rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-11 14:14:39.908558 skytapsdk-20230411.0/PKG-INFO
+-rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-04-11 14:14:39.908757 skytapsdk-20230411.0/setup.cfg
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1389 2023-04-11 14:11:52.000000 skytapsdk-20230411.0/setup.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-11 14:14:39.907018 skytapsdk-20230411.0/skytapsdk/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      102 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/__init__.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-11 14:14:39.908382 skytapsdk-20230411.0/skytapsdk/api_endpoints/
+-rw-r--r--   0 dmickelson   (503) staff       (20)        0 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1068 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/assets.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1141 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/environments.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1609 2023-04-10 15:37:33.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/projects.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1138 2023-04-10 15:37:33.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/reports.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1102 2023-02-07 14:36:46.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/templates.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1316 2023-04-11 14:12:27.000000 skytapsdk-20230411.0/skytapsdk/api_endpoints/users.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1481 2023-02-07 15:11:48.000000 skytapsdk-20230411.0/skytapsdk/helpers.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     3286 2023-04-10 15:37:33.000000 skytapsdk-20230411.0/skytapsdk/skytap.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-04-11 14:14:39.907609 skytapsdk-20230411.0/skytapsdk.egg-info/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      831 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/PKG-INFO
+-rw-r--r--   0 dmickelson   (503) staff       (20)      507 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        8 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/requires.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)       10 2023-04-11 14:14:39.000000 skytapsdk-20230411.0/skytapsdk.egg-info/top_level.txt
```

### Comparing `skytapsdk-20230208.0/LICENSE.md` & `skytapsdk-20230411.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230208.0/PKG-INFO` & `skytapsdk-20230411.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytapsdk
-Version: 20230208.0
+Version: 20230411.0
 Summary: SDK for interacting with Skytap's APIs.
 Home-page: 
 Author: Dax Mickelson
 Author-email: dmickelson@zscaler.com
 License: BSD
 Keywords: skytap
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `skytapsdk-20230208.0/setup.py` & `skytapsdk-20230411.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version = "20230208.0"
+__version = "20230411.0"
 __author = "Dax Mickelson"
 __author_email = "dmickelson@zscaler.com"
 __license = "BSD"
 __name = "skytapsdk"
 __description = "SDK for interacting with Skytap's APIs."
 __long_description = __description
 __url = ""
```

### Comparing `skytapsdk-20230208.0/skytapsdk/api_endpoints/assets.py` & `skytapsdk-20230411.0/skytapsdk/api_endpoints/assets.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230208.0/skytapsdk/api_endpoints/environments.py` & `skytapsdk-20230411.0/skytapsdk/api_endpoints/environments.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230208.0/skytapsdk/api_endpoints/projects.py` & `skytapsdk-20230411.0/skytapsdk/api_endpoints/projects.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230208.0/skytapsdk/api_endpoints/reports.py` & `skytapsdk-20230411.0/skytapsdk/api_endpoints/reports.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230208.0/skytapsdk/api_endpoints/templates.py` & `skytapsdk-20230411.0/skytapsdk/api_endpoints/templates.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230208.0/skytapsdk/api_endpoints/users.py` & `skytapsdk-20230411.0/skytapsdk/api_endpoints/users.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,7 +34,19 @@
             uid: ID of desired user.
 
         Returns:
             dict of queried user account.
         """
         self._path = f"{self._path}/{uid}"
         return self._get().json()
+
+    def add_user(
+        self,
+        **kwargs,
+    ):
+        """Add a user"""
+        # Add parameters to payload
+        payload = {}
+        for key, value in kwargs.items():
+            payload[key] = value
+
+        return self._post(json=payload)
```

### Comparing `skytapsdk-20230208.0/skytapsdk/helpers.py` & `skytapsdk-20230411.0/skytapsdk/helpers.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230208.0/skytapsdk/skytap.py` & `skytapsdk-20230411.0/skytapsdk/skytap.py`

 * *Files identical despite different names*

### Comparing `skytapsdk-20230208.0/skytapsdk.egg-info/PKG-INFO` & `skytapsdk-20230411.0/skytapsdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skytapsdk
-Version: 20230208.0
+Version: 20230411.0
 Summary: SDK for interacting with Skytap's APIs.
 Home-page: 
 Author: Dax Mickelson
 Author-email: dmickelson@zscaler.com
 License: BSD
 Keywords: skytap
 Classifier: Development Status :: 5 - Production/Stable
```

