# Comparing `tmp/egune-0.2.6.tar.gz` & `tmp/egune-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egune-0.2.6.tar", last modified: Mon Apr  3 08:06:58 2023, max compression
+gzip compressed data, was "egune-0.2.7.tar", last modified: Tue Apr 11 02:52:42 2023, max compression
```

## Comparing `egune-0.2.6.tar` & `egune-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 bilguun   (1000) docker     (999)        0 2023-04-03 08:06:58.984581 egune-0.2.6/
--rw-r--r--   0 bilguun   (1000) docker     (999)     1073 2023-02-10 02:45:00.000000 egune-0.2.6/LICENSE
--rw-rw-r--   0 bilguun   (1000) docker     (999)      342 2023-04-03 08:06:58.984581 egune-0.2.6/PKG-INFO
--rw-r--r--   0 bilguun   (1000) docker     (999)        0 2023-02-10 02:45:00.000000 egune-0.2.6/README.md
-drwxrwxr-x   0 bilguun   (1000) docker     (999)        0 2023-04-03 08:06:58.984581 egune-0.2.6/egune/
--rw-r--r--   0 bilguun   (1000) docker     (999)        0 2023-03-01 04:05:07.000000 egune-0.2.6/egune/__init__.py
--rw-rw-r--   0 bilguun   (1000) docker     (999)     4704 2023-03-30 06:15:28.000000 egune-0.2.6/egune/dataclasses.py
--rw-rw-r--   0 bilguun   (1000) docker     (999)     3162 2023-03-21 04:20:36.000000 egune-0.2.6/egune/definitions.py
--rw-rw-r--   0 bilguun   (1000) docker     (999)    13848 2023-03-02 07:34:54.000000 egune-0.2.6/egune/difference.py
--rw-rw-r--   0 bilguun   (1000) docker     (999)     2946 2023-03-01 03:20:55.000000 egune-0.2.6/egune/enumerators.py
--rw-r--r--   0 bilguun   (1000) docker     (999)     2119 2023-03-01 07:45:48.000000 egune-0.2.6/egune/logger.py
--rw-r--r--   0 bilguun   (1000) docker     (999)     4777 2023-03-01 03:10:50.000000 egune-0.2.6/egune/utils.py
-drwxrwxr-x   0 bilguun   (1000) docker     (999)        0 2023-04-03 08:06:58.984581 egune-0.2.6/egune.egg-info/
--rw-r--r--   0 bilguun   (1000) docker     (999)      342 2023-04-03 08:06:58.000000 egune-0.2.6/egune.egg-info/PKG-INFO
--rw-r--r--   0 bilguun   (1000) docker     (999)      310 2023-04-03 08:06:58.000000 egune-0.2.6/egune.egg-info/SOURCES.txt
--rw-r--r--   0 bilguun   (1000) docker     (999)        1 2023-04-03 08:06:58.000000 egune-0.2.6/egune.egg-info/dependency_links.txt
--rw-rw-r--   0 bilguun   (1000) docker     (999)       13 2023-04-03 08:06:58.000000 egune-0.2.6/egune.egg-info/requires.txt
--rw-r--r--   0 bilguun   (1000) docker     (999)        6 2023-04-03 08:06:58.000000 egune-0.2.6/egune.egg-info/top_level.txt
--rwxr-xr-x   0 bilguun   (1000) docker     (999)       68 2023-02-10 02:45:00.000000 egune-0.2.6/egunesh
--rw-rw-r--   0 bilguun   (1000) docker     (999)       38 2023-04-03 08:06:58.984581 egune-0.2.6/setup.cfg
--rw-r--r--   0 bilguun   (1000) docker     (999)      631 2023-03-30 06:17:28.000000 egune-0.2.6/setup.py
+drwxrwxr-x   0 bilguun   (1000) bilguun   (1000)        0 2023-04-11 02:52:42.567734 egune-0.2.7/
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)     1073 2023-02-10 02:45:00.000000 egune-0.2.7/LICENSE
+-rw-rw-r--   0 bilguun   (1000) bilguun   (1000)      342 2023-04-11 02:52:42.567734 egune-0.2.7/PKG-INFO
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)        0 2023-02-10 02:45:00.000000 egune-0.2.7/README.md
+drwxrwxr-x   0 bilguun   (1000) bilguun   (1000)        0 2023-04-11 02:52:42.567734 egune-0.2.7/egune/
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)        0 2023-03-01 04:05:07.000000 egune-0.2.7/egune/__init__.py
+-rw-rw-r--   0 bilguun   (1000) bilguun   (1000)     4704 2023-03-30 06:15:28.000000 egune-0.2.7/egune/dataclasses.py
+-rw-rw-r--   0 bilguun   (1000) bilguun   (1000)     3165 2023-04-11 02:52:07.000000 egune-0.2.7/egune/definitions.py
+-rw-rw-r--   0 bilguun   (1000) bilguun   (1000)    13848 2023-03-02 07:34:54.000000 egune-0.2.7/egune/difference.py
+-rw-rw-r--   0 bilguun   (1000) bilguun   (1000)     2946 2023-03-01 03:20:55.000000 egune-0.2.7/egune/enumerators.py
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)     2119 2023-03-01 07:45:48.000000 egune-0.2.7/egune/logger.py
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)     4777 2023-03-01 03:10:50.000000 egune-0.2.7/egune/utils.py
+drwxrwxr-x   0 bilguun   (1000) bilguun   (1000)        0 2023-04-11 02:52:42.567734 egune-0.2.7/egune.egg-info/
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)      342 2023-04-11 02:52:42.000000 egune-0.2.7/egune.egg-info/PKG-INFO
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)      310 2023-04-11 02:52:42.000000 egune-0.2.7/egune.egg-info/SOURCES.txt
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)        1 2023-04-11 02:52:42.000000 egune-0.2.7/egune.egg-info/dependency_links.txt
+-rw-rw-r--   0 bilguun   (1000) bilguun   (1000)       13 2023-04-11 02:52:42.000000 egune-0.2.7/egune.egg-info/requires.txt
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)        6 2023-04-11 02:52:42.000000 egune-0.2.7/egune.egg-info/top_level.txt
+-rwxr-xr-x   0 bilguun   (1000) bilguun   (1000)       68 2023-02-10 02:45:00.000000 egune-0.2.7/egunesh
+-rw-rw-r--   0 bilguun   (1000) bilguun   (1000)       38 2023-04-11 02:52:42.567734 egune-0.2.7/setup.cfg
+-rw-r--r--   0 bilguun   (1000) bilguun   (1000)      631 2023-04-11 02:52:22.000000 egune-0.2.7/setup.py
```

### Comparing `egune-0.2.6/LICENSE` & `egune-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `egune-0.2.6/egune/dataclasses.py` & `egune-0.2.7/egune/dataclasses.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.6/egune/definitions.py` & `egune-0.2.7/egune/definitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                     entity_val = userMessage.get_entity_val(entity_name)
                     if entity_val is not None:
                         filled_slots[slotName] = SlotVal(
                             slotName, entity_name, entity_val, None)
                         break
                 else:
                     for intent, value in slotDef.intent:
-                        if intent == userMessage.intent.chosen:
+                        if intent in userMessage.intent.positives:
                             filled_slots[slotName] = SlotVal(
                                 slotName, None, value, None)
                             break
 
         return Issue(
             id=Issue.new_id() if id is None else id,
             type=self.type,
```

### Comparing `egune-0.2.6/egune/difference.py` & `egune-0.2.7/egune/difference.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.6/egune/enumerators.py` & `egune-0.2.7/egune/enumerators.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.6/egune/logger.py` & `egune-0.2.7/egune/logger.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.6/egune/utils.py` & `egune-0.2.7/egune/utils.py`

 * *Files identical despite different names*

### Comparing `egune-0.2.6/setup.py` & `egune-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='egune',
-    version='0.2.6',
+    version='0.2.7',
     scripts=['egunesh'],
     author="Bilguun Chinzorig",
     author_email="bilguun@bolorsoft.com",
     description="Egune Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
```

