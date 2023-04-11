# Comparing `tmp/nextpcg-0.3.1.tar.gz` & `tmp/nextpcg-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.3.1.tar", last modified: Tue Apr 11 07:37:48 2023, max compression
+gzip compressed data, was "nextpcg-0.4.0.tar", last modified: Tue Apr 11 07:54:21 2023, max compression
```

## Comparing `nextpcg-0.3.1.tar` & `nextpcg-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:37:48.296194 nextpcg-0.3.1/
--rw-rw-rw-   0        0        0       72 2023-03-17 08:38:04.000000 nextpcg-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1321 2023-04-11 07:37:48.295198 nextpcg-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 07:37:48.233666 nextpcg-0.3.1/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1321 2023-04-11 07:37:48.000000 nextpcg-0.3.1/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-04-11 07:37:48.000000 nextpcg-0.3.1/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:37:48.000000 nextpcg-0.3.1/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-11 07:37:48.000000 nextpcg-0.3.1/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-04-11 07:37:48.000000 nextpcg-0.3.1/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 07:37:48.000000 nextpcg-0.3.1/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-02 08:29:40.000000 nextpcg-0.3.1/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-11 07:37:48.286221 nextpcg-0.3.1/pypapi/
--rw-rw-rw-   0        0        0      749 2023-03-17 08:38:04.000000 nextpcg-0.3.1/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-03-17 08:38:04.000000 nextpcg-0.3.1/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-04-11 03:30:49.000000 nextpcg-0.3.1/pypapi/const.py
--rw-rw-rw-   0        0        0     5482 2023-03-17 08:38:04.000000 nextpcg-0.3.1/pypapi/dispatch.py
--rw-rw-rw-   0        0        0     2124 2023-03-17 08:38:04.000000 nextpcg-0.3.1/pypapi/dson.py
--rw-rw-rw-   0        0        0     3061 2023-04-11 04:04:20.000000 nextpcg-0.3.1/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    14387 2023-03-29 08:40:38.000000 nextpcg-0.3.1/pypapi/field.py
--rw-rw-rw-   0        0        0     1835 2023-02-20 07:01:34.000000 nextpcg-0.3.1/pypapi/field_heightfield.py
--rw-rw-rw-   0        0        0     1098 2023-03-28 09:08:32.000000 nextpcg-0.3.1/pypapi/field_instanced_staticmesh.py
--rw-rw-rw-   0        0        0     1060 2023-03-28 09:08:38.000000 nextpcg-0.3.1/pypapi/field_texture.py
--rw-rw-rw-   0        0        0     9095 2023-03-17 08:38:04.000000 nextpcg-0.3.1/pypapi/geo.py
--rw-rw-rw-   0        0        0     9503 2023-02-20 07:01:34.000000 nextpcg-0.3.1/pypapi/geo_heightfield.py
--rw-rw-rw-   0        0        0     6603 2023-02-20 07:01:34.000000 nextpcg-0.3.1/pypapi/geo_instanced_staticmesh.py
--rw-rw-rw-   0        0        0    13392 2023-03-29 08:35:32.000000 nextpcg-0.3.1/pypapi/geo_texture.py
--rw-rw-rw-   0        0        0      160 2023-02-20 07:01:34.000000 nextpcg-0.3.1/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-20 07:01:34.000000 nextpcg-0.3.1/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:37:48.292205 nextpcg-0.3.1/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-17 08:38:04.000000 nextpcg-0.3.1/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-03-17 08:38:04.000000 nextpcg-0.3.1/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-17 08:38:04.000000 nextpcg-0.3.1/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-04-11 07:37:48.296194 nextpcg-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2435 2023-04-11 07:37:15.000000 nextpcg-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:54:21.347160 nextpcg-0.4.0/
+-rw-rw-rw-   0        0        0       72 2023-03-17 08:38:04.000000 nextpcg-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1321 2023-04-11 07:54:21.346162 nextpcg-0.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-11 07:54:21.203826 nextpcg-0.4.0/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1321 2023-04-11 07:54:21.000000 nextpcg-0.4.0/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-04-11 07:54:21.000000 nextpcg-0.4.0/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-11 07:54:21.000000 nextpcg-0.4.0/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-04-11 07:54:21.000000 nextpcg-0.4.0/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-04-11 07:54:21.000000 nextpcg-0.4.0/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-11 07:54:21.000000 nextpcg-0.4.0/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-03-02 08:29:40.000000 nextpcg-0.4.0/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-11 07:54:21.337188 nextpcg-0.4.0/pypapi/
+-rw-rw-rw-   0        0        0      749 2023-03-17 08:38:04.000000 nextpcg-0.4.0/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-03-17 08:38:04.000000 nextpcg-0.4.0/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-04-11 03:30:49.000000 nextpcg-0.4.0/pypapi/const.py
+-rw-rw-rw-   0        0        0     5482 2023-03-17 08:38:04.000000 nextpcg-0.4.0/pypapi/dispatch.py
+-rw-rw-rw-   0        0        0     2124 2023-03-17 08:38:04.000000 nextpcg-0.4.0/pypapi/dson.py
+-rw-rw-rw-   0        0        0     3061 2023-04-11 04:04:20.000000 nextpcg-0.4.0/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    14387 2023-03-29 08:40:38.000000 nextpcg-0.4.0/pypapi/field.py
+-rw-rw-rw-   0        0        0     1835 2023-02-20 07:01:34.000000 nextpcg-0.4.0/pypapi/field_heightfield.py
+-rw-rw-rw-   0        0        0     1098 2023-03-28 09:08:32.000000 nextpcg-0.4.0/pypapi/field_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0     1060 2023-03-28 09:08:38.000000 nextpcg-0.4.0/pypapi/field_texture.py
+-rw-rw-rw-   0        0        0     9095 2023-03-17 08:38:04.000000 nextpcg-0.4.0/pypapi/geo.py
+-rw-rw-rw-   0        0        0     9503 2023-02-20 07:01:34.000000 nextpcg-0.4.0/pypapi/geo_heightfield.py
+-rw-rw-rw-   0        0        0     6603 2023-02-20 07:01:34.000000 nextpcg-0.4.0/pypapi/geo_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0    13392 2023-03-29 08:35:32.000000 nextpcg-0.4.0/pypapi/geo_texture.py
+-rw-rw-rw-   0        0        0      160 2023-02-20 07:01:34.000000 nextpcg-0.4.0/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-20 07:01:34.000000 nextpcg-0.4.0/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-04-11 07:54:21.344169 nextpcg-0.4.0/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-17 08:38:04.000000 nextpcg-0.4.0/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-03-17 08:38:04.000000 nextpcg-0.4.0/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-17 08:38:04.000000 nextpcg-0.4.0/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-04-11 07:54:21.348158 nextpcg-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2435 2023-04-11 07:54:02.000000 nextpcg-0.4.0/setup.py
```

### Comparing `nextpcg-0.3.1/PKG-INFO` & `nextpcg-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.3.1
+Version: 0.4.0
 Summary: pypapi module in NextPCG
 Home-page: https://glacier-request-888.notion.site/Wiki-f2600ce902b743f3ac7a40322496390a
 Author: IEGG
 Author-email: cheneyshen@tencent.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nextpcg-0.3.1/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.4.0/nextpcg.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.3.1
+Version: 0.4.0
 Summary: pypapi module in NextPCG
 Home-page: https://glacier-request-888.notion.site/Wiki-f2600ce902b743f3ac7a40322496390a
 Author: IEGG
 Author-email: cheneyshen@tencent.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `nextpcg-0.3.1/nextpcg.egg-info/SOURCES.txt` & `nextpcg-0.4.0/nextpcg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/__init__.py` & `nextpcg-0.4.0/pypapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/__main__.py` & `nextpcg-0.4.0/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/dispatch.py` & `nextpcg-0.4.0/pypapi/dispatch.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/dson.py` & `nextpcg-0.4.0/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/dson_create.py` & `nextpcg-0.4.0/pypapi/dson_create.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/field.py` & `nextpcg-0.4.0/pypapi/field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/field_heightfield.py` & `nextpcg-0.4.0/pypapi/field_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/field_instanced_staticmesh.py` & `nextpcg-0.4.0/pypapi/field_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/field_texture.py` & `nextpcg-0.4.0/pypapi/field_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/geo.py` & `nextpcg-0.4.0/pypapi/geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/geo_heightfield.py` & `nextpcg-0.4.0/pypapi/geo_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/geo_instanced_staticmesh.py` & `nextpcg-0.4.0/pypapi/geo_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/geo_texture.py` & `nextpcg-0.4.0/pypapi/geo_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/meta_helper.py` & `nextpcg-0.4.0/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/pantry/dson_generator.py` & `nextpcg-0.4.0/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/pypapi/plugin_protocol.py` & `nextpcg-0.4.0/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.3.1/setup.py` & `nextpcg-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='IEGG',
-    version='0.3.1',
+    version='0.4.0',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```

